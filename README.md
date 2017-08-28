# nginx-for-android

* Basic Configuration
```
./auto/configure \
--crossbuild=android-x86_64 \
--prefix=/sdcard/nginx \
--with-cc=/Users/sanghwa/android-r15-x86_64/bin/x86_64-linux-android-gcc \
--with-pcre=/Users/sanghwa/project/nginx/thirdparty/pcre-8.41 \
--with-cc-opt=-Wno-sign-compare
```

* ssl Configiration
```
./auto/configure \
--crossbuild=android-x86_64 \
--prefix=/sdcard/nginx \
--with-host=x86_64-linux-android \
--with-cc=/Users/sanghwa/android-r15-x86_64/bin/x86_64-linux-android-gcc \
--with-pcre=/Users/sanghwa/project/nginx/thirdparty/pcre-8.41 \
--with-openssl-opt="android" \
--with-openssl=/Users/sanghwa/project/nginx/thirdparty/openssl-1.0.2l \
--with-http_ssl_module \
--with-cc-opt=-Wno-sign-compare
```
