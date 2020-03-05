---
title: "HITYAVIE. Yet another visual inertial estimator."
collection: projects
permalink: /projects/yavie
excerpt: 'Yet another visual inertial estimator(YAVIE). This is a hands on project for fun.'
date: 2020-1-01
---
# hityavie
Yet another visual inertial estimator(YAVIE). See [here](https://github.com/hitdshu/hityavie)

This is a hands on project for fun. I don't want to write any detail about this repo since no one would actually check it carefully. Though I learned a lot and got a lot of fun while creating it.

## Structrue from motion
See folder sfm. This folder contains a monocular visual odometry module which can run with only image infomation.

## Visual inertial odometry
See folder yavie. We don't use sliding window(schur complement) to limit the computation. Instead the double window optimization(see ORB-SLAM for details) is used here. There maybe many bugs in this code. The way we utilize imu information is borrowed shamelessly from VINS-MONO. Currently loop closing is not contained in the repo.

## Some demo images
Initialization success. See pictures/init.png.

Tracking. See pictures/tracking.png, pictures/tracking2.png.

Blue boxes are trajectories of cameras. Purple points are map points while the green are currently observed points.
