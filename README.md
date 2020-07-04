# elasticsearch-lab

This is a simple playbook i use to configure an LXC container in proxmox as a full elkstack. I'll add more bits and pieces as I need them. 

July 2020 - I added significant changes here - configuring passwords for users, adding xpack security, getting it working mostly in one go.

Problems:
- Sometimes apt fails on the logstash install, not sure why yet, but running the playbook again fixes it. 

Thanks:
- The kibana template was lifted from [here](https://github.com/geerlingguy/ansible-role-kibana) to save time. 
- Took a lot of examples from the https://github.com/elastic/ansible-elasticsearch, especailly for the http posts. 

To Do:
- Parameterize more stuff
- make this more flexible
- enable HTTPS with let's encrypt certs
- add index mappings at startup
- add dashboards and visualizations 