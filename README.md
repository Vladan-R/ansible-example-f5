### Ansible example - F5 configuration
This is an example of F5 change prepared for execution by Ansible.

- The change implements logging of F5 syslog messages to regional Splunk servers.
- Ansible connectivity towards F5s is handled via SSH tunnel to a jump server.

**Change steps are:**
1. Pre checks.
2. Determining next hop for managment route towards Splunk.
3. Implementation of management route.
3. Implementation of logging configuration.
4. Saving configuration.
5. Syncing configuration from Active to Standby F5.
6. Post checks.