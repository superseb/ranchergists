# Rancher tools

**Note: Repository archived on Jan 20 2025, archived copy for reference or free to re-use**

**Note: this is not official documentation, make sure you have a backup and test it before applying any of this**

Index of miscellaneous non official gists/tools for Rancher

## Release notes

Find all Rancher/RKE/k3s/RKE2 release notes and component info in [./release-notes](./release-notes).

## Versions

Find all k3s/RKE2 release channels in [./CHANNELS.md](./CHANNELS.md).

[![Latest stable](https://img.shields.io/badge/dynamic/yaml?label=Rancher%20stable&query=%24.entries.rancher%5B0%5D.appVersion&url=https%3A%2F%2Freleases.rancher.com%2Fserver-charts%2Fstable%2Findex.yaml)](https://github.com/rancher/rancher/releases)
[![Latest](https://img.shields.io/badge/dynamic/yaml?label=Rancher%20latest&query=%24.entries.rancher%5B0%5D.appVersion&url=https%3A%2F%2Freleases.rancher.com%2Fserver-charts%2Flatest%2Findex.yaml)](https://github.com/rancher/rancher/releases)

![RKE2 stable](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fupdate.rke2.io%2Fv1-release%2Fchannels&query=%24.data%5B%3F(%40.name%20%3D%3D%20%22stable%22)%5D.latest&label=RKE2%20stable)
![RKE2 latest](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fupdate.rke2.io%2Fv1-release%2Fchannels&query=%24.data%5B%3F(%40.name%20%3D%3D%20%22latest%22)%5D.latest&label=RKE2%20latest)
![RKE2 testing](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fupdate.rke2.io%2Fv1-release%2Fchannels&query=%24.data%5B%3F(%40.name%20%3D%3D%20%22testing%22)%5D.latest&label=RKE2%20testing)

![k3s stable](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fupdate.k3s.io%2Fv1-release%2Fchannels&query=%24.data%5B%3F(%40.name%20%3D%3D%20%22stable%22)%5D.latest&label=k3s%20stable)
![k3s latest](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fupdate.k3s.io%2Fv1-release%2Fchannels&query=%24.data%5B%3F(%40.name%20%3D%3D%20%22latest%22)%5D.latest&label=k3s%20latest)
![k3s testing](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fupdate.k3s.io%2Fv1-release%2Fchannels&query=%24.data%5B%3F(%40.name%20%3D%3D%20%22testing%22)%5D.latest&label=k3s%20testing)

## Gists

- [Retrieve kubeconfig for custom cluster from Rancher](https://gist.github.com/superseb/f6cd637a7ad556124132ca39961789a4)
- [Retrieve kubeconfig from RKE or Rancher 2 custom cluster controlplane node for RKE v0.2.x+ and Rancher v2.2.x+](https://gist.github.com/superseb/b14ed3b5535f621ad3d2aa6a4cd6443b)
- [Recover cluster.rkestate using kubeconfig](https://gist.github.com/superseb/649a64bdbca51e0cba5341d94608ae48)
- [Recover cluster.rkestate file from controlplane node](https://gist.github.com/superseb/e9f2628d1033cb20e54f6ee268683a7a)
- [Rancher v2.6.3 and up single install embedded etcd maintenance](https://gist.github.com/superseb/bcfeb07931b70b8722b77f1fbd791e99)
- [Rancher v2.x single install embedded etcd query](https://gist.github.com/superseb/d27253befe5e180334162c18187212fb)
- [Check kubelet nodefs/imagefs](https://gist.github.com/superseb/a4fa9640d801c54452132db8af51f2e4)
- [Run WebSocket test for Rancher 2](https://gist.github.com/superseb/89972344508e99b9336ad7eff78cb928)
- [cluster.rkestate to kubeconfig](https://gist.github.com/superseb/acb944e39c0166ec33aa1c43b5c61f8c)
- [CNI interface per pod](https://gist.github.com/superseb/4e0577a93ced88fa6fe5c39d2d778060)
- [Delete evicted pods using kubectl](https://gist.github.com/superseb/0f654d4e8945195e08fd1a2a061e0762)
- [Create local user and generate kubeconfig in Rancher 2 via API](https://gist.github.com/superseb/cad9b87c844f166b9c9bf97f5dea1609)
- [Extended Rancher 2 cleanup for custom cluster hosts](https://gist.github.com/superseb/06539c6dcd377e118d72bfefdd444f81)
- [Single command etcd snapshot restore to inspect etcd contents](https://gist.github.com/superseb/d6560a18ce5df47bac01477203b87950)
- [curl a gist to generate self signed certificates](https://gist.github.com/superseb/b2c1d6c9baa32609a49ee117a27bc700) 
```
curl https://gist.githubusercontent.com/superseb/b2c1d6c9baa32609a49ee117a27bc700/raw/7cb196e974e13b213ac6ec3105971dd5e21e4c66/selfsignedcert.sh | bash -s -- test.example.com
```
- [Generate CA, intermediate CA and server certificate with DNS alt names using Terraform in Docker and launch Rancher](https://gist.github.com/superseb/14ce3c94e0d6896bb43b19b70543be67)
- [Generate ECDSA CA, intermediate CA and server certificate with DNS alt names using Terraform in Docker and launch Rancher
](https://gist.github.com/superseb/610800c387c1d099fa86020fbcf908d9)
- [PLEG tester](https://gist.github.com/superseb/af32314125aac8e0aa7546239db55f82)
- [k3s etcd commands](https://gist.github.com/superseb/0c06164eef5a097c66e810fe91a9d408)
- [RKE2/rancherd2 commands](https://gist.github.com/superseb/3b78f47989e0dbc1295486c186e944bf)
- [Minio using Let's Encrypt certbot obtained certificates](https://gist.github.com/superseb/b8fd848525d68168cbaa4c8f1f44608e)
- [Minio + NGINX in Docker using self signed certificates](https://gist.github.com/superseb/32c439aac5097723f395acc77c47e829)
- [Rancher check stored cluster secret for fullState and state](https://gist.github.com/superseb/84025e1eeb7158ed97015aa9331fe3db)
- [Retrieve cluster.rkestate for Rancher c-c-XXXXX cluster secret reconstruction](https://gist.github.com/superseb/4a78a0ac34a36eacaa9e6440729619c3)
- [Get RKE config for worker node in Rancher 2.x](https://gist.github.com/superseb/117efe9faaa6655c7483e92209033c6d)

## Tools

- [ranchercheck: Check certificate chain on your Rancher 2 install](https://github.com/superseb/ranchercheck)

## Repositories

- [tf-do-rancher2: Automated Rancher single install and custom cluster with nodes using API and shell scripts](https://github.com/superseb/tf-do-rancher2)
- [multipass-rke: RKE cluster on multipass instances](https://github.com/superseb/multipass-rke)
- [multipass-k3s: k3s cluster on multipass instances](https://github.com/superseb/multipass-k3s)
- [multipass-rke2: rke2 cluster on multipass instances](https://github.com/superseb/multipass-rke2)
- [kdmq (kdmquery): show/diff kontainer-driver-metadata data (k8s/images/addons)](https://github.com/superseb/kdmq)

## Deprecated

No longer applicable, end of life, does not exist anymore etc... still here for archive

- [Rancher v2.1.8 single install embedded etcd maintenance](https://gist.github.com/superseb/48037c0323147e603bc0197bd5ecb9b5)
- [Rancher v2.2.0 single install embedded etcd maintenance](https://gist.github.com/superseb/f223b15949c031983da2cb850f56a897)
- [Rancher v2.5.x single install embedded etcd maintenance](https://gist.github.com/superseb/c8d0188302fdbd0127e52cf6ce93ce94)
- [Rancher v2.6.x single install embedded etcd maintenance](https://gist.github.com/superseb/566960fa1ebbb0891cf11b0cdf255369)
- [Retrieve kubeconfig from RKE v0.1.x or Rancher v2.0.x/v2.1.x custom cluster controlplane node](https://gist.github.com/superseb/3d8de6092ebc4b1581185197583f472a)
- [Roll nodes in a Rancher 2 custom cluster using DigitalOcean droplets](https://gist.github.com/superseb/922f3be6eacc89fcc31a45353dc5aaf5)
- [Run nodelocal DNS on Rancher 2 custom cluster (RKE)](https://gist.github.com/superseb/0500a758cdb8bbac5dc47ca570738a1d)
- [Run kube-dns preferably on controlplane nodes and else on etcd nodes on a Rancher 2 custom cluster](https://gist.github.com/superseb/893e1d5b1e4fd19160d9611dbe63d073)
- [Extract self signed CA certificate from Rancher](https://gist.github.com/superseb/2732303f0c85d6aca8fab617ea262ebb)
- [Debug EKS cluster created in Rancher](https://gist.github.com/superseb/c6e8581eef5d01518b17544c07ea4032)
- [tf-do-rancher16: Automated Rancher 1.6 single install and custom cluster with nodes using API and shell scripts](https://github.com/superseb/tf-do-rancher16)
- [tf-do-rancherd: Automated rancherd single install and custom cluster with nodes using API and shell scripts](https://github.com/superseb/tf-do-rancherd)
- [tf-do-rancher2-airgap: Terraform config to launch Rancher 2.0 in a simulated airgapped environment](https://github.com/superseb/tf-do-rancher2-airgap/)
- [Katacoda: Explore RKE2](https://katacoda.com/superseb/scenarios/rke2)
- [Katacoda: Explore K3s](https://katacoda.com/superseb/scenarios/k3s)
- [Katacoda: Import K3s in Rancher 2](https://www.katacoda.com/superseb/scenarios/rancher2-k3s-import)
- [Katacoda: Import RKE2 in Rancher 2.5](https://katacoda.com/superseb/scenarios/rancher25-rke2-import)
- [Katacoda scenarios source](https://github.com/superseb/katacoda-scenarios)
