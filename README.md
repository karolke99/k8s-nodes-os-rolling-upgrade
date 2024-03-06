# k8s-nodes-os-rolling-upgrade

This repository contains ansible roles that upgrades operating system on Kubernetes cluster's nodes.

## Tested OS distro
* Ubuntu 20.04 -> Ubuntu 22.04 upgrade

## How to

1. Clone this repo
2. Set configuration in [`defaults/main.yml`](os-rolling-upgrade/defaults/main.yml).
3. Provide list of hosts in inventory file (e.g. `hosts`).
4. Run playbooks

    ```bash
    $ ansible-playbook -i hosts ./os-upgrade.yml
    ```

5. Wait untill the upgrade is done.
