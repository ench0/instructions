sudo apt-get install aptitude
sudo aptitude update 
sudo aptitude dist-upgrade
sudo apt-get install ubuntu-restricted-addons ubuntu-restricted-extras 
sudo aptitude install bison build-essential curl flex git gnupg gperf libesd0-dev libncurses5-dev libsdl1.2-dev libwxgtk2.8-dev libxml2 libxml2-utils lzop openjdk-7-jdk openjdk-7-jre pngcrush schedtool squashfs-tools xsltproc zip zlib1g-dev
sudo aptitude install g++-multilib gcc-multilib lib32ncurses5-dev lib32readline-gplv2-dev lib32z1-dev 
sudo aptitude install git-core gnupg flex bison python rar original-awk gawk p7zip-full gperf libsdl1.2-dev libesd0-dev libwxgtk2.6-dev squashfs-tools build-essential zip curl libncurses5-dev zlib1g-dev pngcrush schedtool libc6-dev x11proto-core-dev libx11-dev libg11-mesa-dev mingw32 tofrodos python-markdown libxml2-utils g++-multilib lib32z1-dev ia32-libs lib32ncurses5-dev lib32readline-gplv2-dev gcc-multilib g++-multilib xsltproc
sudo aptitude install optipng
nano .bashrc 
#######
# enable bash completion in interactive shells
if ! shopt -oq posix; then
  if [ -f /usr/share/bash-completion/bash_completion ]; then
    . /usr/share/bash-completion/bash_completion
  elif [ -f /etc/bash_completion ]; then
    . /etc/bash_completion
  fi
fi
export USE_CCACHE=1
PATH="/home/ensar/bin:$PATH"
#######
cd android/pac
prebuilts/misc/linux-x86/ccache/ccache -M 25G
nano ~/.profile
#######
# ~/.profile: executed by Bourne-compatible login shells.

if [ "$BASH" ]; then
  if [ -f ~/.bashrc ]; then
    . ~/.bashrc
  fi
fi

mesg n
PATH="/home/ensar/bin:$PATH"
#######

?sudo apt-get install libcap-dev texinfo automake libgmp-dev
sudo apt-get install oracle-java7-installer
sudo update-java-alternatives -s java-7-oracle
sudo update-alternatives --config java
sudo apt-get install git-review

export USE_PREBUILT_CHROMIUM=1
