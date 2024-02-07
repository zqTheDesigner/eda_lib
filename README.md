set this repo as a submodule
```sh
git submodule add git@github.com:zqTheDesigner/eda_lib.git
git submodule update --init --recursive
```

In another repo, pull from submodule
```sh
git pull --recursive-submodules
```

To pull a repo contains submodule, add --recursive flag
```sh
git clone --recursive <project url>
```
or if the repo already cloned, use
```sh
git submodule update --init --recursive
```

If there is no .gitmodules folder, create one
```
[submodule "eda_lib"] 
  path = eda_lib
  url = git@github.com:zqTheDesigner/eda_lib.git
```