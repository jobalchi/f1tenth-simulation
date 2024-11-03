# F1tenth-simulation
F1tenth simulation for ROS1 Noetic.
This copyright is in the official F1TENTH repository.

## Installation (Native Ver.)
The environment officially supports Python3, Python2 might also work. You'll need several dependencies to run this environment:

### Eigen and protobuf dependencies:
```bash
$ sudo apt install libzmq3-dev build-essential autoconf libtool libeigen3-dev
$ sudo cp -r /usr/include/eigen3/Eigen /usr/include
```

### Python packages:
```bash
$ pip3 install numpy scipy numba zmq pyzmq Pillow gym==0.18.0 protobuf==3.20.0 pyyaml msgpack llvmlite empy wheel
```

### Then install the env via the following steps:
```bash
$ cd f1tenth_gym
$ mkdir -p build
$ cd build
$ cmake ..
$ make
$ cp sim_requests_pb2.py ../gym/
$ cd ..
$ pip3 install -e gym/
```
