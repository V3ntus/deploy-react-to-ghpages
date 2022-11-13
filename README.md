## Deploy React app to gh-pages 

This Action will automate the process of building and depolying react app to gh-pages.

## Notice:  
This fork introduces the `--force` flag. Do not use unless you know what you're doing

## Action 
Add this action inside your Repository's Actions

```
name: React app deployement

on:
  push:
    branches: [ master ]
  pull_request:
    branches: [ master ]

jobs:
  build:

    runs-on: ubuntu-latest
    
    steps:
    - uses: actions/checkout@v2

    - name: Deploy react app to github pages
      uses: tanwanimohit/deploy-react-to-ghpages@v1.0.1
```
