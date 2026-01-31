The goal is to provide Debian and Ubuntu nightly packages ready to be installed with minimal impact on the distribution.
Packages are available for amd64, i386 (Debian only), s390x and arm64 (aka aarch64). This for both the stable, qualification and development branches (currently 20, 21 and 22).

Packages are built using stage2 and extremely similar to the one shipping in Debian & Ubuntu.

Usage
```
name: Test
on: push

jobs:
  build:
    name: Test
    runs-on: ubuntu-24.04
    steps:

    - name: Free disk space
      uses: sirpdboy/actions@install-llvm

```


