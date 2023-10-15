## How to build .so from code

### Reference URL

https://www.php.net/manual/en/imagick.installation.php

### Build

Unpack `7.1.1-20.tar.gz` and then from terminal issue the following commands:
1.  cd ImageMagick-7.1.1

2.  ./configure

3.  make

If ImageMagick configured and compiled without complaint, you are ready to install it on your system. Administrator privileges are required to install. To install, type the following command in terminal:

1.  sudo make install

To check your ImageMagick installation enter the following command in terminal:

1. make check


Next we need to install Imagick.so which is what we want for PHP.

First of all we need to get the right file and we can get that from here:

Unpack the `imagick-3.7.0.tgz` file and then enter the commands in quotes in terminal:

1.  cd imagick-3.7.0

2.   phpize

3.   ./configure --with-imagick=/opt/local

4.   make

5.   make install
