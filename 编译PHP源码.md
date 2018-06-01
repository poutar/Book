### 编译PHP源码

```shell
> ./configure  
  --with-apxs2=/home/apache/bin/apxs	//编译php成为apache的一个模块
  --with-mysqli 
  --with-openssl
  --with-curl=/usr/bin/curl
  --enable-zip
  --enable-mbstring
  --disable-fileinfo
> make
> make install

```

