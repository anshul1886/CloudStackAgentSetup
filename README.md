CloudStackAgentSetup
====================

This conatins the source code to generate the clickable Installer for CloudStack Agent for Hyperv

To use this source code you have to copy CloudStackAgentSetup project folder in cloudstack source code at follwing location
(cloudstack src folder)/plugins/hypervisors/hyperv/DotNet/ServerResource

You can build the code using msbuild as follows 

**msbuild  CloudAgentSetup.wixproj**

This will generate the installer in bin/Debug folder 
