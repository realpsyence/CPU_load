# CPU and GPU load script 

This script generates a desired CPU load and forces it per each core on 
machines running Ubuntu.

It requires *stress* and *cpulimit* to be installed on the target machine:

	- sudo apt-get install stress cpulimit

Usage: 

	- ./cpuload.sh [cpu load in percent] [duration in seconds]
	- ./cpuload.sh 25 10

Additionally, if *glmark2* is installed on the target machine:

  - sudo apt-get install glmark2 

The script will run glmark2 for the duration of the test when a 
third argument is given. This third argument can be anything.

Usage:
  - ./stress\_test.sh [cpu load in percent] [duraction in seconds] [test gpu]
  - ./stress\_test.sh 25 10 1
