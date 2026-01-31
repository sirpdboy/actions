Show system info

Usage
```
name: Test
on: push

jobs:
  build:
    name: Test
    runs-on: ubuntu-24.04
    steps:
      - name: Show system info
        uses: sirpdboy/actions@show-system
       
