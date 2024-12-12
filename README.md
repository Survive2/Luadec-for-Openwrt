默认编译的lua与luadec是lua5.1的，默认为32位，如果需要64位，需要更改lua-5.1/src下的Makefile与luadec/luadec下的Makefile，去掉CFLAGS与MYLDFLAGS中的-m32
# Usage
```sh
git clone https://github.com/Survive2/Luadec-for-Openwrt.git
cd Luadec-for-Openwrt
cd luadec/lua-5.1
make linux
cd ../luadec
make LUAVER=5.1
```
