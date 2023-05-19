# SPDK Storage Management Agent Go API bindings

This repository contains golang API bindings for SPDK Storage Management Agent's (SMA) gRPC
interface.  More details on SMA can be found in [SPDK documentation](https://spdk.io/doc/sma.html).

Generating SMA Go API from spdk into sma-goapi:

```
git clone https://github.com/spdk/spdk
git clone https://github.com/spdk/sma-goapi
spdk/scripts/pkgdep.sh --golang
source /etc/opt/spdk-pkgdep/paths/export.sh
spdk/scripts/gen_sma_goapi.sh -o sma-goapi
cd sma-goapi
git add *
git commit -m "Generated from SPDK $(cd ../spdk && git describe)"
```
