# random_numbers

*This branch has been ported to ROS 2.0*

This library contains wrappers for generating floating point values, integers, quaternions using boost libraries.

## Build Status

ros2 branch: [![Build Status](https://travis-ci.com/ros-planning/random_numbers.svg?branch=ros2)](https://travis-ci.com/ros-planning/random_numbers)

## Features

New: you can pass in a custom random number generator seed to allow optional deterministic behavior during debugging, testing, etc. using the secondary constructor.
