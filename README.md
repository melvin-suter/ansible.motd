# ansible.motd

Generates a motd automatically.

# Usage for projects

Add the role at the end.
See the magic happen.

# Usage for other roles
somewhere in your variables do this:
```
rolename_motd_roles:
  - rolename
motd_roles: "{{ motd_roles + rolename_motd_roles }}"
```
```
rolename_motd__commands:
  - my command
  - systemctl restart this
motd_commands: "{{ motd_commands + rolename_motd_commands }}"
```
