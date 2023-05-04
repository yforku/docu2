# Docusaurus

* <https://doit.vlsm.org/013.html>
* <https://doit.vlsm.org/014.html>
* <https://osp4diss.vlsm.org/osp-102.html>
* <https://osp4diss.vlsm.org/osp-103.html>

```
export DEBS="
aptitude
git
sudo
vim
"

```

```
date;
time apt-get install $DEBS -y
time (aptitude update&&echo " =1= "&&aptitude safe-upgrade -y&&echo " =2= "&&aptitude autoclean -y;)

```

```
[ -d /etc/sudoers.d/ ] && echo "cbkadal    ALL=(ALL:ALL) ALL" > /etc/sudoers.d/cbkadal

````

* <https://osp4diss.vlsm.org/osp-106.html>
* <https://osp4diss.vlsm.org/osp-107.html>
* <https://osp4diss.vlsm.org/osp-108.html>
* <https://osp4diss.vlsm.org/osp-109.html>
* <https://osp4diss.vlsm.org/osp-112.html>
* <https://osp4diss.vlsm.org/osp-132.html>

```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash

```

```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

```

```
nvm ls-remote
nvm install v18.16.0
node -v
npm install yarn
yarn --version
```

```
mkdir -vp $HOME/docusaurus/
cd $HOME/docusaurus/

```

```
npm init docusaurus@latest docu2 classic

```

```
cd $HOME/docusaurus/docu2/
npm run start -- --host 0.0.0.0

```

```
npm run build
npm run serve

```

```
GIT_USER=cbkadal USE_SSH=true yarn deploy

```

```
npm audit fix

```


