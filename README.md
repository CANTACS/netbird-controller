# Netbird-Controller

An Ansible playbook to deploy the Netbird controller on a server.

*This was built for CANTACS and suits our needs, but probably will not suit yours.  You might need to do some customization work to use this successfully.*

---

Set the IP of the controller in the inventory file.

#### Set the 1Password Environment Variable:
On Linux/MacOS:
```
export OP_SERVICE_ACCOUNT_TOKEN=
```

#### Install the role:
```
ansible-galaxy install -r roles/requirements.yml -p ./roles
```

#### Options:
|Option|Values|Description|
|---|---|---|
|`ufw-setup`|`true` or `false`|Ensures UFW is installed and configured with the required Netbird ports|
