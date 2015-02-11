Usage:
 
    sudo apt-get install git-review
    git clone https://github.com/PAC-man/android_vendor_pac
    cd android_vendor_pac
    <make edits>
    git add -A
    git commit -m "Message"
    git-review
 
OR you can use the convential method:
 
    cd <project>
    <make edits>
    git add -A
    git commit -m "Message"
    git push ssh://<username>@review.pac-rom.com:29418/<project> HEAD:refs/for/pac-4.4
 
 
The git-review package will only have to be installed once.
 
If you are going to make additional edits, just repeat steps, but instead of using:
 
    git commit -m "Message"
 
use:
 
    git commit --amend
