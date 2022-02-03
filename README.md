# Ansible Playbook to install RKE2 
You can install a RKE2 cluster with kubevip with this Playbook

# Example cluster config
``` 
---
kubernetesVersion: v1.22.5+rke2r2
token: xxx
tlssan:
    - test
    - test2
kubevip:
  enabled: false
  controlplane: true
  controlplaneVip: 192.168.178.5
  interface: eth0
  services: false
  cloudProvider: true
```


# TODOs
- [] add calico
````
cni:
  - calico
````
- [] Install rke2 via binary
