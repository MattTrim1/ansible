# debian11

This playbook brings a brand new Debian 11 server up to a known state.

It installs various packages, creates a user with passwordless root, and restricts SSH access.

To run the playbook, use the following command:

`ansible-playbook -i HOSTNAME, playbooks/debian11/playbook.yml --extra-vars "ansible_control_plane_ip=CONTROL_PLANE_IP`
