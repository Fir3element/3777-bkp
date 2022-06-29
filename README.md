## Useful links
### Binaries
- x32 (visual studio): https://github.com/Fir3element/binaries/raw/master/x32.rar
- x32 (dev-cpp): https://github.com/Fir3element/binaries/raw/master/x32_dev.rar
- x64 (visual studio): https://github.com/Fir3element/binaries/raw/master/x64.rar

### Source
- https://github.com/Fir3element/3777/archive/master.zip

### Dev cpp
- https://github.com/Fir3element/binaries/raw/master/dev-cpp.rar

### MSVC10 libs and includes
- https://github.com/Fir3element/binaries/raw/master/vc10_pack.rar

## Libraries for Visual Studio 2022 (using vcpkg)

```
vcpkg install --triplet x64-windows luajit sqlite3 libmysql libxml2 gmp boost-filesystem boost-regex boost-thread boost-asio
```

## Build instruction for Ubuntu

```
sudo apt-get update
```

```
sudo apt-get install --no-install-recommends -y git autoconf automake pkg-config build-essential liblua5.1-0-dev libsqlite3-dev libmysqlclient-dev libxml2-dev libgmp3-dev libboost-filesystem-dev libboost-regex-dev libboost-thread-dev
```

```
git clone https://github.com/Fir3element/3777.git
```

```
cd /3777-master/src
```

```
sudo chmod +x autogen.sh
```

```
./autogen.sh
```

```
./configure --enable-sqlite --enable-mysql --enable-root-permission --enable-server-diag
```

```
./build.sh
```
