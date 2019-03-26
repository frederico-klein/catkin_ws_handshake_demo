# Handshake workspace repository

## Getting started

Clone recursively with:

    git clone --recursive https://github.com/frederico-klein/catkin_ws_handshake_demo.git
    
See https://www.vogella.com/tutorials/GitSubmodules/article.html for a nice little tutorial about submodules.
    
Install all the dependencies from the packages with:

    rosdep install --from-paths src --ignore-src -r -y
    
Run catkin_make.

If you've never ran any serial comms program before in your pc, you need to add yourself to dialout group, log off and on again:

    sudo usermod -a -G dialout $USER

## Usage

make sure to "source devel/setup.bash" from the catkin-workspace

open separate terminal shells ( at least 4)

run the following commands in separate windows:

    roslaunch gummi_base_template manager.launch
    roslaunch gummi_base_template controllers.launch
    roslaunch gummi_interface gummi.launch
    roslaunch gummi_demo_handshake hand_shake_all.launch
