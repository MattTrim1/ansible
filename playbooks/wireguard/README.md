# wireguard

Contains a playbook to deploy a brand new Wireguard VPN. Usage:

`ansible-playbook -i HOSTNAME, deploy.yml --extra-vars "wireguard_srv_private_key=PRIVATEKEY"`

Also contains a playbook to add a new client to the Wireguard config on the server.

`ansible-playbook -i HOSTNAME, add_client.yml --extra-vars "client_pub_key=CLIENT_PUBLIC_KEY" --extra-vars "client_cidr=CLIENT_ALLOWED_IPS"`
