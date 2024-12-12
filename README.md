# Luadec-for-Openwrt
用来反编译Openwrt下的lua字节码<br>
感谢viruscamp(https://github.com/viruscamp/luadec.git)
# 说明
默认编译的lua与luadec是lua5.1的，默认为32位，如果需要64位，需要更改lua-5.1/src下的Makefile与luadec/luadec下的Makefile，去掉CFLAGS与MYLDFLAGS中的-m32标志。<br>

# 示例:<br>
使用原版luadec反编译会报错：<br>
![image](https://github.com/user-attachments/assets/3ce78119-b993-4908-8172-ded061e95937)<br>

使用更改后的luadec反编译成功：<br>
![image](https://github.com/user-attachments/assets/b592a1c0-1639-47ce-98c7-44edee0660e5)<br>

# Usage
```sh
git clone https://github.com/Survive2/Luadec-for-Openwrt.git
cd Luadec-for-Openwrt
cd luadec/lua-5.1
make linux
cd ../luadec
make LUAVER=5.1
```
