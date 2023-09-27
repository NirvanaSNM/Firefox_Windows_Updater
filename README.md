# Firefox_Windows_Updater
Ansible playbook that checks if Firefox is installed on Windows machines and installs the latest version if it is not already installed.

Code Analysis:

Inputs
windows_hosts: The hosts on which the playbook will be executed.

Flow
The playbook starts by checking if Firefox is already installed on the Windows hosts.
If Firefox is not installed, the playbook proceeds to fetch the latest version of Firefox from the Mozilla API.
The playbook then downloads the latest version of Firefox and updates the installation if the installed version is not the latest.
After the update, the playbook validates the newly installed Firefox version.
Finally, the playbook sets a fact with the latest installed Firefox version.

Outputs
mstr_firefox_latest_version: The latest installed Firefox version.
