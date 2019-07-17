# Yaffey
Automatically exported from code.google.com/p/yaffey

###  Building Yaffey on Mac:
```sh
brew install qt #install qt version 4.x
git clone https://github.com/danielkutik/yaffey.git
cd yaffey
qmake
make
mv yaffey.app /Applications/
```

### Building Yaffey on Ubuntu 18.04:
```sh
sudo apt-get install libqt4-dev
git clone https://github.com/DavisDevasia/yaffey
vi yaffey/yaffs2/yaffs_guts.h
```
Replace `typedef unsigned loff_t;` with `#include <stdlib.h>` and save.
```sh
cd yaffey
qmake && make
./yaffey
```

See also: http://askubuntu.com/a/281178/11339
