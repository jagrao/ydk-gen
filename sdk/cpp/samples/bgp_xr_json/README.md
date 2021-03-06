# YDK C++ BGP JSON Samples for XR
###Prerequisite
First install the [system requirements](https://github.com/CiscoDevNet/ydk-gen#system-requirements). Then follow the [ydk-gen README](https://github.com/CiscoDevNet/ydk-gen#usage) and generate/install the C++ core, [ietf bundle](https://github.com/CiscoDevNet/ydk-gen/blob/master/profiles/bundles/ietf_0_1_1.json) and [cisco-ios-xr bundle](https://github.com/CiscoDevNet/ydk-gen/blob/master/profiles/bundles/cisco-ios-xr_6_1_2.json).
### 1) Build the sample apps
```
$ mkdir build && cd build
$ cmake ..
$ make && sudo make install
$ cd ..
```

### 2) Run the apps

Note: `-v` will turn on verbose mode
```
$ cd build
$ ./bgp_xr_write ssh://<username>:<password>@<host address>:<port> [-v]
$ ./bgp_xr_read ssh://<username>:<password>@<host address>:<port> [-v]
```
