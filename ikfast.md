export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:/media/7c969b45-e4db-4fa3-9e23-7f3d8a3c9470/home/kohlbrecher/thor/src/thor_mang/thor_mang_common/

rosrun collada_urdf urdf_to_collada thor_mang_simple.urdf thor_mang_simple.dae

rosrun moveit_ikfast round_collada_numbers.py thor_mang_simple.dae thor_mang_simple_rounded.dae 5

openrave-robot.py thor_mang_simple_rounded.dae --info links


#thor right leg:
python `openrave-config --python-dir`/openravepy/_openravepy_/ikfast.py --robot=thor_mang_simple_rounded.dae --iktype=transform6d --baselink=0 --eelink=12 --savefile=r_leg.cpp

#thor right arm without final rotation:
python `openrave-config --python-dir`/openravepy/_openravepy_/ikfast.py --robot=thor_mang_simple_rounded.dae --iktype=transform6d --baselink=14 --eelink=30 --savefile=r_arm_thor_utorso_to_r_arm_wrist_roll.cpp

#thor right arm to right hand with free index
python `openrave-config --python-dir`/openravepy/_openravepy_/ikfast.py --robot=thor_mang_simple_rounded.dae --iktype=transform6d --baselink=14 --eelink=32 --savefile=r_arm_thor_utorso_to_r_hand.cpp --freeindex=29

#thor right leg
python `openrave-config --python-dir`/openravepy/_openravepy_/ikfast.py --robot=thor_mang_simple_rounded.dae --iktype=transform6d --baselink=0 --eelink=12 --savefile=r_arm_thor_pelvis_to_r_foot.cpp


#With database:
openrave.py --database inversekinematics --robotgit =thor_arm_right.xml --usecached --perftiming=100000

#thor_arm_right.xml:
<Robot name="thor_arm_right" file="thor_mang_simple_rounded.dae">
  <Manipulator name="thor_arm_right">
    <base>utorso</base>
    <effector>r_hand</effector>
    <direction>1 0 0</direction>
    <translation>0 0 0</translation>
  </Manipulator>
</Robot>

#compile:
g++ -lstdc++ -llapack -o ik r_leg.cpp 