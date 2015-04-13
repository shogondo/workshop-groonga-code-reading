# 環境構築メモ

## 1. パッケージインストール

```
sudo apt-get -V -y install wget tar build-essential zlib1g-dev liblzo2-dev libmsgpack-dev libzmq-dev libevent-dev libmecab-dev gdb git
```

### 2. Groongaをビルド

```
wget http://packages.groonga.org/source/groonga/groonga-5.0.2.tar.gz
tar zxf groonga-5.0.2.tar.gz
cd groonga-5.0.2
./configure CFLAGS="-O0 -g3" CXXFLAGS="-O0 -g3"
make
```
