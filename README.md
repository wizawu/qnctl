qnctl
===

### Build

```
apt-get install golang

cd /path/to/qnctl
GOPATH=$PWD/Godeps/_workspace go build
```

### Usage

```
qnctl help

export QINIU_AK=...
export QINIU_SK=...
export QINIU_BUCKET=test

qnctl add images/ ~/001.png
qnctl add images/003.png ~/002.png

qnctl stat images/001.png
qnctl stat images/002.png    # no such file or directory
qnctl stat images/003.png

qnctl rm images/001.png
qnctl rm images/003.png
```
