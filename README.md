forked from [moovweb/gvm](https://github.com/moovweb/gvm), 替换 Go 源, 解决 gvm 的 go 源被墙无法使用问题



## Changes

| replace                                | to                                 |
| -------------------------------------- | ---------------------------------- |
| https://go.googlesource.com/go         | https://github.com/golang/go       |
| https://storage.googleapis.com/golang/ | http://mirrors.ustc.edu.cn/golang/ |



## Usage

```shell
# install
zsh < <(curl -s -S -L https://raw.githubusercontent.com/xinjie-canya/gvm/master/binscripts/gvm-installer)

gvm

gvm listall

gvm install go1.4
gvm use go1.4 [--default]

# install go1.4+
gvm install go1.4 -B
gvm use go1.4
export GOROOT_BOOTSTRAP=$GOROOT
gvm install go1.5

# uninstall
rm -rf ~/.gvm
```
