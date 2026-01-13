# npk-repo

> this official repository of Nowa Package Keeper(NPK).

## Docs:

how to install packages? 

```sh
npk.sh -i package # install package

npk.sh -r package # remove package

npk.sh -l # list of installed packages

npk.sh -s package # sync(update package)

npk.sh -v # see version

npk.sh -u # upgrade npk

npk.sh -cleanup # clean trash made by npk
```

how to install npk to my pc?

first of all, requirements:
- linux
- bash >= 3.1
- tar and wget

```sh
wget https://raw.githubusercontent.com/Naharashu/npk-repo/main/npk.tar.gz 

mkdir -p $HOME/npk

tar -xvzf npk.tar.gz -C $HOME/npk

rm -f npk.tar.gz

chmod +x $HOME/npk/npk.sh

chmod +x $HOME/npk/npk-upgrade.sh

sudo ln -s $HOME/npk/npk.sh /usr/local/bin/npk  # on linux

ln -s $HOME/npk/npk.sh $PREFIX/bin/npk # on Termux
```

pros:
- fast and lightweight(100 lines of bash script)
- have security against dependency cycles
- easy to use
- rolling release
- have backups of old packages in ~/npk/old/
- required only minimal linux environment, bash and tar
