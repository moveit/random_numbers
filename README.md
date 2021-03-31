# random_numbers

This library contains wrappers for generating floating point values, integers, quaternions using boost libraries.

## Build Status

[![BuildAndTest](https://github.com/ros-planning/random_numbers/actions/workflows/industrial_ci_action.yaml/badge.svg?branch=master)](https://github.com/ros-planning/random_numbers/actions/workflows/industrial_ci_action.yaml?branch=master)
[![Format](https://github.com/ros-planning/random_numbers/actions/workflows/format.yaml/badge.svg?branch=master)](https://github.com/ros-planning/random_numbers/actions/workflows/format.yaml?branch=master)

## Features

New: you can pass in a custom random number generator seed to allow optional deterministic behavior during debugging, testing, etc. using the secondary constructor.
