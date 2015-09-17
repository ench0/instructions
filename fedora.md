sudo yum install -y zip curl gcc gcc-c++ flex bison gperf glibc-devel.{x86_64,i686} zlib-devel.{x86_64,i686} ncurses-devel.i686 libX11-devel.i686 libstdc++.i686 readline-devel.i686 libXrender.i686 libXrandr.i686 perl-Digest-MD5-File python-markdown mesa-libGL-devel.i686 git schedtool pngcrush lzma nano

#opt
su -c 'dnf remove java-1.8.0-openjdk'
su -c 'dnf remove java-1.8.0-openjdk-devel'

prebuilts/misc/linux-x86/ccache/ccache -M 50G

nano .bashrc
###
# User specific aliases and functions
export PATH=~/bin:$PATH
export USE_CCACHE=1
###
git config --global user.email "x@y.net"
git config --global user.name "xx"

sudo alternatives --install /usr/bin/java java /usr/java/latest/bin/java 1
sudo update-alternatives --config java
java -version
