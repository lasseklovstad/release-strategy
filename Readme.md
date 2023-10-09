## Setup

### 1. Generate deploy key: `ssh-keygen`

The deploy key is used to create and push new branches to the repository.
Then we can use is here.

```
 - uses: actions/checkout@v4
   with:
     ref: development
     ssh-key: ${{ secrets.ADMIN_DEPLOY_KEY }}
```

### 2. Allow github actions to approve pull requests

Go to Settings / Actions / General and select the option.
