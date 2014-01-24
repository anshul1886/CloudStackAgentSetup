CloudStackAgentSetup
====================

This conatins the source code to generate the clickable Installer for CloudStack Agent for Hyperv

To use this source code you have to copy InstallerSetup project folder in cloudstack source code at follwing location
(cloudstack src folder)/plugins/hypervisors/hyperv/DotNet/

After copying the installer code go to CloudStackAgentSetup folder

**cd (cloudstack src folder)/plugins/hypervisors/hyperv/DotNet/InstallerSetup/CloudStackAgentSetup **

You can build the code using msbuild as follows 

**msbuild.exe  CloudAgentSetup.wixproj**

This will generate the installer in (cloudstack src folder)/plugins/hypervisors/hyperv/DotNet/InstallerSetup/CloudStackAgentSetup/bin/Debug folder 
