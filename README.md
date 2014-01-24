CloudStackAgentSetup
====================

This conatins the source code to generate the clickable Installer for CloudStack Agent for Hyperv

It does the following

- packages all the needed files
- Prompts for user\password the HyperV agent should run under
- Option to create and install an SSL certificate since the communication between mgmt server and HyperV agent is secure. One has also an option to install a different ssl certificate. Procedure to install the certificate onto HyperV agent is https://cwiki.apache.org/confluence/display/CLOUDSTACK/Manually+Creating+and+installing+self+signed+certificate+for+CloudStack+Management+Server+communication+with+Hyper-V+agent .
- option to update, upgrade and downgrade the installation.


To use this source code you have to copy InstallerSetup project folder in cloudstack source code at follwing location
(cloudstack src folder)/plugins/hypervisors/hyperv/DotNet/

After copying the installer code go to CloudStackAgentSetup folder

**cd (cloudstack src folder)/plugins/hypervisors/hyperv/DotNet/InstallerSetup/CloudStackAgentSetup**

You can build the code using msbuild as follows 

**msbuild.exe  CloudAgentSetup.wixproj**

This will generate the installer in (cloudstack src folder)/plugins/hypervisors/hyperv/DotNet/InstallerSetup/CloudStackAgentSetup/bin/Debug folder

This code uses the WixCommonUiExtension.dll with eclipse public license https://github.com/dblock/msiext/blob/master/LICENSE
