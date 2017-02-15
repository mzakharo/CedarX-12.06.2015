# CedarX-12.06.2015
This is new CedarX library from Allwinner with Chinese documentation and example C application...

#Compile CedarX library
```
cd  CedarX-12.06.2015
export WORKSPACE=$(pwd)
export PREFIX=/usr/local
cd $WORKSPACE/src/
./bootstrap 
./configure --prefix=$PREFIX
make
sudo make install
```
Install H.264/JPEG Encoder Binary
```
sudo install $WORKSPACE/binary/libcedar_plugin_venc.so $PREFIX/lib/cedarx/
```

Add CedarX library LD Path
```
sudo echo $PREFIX/lib/cedarx >> /etc/ld.so.conf
ldconfig
```
