This is a Github Action to checkout Git repos that doesn't depend on NodeJS (or anything else except git), so that you can continue to checkout repos even on older machines.

Use it like this:

```
on:
  pull_request:
  push:

jobs:
  default:
    runs-on: ubuntu-latest
    steps:
      - uses: iffy/checkoutnodeps@v0.1.0
```
