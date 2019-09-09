# Firekube

Firekube is a Kubernetes cluster working on top of [ignite][gh-ignite] and
using GitOps for its management.

## Creating a Firekube cluster

1. Fork this repository.

1. Clone your fork and `cd` into it:

```console
git clone git@github.com:$user/wks-quickstart-firekube.git
cd wks-quickstart-firekube
```

1. Create an SSH key pair:

```console
ssh-keygen -t rsa -b 4096 -C "damien+firekube@weave.works" -f deploy-firekube  -N ""
```

1. Upload the deploy to your fork (with read/write access):

1. Start the cluster:

```console
cd wks-quickstart-firekube
./setup.sh --git-deploy-key  ./deploy-firekube
```

This step will take several minutes.

1. Profit!

[gh-ignite]: https://github.com/weaveworks/ignite
[gh-firecracker]: https://github.com/firecracker-microvm/firecracker
