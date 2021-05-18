# Kubeadm deployment to Ubuntu 20.04

You need: 

1. ansible installed on your local computer.
2. ssh public key to be copied to server machines for passwordless access.
3. hosts file to be changed according to your server nodes IP addresses.

Run playbooks with command:

> ansible-playbook -i hosts ansible-playbook-file.yml

Run ansible playbooks in following order:

1. initial.yml
2. set_hostname.yml
2. kube-dependencies.yml
3. master.yml
4. workers.yml
