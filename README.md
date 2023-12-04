# Synopsis

This Ansible Asset is intended for getting TSM Container Capacity reports


# Variables

Variable | Default| Comments
----------|-----------------|--------
execution_node (String) | - | **Mandatory**. Hostname of the endpoint as configured in Ansible Tower inventory. It should be having active connectivity with TSM Server.
reportdir  (String) | - | **Mandatory**.  /SP_CONTAINER_REPORTS should be created on the endpoint/execution node to store the logs for temp basis

# Results from execution
After successful execution, We collect the TSM Contianer capacity reports and for mentioned TSM Server
Here is the list of return codes that this asset returns.

Return Code Group | Return Code | Comments
----------|--------------|---------


# Procedure

Container_report Playbook is responsible to collect the TSM Container capacity report (having connectivity with TSM Servers) to collect the data and save to the endpoint server.

# Support

# Known problems and limitations
* No known problems and limitations as of know within the scope of this automation.

# Prerequisites
* python 3.6 (release 3.6.3) or above
* "execution_node" variable should be configured in Job Template details section with hostname that is configured in inventory. This host should have connectivity enabled with TSM Server.
* TSM admin should have the rights to issue the select commands to collect the data for containers.

# Examples

Instructions to use this role 

1- Use Extra Variables section in Job Template to pass values to __execution_node__

# License

