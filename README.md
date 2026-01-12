# npk-repo

> this official repository of Nowa Package Keeper(NPK).

## Docs:

how to install packages? 

```bash
./npk.sh -i package # install package

./npk.sh -r package # remove package

./npk.sh -l # list of installed packages

./npk.sh -s package # sync(update package)

./npk.sh -cleanup # clean trash made by npk
```

pros:
- fast and lightweight(100 lines of bash script)
- have security against dependency cycles
- easy to use
- rolling release
- have backups of old packages in ~/npk/old/
- required only minimal linux environment, bash and tar