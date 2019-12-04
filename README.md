# Wheelchair Auto-Pilot Software 

This repository contains the ROS package software used to launch the autonomous system to drive the Eightfold Smart Chair.


This package relies on the following ROS package:
      - wc_llc
      - wc_perception 
      - video_stream_opencv
      - image_view 



# Running the Code

This is used to launch the ROS nodes and i/f sofware to send control data to the Eightfold 
  SMART Chair Interface, and to activate the perception module to run the CNN.  

In order to run this package the following devices need to be connected and powered up:
  - usb camera 
  - Seagate mass storage device
  - USB to Eightfold Smaert Chair Arduino serial port


Use the following examples to perform the ROS launch command, when launching on a platform that can also display ROS image_view images:

         roslaunch wc_auto chair.full.launch

Here are other examples: 


         roslaunch wc_auto chair.full.launch video_stream_provider:=1 buffer_queue_size:=1 

         roslaunch wc_auto chair.full.launch onboard_images_folder:='/media/nvidia/Seagate Backup Plus Drive/Data/WC/WC_PERCEPTION/onboard_images' 

         roslaunch wc_auto chair.full.launch arduino_device_name:="/dev/ttyUSB0"


