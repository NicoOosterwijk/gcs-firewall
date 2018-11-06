## About
This repostory provides the `gcloud` tool to manage google cloud platform.  


Firewall Rules
==============
## Google Compute Engine
### Roles:
- create
- delete

## How to use
You should setup your `gcloud` environment first, and you can refer to [here](https://cloud.google.com/compute/docs/gcloud-compute/#auth) to learn more about it.

# Create
## setup the required variables in the defaults var file of the create role.
There is a section for every rule with the following items:
- port
- name
- project
- source_ranges
- target
- protocol
- action

You can refer to [gcloud compute firewall-rules documentation](https://cloud.google.com/sdk/gcloud/reference/compute/firewall-rules/) for more details.

Run the create_firewall_rules playbook: **ansible-playbook create_firewall_rules.yaml**

# Delete
## Setup the preferred firewall rule items to delete in the defaults var file in the delete role.
Then run the delete_firewall_rules playbook: **ansible-playbook delete_firewall_rules.yaml**

