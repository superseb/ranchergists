| Version | Date | US date | EU date |
| ------- | ---- | ------- | ------- |
| [v1.5.15](rke-v1.5.md#release-v1515) | Nov 12 2024 | 11/12/24 | 2024-11-12 |
| [v1.5.14](rke-v1.5.md#release-v1514) | Oct 21 2024 | 10/21/24 | 2024-10-21 |
| [v1.5.13](rke-v1.5.md#release-v1513) | Sep 17 2024 | 09/17/24 | 2024-09-17 |
| [v1.5.12](rke-v1.5.md#release-v1512) | Aug 05 2024 | 08/05/24 | 2024-08-05 |
| [v1.5.11](rke-v1.5.md#release-v1511) | Jul 22 2024 | 07/22/24 | 2024-07-22 |
| [v1.5.10](rke-v1.5.md#release-v1510) | Jun 10 2024 | 06/10/24 | 2024-06-10 |
| [v1.5.9](rke-v1.5.md#release-v159) | May 13 2024 | 05/13/24 | 2024-05-13 |
| [v1.5.8](rke-v1.5.md#release-v158) | Apr 10 2024 | 04/10/24 | 2024-04-10 |
| [v1.5.7](rke-v1.5.md#release-v157) | Mar 27 2024 | 03/27/24 | 2024-03-27 |
| [v1.5.6](rke-v1.5.md#release-v156) | Mar 07 2024 | 03/07/24 | 2024-03-07 |
| [v1.5.5](rke-v1.5.md#release-v155) | Feb 13 2024 | 02/13/24 | 2024-02-13 |
| [v1.5.3](rke-v1.5.md#release-v153) | Jan 22 2024 | 01/22/24 | 2024-01-22 |
| [v1.5.2](rke-v1.5.md#release-v152) | Jan 17 2024 | 01/17/24 | 2024-01-17 |
| [v1.5.1](rke-v1.5.md#release-v151) | Dec 19 2023 | 12/19/23 | 2023-12-19 |
| [v1.5.0](rke-v1.5.md#release-v150) | Dec 01 2023 | 12/01/23 | 2023-12-01 |



## What's Changed
- Introduced `v1.28.15`

# RKE Kubernetes versions
- `v1.25.16-rancher2-3`
- `v1.26.15-rancher1-1`
- `v1.27.16-rancher1-1`
- `v1.28.15-rancher1-1` (default)


**Full Changelog**: https://github.com/rancher/rke/compare/v1.5.14...v1.5.15
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed
* Fix the issue where it may fail to remove the etcd+controlplane node from a cluster 
* Add ACI-CNI 6.1.1.1 variable

# RKE Kubernetes versions
- `v1.25.16-rancher2-3`
- `v1.26.15-rancher1-1`
- `v1.27.16-rancher1-1`
- `v1.28.14-rancher1-1` (default)


-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed

- Introduced `v1.28.13` 
- Introduced calico and canal  `v3.27.4` for `v1.28.13`
- Introduced nginx `v1.11.2` for `v1.28.13` 
- Introdced ACI `v6.0.4.3` for `v1.28.13`  

# RKE Kubernetes versions
- `v1.25.16-rancher2-3`
- `v1.26.15-rancher1-1`
- `v1.27.16-rancher1-1`
- `v1.28.13-rancher1-1` (default)

-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed

- Introduced `v1.28.12` and `v1.27.16`

# RKE Kubernetes versions
- `v1.25.16-rancher2-3`
- `v1.26.15-rancher1-1`
- `v1.27.16-rancher1-1`
- `v1.28.12-rancher1-1` (default)

-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed

- Introduced `v1.28.11` and `v1.27.15` (https://github.com/rancher/rke/pull/3620)
- Introduced ACI CNI v6.0.4.2 (https://github.com/rancher/rke/pull/3625)
- Fixed an issue with cluster provisioning and reconciling when using `extra_env` for `kube-api` (https://github.com/rancher/rke/pull/3599) 
- Fixed an issue with k8s >= 1.22 clusters where clusters would sporadically fail to scale etcd nodes (https://github.com/rancher/rke/pull/3536) 

# RKE Kubernetes versions
- `v1.25.16-rancher2-3`
- `v1.26.15-rancher1-1`
- `v1.27.15-rancher1-1`
- `v1.28.11-rancher1-1` (default)

-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed

Fixed an issue where an RKE provisioned cluster stores the cluster state in a configmap called `full-cluster-state` inside the `kube-system` namespace. This cluster state object contains information used to set up the Kubernetes cluster, which may include sensitive data. For more information, see [CVE-2023-32191](https://github.com/rancher/rke/security/advisories/GHSA-6gr4-52w6-vmqx).

# RKE Kubernetes versions
- `v1.25.16-rancher2-3`
- `v1.26.15-rancher1-1`
- `v1.27.14-rancher1-1`
- `v1.28.10-rancher1-1` (default)

-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed

- Bump containerd to v1.6.27. See https://github.com/rancher/rke/pull/3566
- Fix the issue where not all kube-apiserver containers restart after changing the Pod Security Admission Configuration. See https://github.com/rancher/rke/pull/3547

| Kubernetes version |
| ----- |
| `v1.25.16-rancher2-3` |
| `v1.26.15-rancher1-1` |
| `v1.27.13-rancher1-1` |
| `v1.28.9-rancher1-1` (default) |
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed

| Kubernetes version |
| ----- |
| `v1.25.16-rancher2-3` |
| `v1.26.15-rancher1-1` |
| `v1.27.12-rancher1-1` |
| `v1.28.8-rancher1-1` (default) |
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed
* [v1.28] Bump k8s dependencies to support k8s v1.28 by @chiukapoor in https://github.com/rancher/rke/pull/3472
* [v1.28] go generate by @chiukapoor in https://github.com/rancher/rke/pull/3507
* [release/v1.5] go generate by @github-actions in https://github.com/rancher/rke/pull/3513
* fix the bug that delete_local_data is dropped  by @jiaqiluo in https://github.com/rancher/rke/pull/3511
* [release/v1.5] go generate by @github-actions in https://github.com/rancher/rke/pull/3517
* [release/v1.5] go generate by @github-actions in https://github.com/rancher/rke/pull/3530
* Update README with latest versions by @thatmidwesterncoder in https://github.com/rancher/rke/pull/3528
* Backport v1.5.6 changes into the 1.5.7 release candidate line by @thatmidwesterncoder in https://github.com/rancher/rke/pull/3526
* [release/v1.5] go generate by @github-actions in https://github.com/rancher/rke/pull/3533
* Restart kube-apiserver in all CP nodes after changing the Pod Security Admission Configuration by @jiaqiluo in https://github.com/rancher/rke/pull/3531
* Revert "Merge pull request #3531 from jiaqiluo/fix-kube-apiserver" by @jiaqiluo in https://github.com/rancher/rke/pull/3537
* [release/v1.5] go generate by @github-actions in https://github.com/rancher/rke/pull/3541
* [v1.5] switch KDM branch to release-v2.8 by @jiaqiluo in https://github.com/rancher/rke/pull/3542

| Kubernetes version |
| ----- |
| `v1.28.7-rancher1-1` (default)|
|`v1.27.11-rancher1-1`|
|`v1.26.14-rancher1-1`|
|`v1.25.16-rancher2-3`|


**Full Changelog**: https://github.com/rancher/rke/compare/v1.5.6...v1.5.7
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed
* Add ACI CNI 6033, 6041 variables https://github.com/rancher/rke/pull/3514

| Kubernetes version |
| ----- |
| `v1.27.11-rancher1-1` (default)|
| `v1.26.14-rancher1-1`|
|`v1.25.16-rancher2-3` |

**Full Changelog**: https://github.com/rancher/rke/compare/v1.5.5...v1.5.6

-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

Note: There is no official release for v1.5.4, the next release version available after v1.5.3 is v1.5.5.  

## What's Changed
* Introduced `v1.27.10-rancher1-1` and `v1.26.13-rancher1-1` 
* Updated containerd to v1.6.27 and runc to v1.1.12 https://github.com/rancher/rke/pull/3495

## Kubernetes Versions 

Each version of RKE has a specific list of supported Kubernetes versions. If you want to use a different version than listed below, you will need to update Kubernetes using the [system images](https://rancher.com/docs/rke/latest/en/config-options/system-images/) option in your `cluster.yml`.

| Kubernetes version    |
| --------------------- |
| `v1.27.10-rancher1-1` (Default) |
| `v1.26.13-rancher1-1`  |
| `v1.25.16-rancher2-2`  |

| Experimental Kubernetes version |
| --------------------- |
| N/A | 

**Full Changelog**: https://github.com/rancher/rke/compare/v1.5.3...v1.5.5
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## What's Changed
* Add architecture.md by @manuelbuil in https://github.com/rancher/rke/pull/3453
* Clean/speed up Drone by @superseb in https://github.com/rancher/rke/pull/3417
* [release/v1.5] Simplify update README workflow by @superseb in https://github.com/rancher/rke/pull/3436
* [v1.5] Added ACI-CNI 6.0.3.2 variables by @akhilesh-oc in https://github.com/rancher/rke/pull/3475
* [v1.5] update kdm branch to release-v2.8 by @kinarashah in https://github.com/rancher/rke/pull/3479

| Kubernetes version    |
| --------------------- |
| `v1.27.8-rancher2-2` (Default) |
| `v1.26.11-rancher2-2`  |
| `v1.25.16-rancher2-2`  |

| Experimental Kubernetes version |
| --------------------- |
| N/A | 

**Full Changelog**: https://github.com/rancher/rke/compare/v1.5.2...v1.5.3
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## Enhancements

- Introduced `v1.27.8-rancher2-1`, `v1.26.11-rancher2-1` and `v1.25.16-rancher2-1`
- Introduced calico and canal `v3.26.3` and nginx ingress `v1.9.4` for `v1.27.8-rancher2-1`, `v1.26.11-rancher2-1` and `v1.25.16-rancher2-1`

## Bug Fixes

- Added ACI 6.0.3.1 variables

## Kubernetes Versions

Each version of RKE has a specific list of supported Kubernetes versions. If you want to use a different version than listed below, you will need to update Kubernetes using the [system images](https://rancher.com/docs/rke/latest/en/config-options/system-images/) option in your `cluster.yml`.

| Kubernetes version    |
| --------------------- |
| `v1.27.8-rancher2-1` (Default) |
| `v1.26.11-rancher2-1`  |
| `v1.25.16-rancher2-1`  |

| Experimental Kubernetes version |
| --------------------- |
| N/A | 

**Full Changelog**: https://github.com/rancher/rke/compare/v1.5.2...v1.5.1
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## Enhancements

- Introduced `v1.27.8-rancher2-1`, `v1.26.11-rancher2-1` and `v1.25.16-rancher2-1`
- Introduced calico and canal `v3.26.3` and nginx ingress `v1.9.4` for `v1.27.8-rancher2-1`, `v1.26.11-rancher2-1` and `v1.25.16-rancher2-1`

## Bug Fixes

## Kubernetes Versions

Each version of RKE has a specific list of supported Kubernetes versions. If you want to use a different version than listed below, you will need to update Kubernetes using the [system images](https://rancher.com/docs/rke/latest/en/config-options/system-images/) option in your `cluster.yml`.

| Kubernetes version    |
| --------------------- |
| `v1.27.8-rancher2-1` (Default) |
| `v1.26.11-rancher2-1`  |
| `v1.25.16-rancher2-1`  |

| Experimental Kubernetes version |
| --------------------- |
| N/A | 

**Full Changelog**: https://github.com/rancher/rke/compare/v1.5.1...v1.5.0
-----
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. With RKE, the installation and operation of Kubernetes are both simplified and easily automated, and they are entirely independent of the operating system and platform you're running.

## Enhancements
* Added support for `v1.27.6-rancher1-1`. 
* Introduced support for `external-aws`. 
  - In Kubernetes 1.27 and later, you must use an out-of-tree AWS cloud provider. See [documentation on how to set up external-aws](https://rke.docs.rancher.com/config-options/cloud-providers/aws#using-the-out-of-tree-aws-cloud-provider-for-rke).
  - All existing clusters must migrate prior to upgrading to v1.27 in order to stay functional. See [documentation on how to migrate to external-aws](https://rke.docs.rancher.com/config-options/cloud-providers/aws#migrating-to-the-out-of-tree-aws-cloud-provider-for-rke) on Kubernetes 1.26 and earlier. 
  - Note that there is a known issue with `external-aws` where RKE fails to find the node if both `hostname-override` and `internal-address` are empty. For more information, see https://github.com/rancher/rke/issues/3445 

## Other changes 
* [release/v1.5] Add env var to enable dual-stack in cri-dockerd by @superseb in https://github.com/rancher/rke/pull/3370
* [release/v1.5] Security bumps by @macedogm in https://github.com/rancher/rke/pull/3339
* Add warning log about weave deprecation by @manuelbuil in https://github.com/rancher/rke/pull/3337
* Fix "unknown revision v0.0.0" error caused by the k8s.io/kubernetes module by @jiaqiluo in https://github.com/rancher/rke/pull/3387
* changed etcd restore image to rke-tools for etcd >=3.5.7 by @vardhaman22 in https://github.com/rancher/rke/pull/3390

## Kubernetes Versions

Each version of RKE has a specific list of supported Kubernetes versions. If you want to use a different version than listed below, you will need to update Kubernetes using the [system images](https://rancher.com/docs/rke/latest/en/config-options/system-images/) option in your `cluster.yml`.

| Kubernetes version    |
| --------------------- |
| `v1.27.6-rancher1-1` (Default) | 
| `v1.26.9-rancher1-1`  |
| `v1.25.14-rancher1-1`  |

| Experimental Kubernetes version |
| --------------------- |
| N/A | 

## New Contributors
* @pjbgf made their first contribution in https://github.com/rancher/rke/pull/3410

**Full Changelog**: https://github.com/rancher/rke/compare/v1.4.11...v1.5.0
-----
