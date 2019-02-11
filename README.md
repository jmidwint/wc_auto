# Wheelchair Auto-Pilot Sofware 

This repository contains the ROS package software used to launch the autonomous system to drive the Eightfold Smart Chair.


This package relies on the followingt ROS package:
      - wc_llc
      - dronet_perception 
      - video_stream_opencv
      - image_view 



# Running the Code

This is used to launch the ROS nodes and i/f sofware to send control data to the Eightfold 
  SMART Chair Interface, and to activate the perception module to run the CNN.  

In order to run this package the following devices need to be connected and powered up:
  - usb camera 
  - Seagate mass storage device
  - Usb to Eightfold Smaert Chair Arduino serial port


Use the following examples to perform the ROS launch command:

         roslaunch wc_auto chair.full.launch

Here are other examples: 
         roslaunch wc_auto chair.full.launch video_stream_provider:=1 buffer_queue_size:=1 

         roslaunch wc_auto chair.full.launch onboard_images_folder:='/media/nvidia/Seagate Backup Plus Drive/Data/WC/DRONET_PERCEPTION/onboard_images' 


