Azure DHCP Deployment and Configuration
Overview
This PowerShell script automates the deployment and initial configuration of a DHCP server in Azure. The goal is to provide a quick and repeatable way to stand up DHCP services without requiring manual post-deployment configuration.

The script was designed as a learning project and focuses specifically on DHCP deployment and configuration tasks.

Features
Deploys the required DHCP server resources.
Applies DHCP configuration settings.
Reduces manual setup effort.
Provides a repeatable deployment process.


Limitations
The script does not validate existing DHCP infrastructure before deployment.
Azure may automatically assign DHCP leases to virtual machines before clients can request addresses, which can impact testing scenarios.
Error handling and environment-specific validation are intentionally minimal to keep the script simple and focused on demonstrating automation concepts.
Assumes the user has sufficient Azure permissions to create and configure resources.


Prerequisites
Running Locally
Install the Azure PowerShell (Az) modules:
Install-Module Az -Scope CurrentUser
Ensure execution policy is configured to run script