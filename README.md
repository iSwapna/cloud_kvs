# cloud_kvs
# 

This is a sample implementation of the PUSH based Gossip protocol.
The project is part of [Coursera Cloud Computing I](https://www.coursera.org/learn/cloud-computing/home/welcome)

 cloud_kvs provides:

* **Membership service** - 

* **Failure Detection** - 

* **Key/Value Storage** - TBD

* **Multi-Host** - TBD

Compiled using cmake with googletest integration, currently runs on Mac OS X.
TBD: Support for Linux with a demo on a true cluster.

 Build and install:
 
  $ `mkdir build`
  
  $ `cd build/`
  
  $ `cmake ..`
  
  $ `make install`
 
Running Gossip:

The `App` expects a few parameters in the form of a `*.conf` file, to simulate the network charecteristics. Examples can be found [here](https://github.com/swapnai/cloud_kvs/tree/master/main/testcases)

For example, to simulate a single node failure:

$ `cd <root/cloud_kvs>`

$ `App main/testcases/singlefailure.conf` 

If you make any changes to the code, run `make install` in order to rebuild and install


