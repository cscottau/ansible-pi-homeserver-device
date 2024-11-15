# ansible-pi-homeserver-device

Creates the encrypted external drive for the pi cloud, or if the parition exists, it will create the required configuration to decrypt it and open it.

Creates a key file to use to decrypt the volume

## Requires

This playbook uses the general and crypto community collections:

```
ansible-galaxy collection install community.general
ansible-galaxy collection install community.crypto
```

## Usage

`ansible-playbook site.yaml --ask-vault-pass`

Password is in the vault.