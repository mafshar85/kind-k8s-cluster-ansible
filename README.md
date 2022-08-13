# kind-k8s-cluster-ansible
creating a k8s cluster with kind & ansible tools for ubuntu 

## How to run
if you want to run it on vm ,copy your ssh-key to your vm

‍‍‍`ssh-copy-id  <username>@IP`

then edit the [hosts](./inventory/servers) file and replace your machin ip ,also edit [ansible-user](./roles/kind-cluster/vars/main.yml) and replace with your user

you can also edit cluster parameters from the [default folder](./roles/kind-cluster/defaults/main.yml)

`ansible-playbook playbook.yml  -i inventory/servers -K  -u <machine-username>`
