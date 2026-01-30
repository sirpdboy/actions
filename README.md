OpenWrt Build Setup (ubuntu-24.04)
Usage

```
name: Test
on: push

jobs:
  build:
    name: Test
    runs-on: ubuntu-24.04
    steps:
      - name: Checkout
        uses: actions/checkout@main

      - name: Build System Setup
        uses: sirpdboy/actions@build-setup


```
