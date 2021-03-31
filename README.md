# random_numbers

*This branch has been ported to ROS 2.0*

This library contains wrappers for generating floating point values, integers, quaternions using boost libraries.

## Build Status

[![BuildAndTest](https://github.com/ros-planning/random_numbers/actions/workflows/industrial_ci_action.yaml/badge.svg?branch=ros2)](https://github.com/ros-planning/random_numbers/actions/workflows/industrial_ci_action.yaml?branch=ros2)
[![Format](https://github.com/ros-planning/random_numbers/actions/workflows/format.yaml/badge.svg?branch=ros2)](https://github.com/ros-planning/random_numbers/actions/workflows/format.yaml?branch=ros2)

## Features

New: you can pass in a custom random number generator seed to allow optional deterministic behavior during debugging, testing, etc. using the secondary constructor.
