# dokku-gitversion

Sets an `APP_VERSION` config string for git deploys.   The format of the version string is `$deploy_branch.$updated_at`.  Where `$updated_at` is the seconds from Epoch of the last commit to the deploy branch.

If the deploy branch represents a version ending with a `.x` suffix e.g. `1.1.x`, the `.x` will be substituted with `$updated_at`.

## Installation

```
sudo dokku plugin:install https://github.com/AccountAim/dokku-gitversion.git
```
