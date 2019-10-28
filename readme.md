<img src="/RSK_Logo_RGB_300dpi.png" alt="logo" height="200" />

# Welcome to the precompiled ABIs from RSK repository. 

This repository contains the precompiled contracts used by RSK and was created to be used by npm package modules.

# Version
Different versions of the package mentioned are required for different RSK releases.

The semantic versioning of this package doesn’t correlate to the semantic versioning of RSK. For each named release of RSK, there will be a corresponding name version in npm.  

This package's support starts with ORCHID.

# How to use it. 
For the installation of these package you must execute in a terminal window:

         npm install @rsksmart/rsk-precompiled-abis@<version>

As an example to define and use it:

1) Include Web3 package.

         const Web3 = require('web3');

2) Include precompiled-abis package.

        const precompiled = require('@rsksmart/rsk-precompiled-abis');

3) Create an instance of the contract using package build method and Web3 as a parameter. 

    (i.e.: using Bridge)

        var bridge = precompiled.bridge.build(new Web3('http://localhost:4444'));

4) Example that explains how to use it using a contract's method. In this case calling getFederationAddress, and showing in console the result of this method.
        
        bridge.methods.getFederationAddress().call().then(console.log);


# Important note:
If the version to be installed is not defined in the command line, the version will correspond to the latest version in WASABI.

# Versioning table. 
| Package Version | RSK version   |  
|-----------------|---------------|
| 1.0.0-ORCHID    | ORCHID-0.6.2  |
| 2.0.0-WASABI    | WASABI-1.0.0  |
| 2.0.1-WASABI    | WASABI-1.0.0  | 
