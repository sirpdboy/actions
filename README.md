
ps: uses before actions/checkout

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
        uses: sirpdboy/actions@free-disk
        with:
          build-workdir: /builder

      - name: Checkout
        uses: actions/checkout@main

      - name: Build
        run: |
          echo "Free space:"
          df -h
```

