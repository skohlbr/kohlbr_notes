roscore

roslaunch vigir_worldmodel_server worldmodel_ocs.launch

rosrun topic_tools throttle  messages /move_group/scan_filtered_localized/splitted_scan 50 /move_group/scan_filtered_localized

/media/kohlbrecher/d13379a9-180b-4569-83e9-329f1c847bc7/logs/drc_finals/final_runs/log/finals
rosbag play out.bag --clock
