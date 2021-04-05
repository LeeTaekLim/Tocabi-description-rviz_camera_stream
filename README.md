Tocabi descrption + rviz_camera_stream
---

urdf.rviz, display.launch are modified.

## how to run

roslaunch tocabi_description display.launch 

## urdf.rviz

Rviz setting code for rviz_camera_stream is added to urdf.rviz.

## display.launch

Camera1 and camera2 nodes are added to display.launch.
'''
  <group ns="camera1">
  <node pkg="tf" type="static_transform_publisher" name="camera_broadcaster"
      args="1.0 0.0 0.87 -1.57 3.14 0.9 world camera1 10" />
'''
You can change the args. (args="x y z yaw pitch roll frame_id child_frame_id period_in_ms")
Camera 2 doesn't do anything so you can delete the code which is related to it.
