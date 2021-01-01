# QMK manifests of [krautcat](https://github.com/krautcat)'s keyboards

### Prerequisites

 * [repo](https://gerrit.googlesource.com/git-repo)

## How to start

```bash
mkdir qmk
cd qmk

repo init -u git@github.com:krautcat/qmk-manifests.git
repo sync -j$(($(nproc) * 2))

build/build init-workspace 

make git-init-submodule
```

Now you're ready to compile my keymaps!
