# ns
A dynamic Bash script enabling seamless navigation across Kubernetes namespaces and clusters interactively.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/mdwajid095/ns.git
```
2. Change the permission:
```bash
cd ns
sudo chmod +x ns
```
3. Set the PATH:
```bash
sudo mv ns /usr/local/bin
source ~/.bashrc
```
## Example
```bash
$ ns -h
```
![image](https://github.com/mdwajid095/ns/assets/55093597/772a8825-e466-47f2-a9c6-fbc1de17aa85)

```bash
$ ns wowsome
  Namespace has been set to 'default'

$ ns -c
  Current namespace is 'wowsome'

$ ns
  Clusters in VM 10.170.170.10:
       1  gke_europe-west3_gcp-cs-test-gke-1
       2  gke_europe-west3_gcp-cs-test-gke-2
  Enter the number of the cluster to be set: 2
  Switched to context "gke_europe-west3_gcp-cs-test-gke-2".
  Namespaces in gke_europe-west3_gcp-cs-test-gke-2:
       1  base
       2  default
       3  wowsome
       4  test
  Enter the number of the namespace to be set: 3
  Switched to context "gke_europe-west3_gcp-cs-test-gke-2".
  Context "gke_europe-west3_gcp-cs-test-gke-2" modified.
  Namespace has been set to 'wowsome' in gke_europe-west3_gcp-cs-test-gke-2
```
