image_pipeline
==============

[![CircleCI](https://circleci.com/gh/ros-perception/image_pipeline.svg?style=svg)](https://circleci.com/gh/ros-perception/image_pipeline)

This package fills the gap between getting raw images from a camera driver and higher-level vision processing.

For more information on this metapackage and underlying packages, please see [the ROS wiki entry](http://wiki.ros.org/image_pipeline).

For examples, see the [image_pipeline tutorials entry](http://wiki.ros.org/image_pipeline/Tutorials) on the ROS Wiki.  
  
##使い方
+ カメラからのimageトピックをenter keyを押すたびに保存する
画像を生成したい場所で:```rosrun image_view  extract_images  _sec_per_frame:=0.05 _filename_format:="image%04d.jpg"  image:=/usb_cam/image_raw ```
enter key受付プログラム:```rosrun image_view key_publisher```

