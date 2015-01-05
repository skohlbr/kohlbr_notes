export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:/media/7c969b45-e4db-4fa3-9e23-7f3d8a3c9470/home/kohlbrecher/thor/src/thor_mang/thor_mang_common/

rosrun collada_urdf urdf_to_collada thor_mang_simple.urdf thor_mang_simple.dae

rosrun moveit_ikfast round_collada_numbers.py thor_mang_simple.dae thor_mang_simple_rounded.dae 5

openrave-robot.py thor_mang_simple_rounded.dae --info links


#thor right leg:
python `openrave-config --python-dir`/openravepy/_openravepy_/ikfast.py --robot=thor_mang_simple_rounded.dae --iktype=transform6d --baselink=0 --eelink=12 --savefile=r_leg.cpp

#compile:
g++ -lstdc++ -llapack -o ik r_leg.cpp 