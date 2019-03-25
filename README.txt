make sure to "source devel/setup.bash" from the catkin-workspace

make separate windows (at least 4)

run the following commands in separate windows:

$: roslaunch gummi_base_template manager.launch
$: roslaunch gummi_base_template controllers.launch
$: roslaunch gummi_interface gummi.launch
$: roslaunch gummi_demo_handshake hand_shake_all.launch
