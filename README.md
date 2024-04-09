# liblzma-poc-demo

Demo is built on multipass.
go
x86_64 ONLY

> **Note:** Click [here](https://github.com/frozenprocess/Tigera-Presentations/tree/master/2023-03-30.container-and-Kubernetes-security-policy-design/04.best-practices-for-securing-a-Kubernetes-environment) If you want to learn more about policies.

# Setup the environment
Use the following command to setup nodes:
```bash
multipass launch -n control -c 2 -m 4096M -d 50G --cloud-init release/control-init.yaml https://cloud.debian.org/images/cloud/bookworm/latest/debian-12-genericcloud-amd64.qcow2
```

```bash
multipass launch -n node1 -c 2 -m 2096M -d 20G --cloud-init release/node-init.yaml https://cloud.debian.org/images/cloud/bookworm/latest/debian-12-genericcloud-amd64.qcow2
```


# Credits
[xzbot](https://github.com/amlweems/xzbot)