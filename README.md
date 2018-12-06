
# sip-doc

## Nikola Lukic tests

## Theory

- ITSPs (Internet Telephony Service Providers). 


## manual for freeSwitch master (1.8)

```bash
defaults write com.apple.finder AppleShowAllFiles YES

cd /usr/local                                 // Change to the /usr/local directory
sudo mkdir freeswitch src                     // Create the FreeSWITCH™ runtime and source directories
sudo chown -R `id -u`:`id -g` freeswitch src  // Change the owner of the two new directories to yours

brew install autoconf automake libtool

./bootstrap.sh   # <- Not for Current public release.

./configure

```

fix (missing) :

(configure: error: Library requirements (speex >= 1.2rc1 speexdsp >= 1.2rc1) not met; consider adjusting the PKG_CONFIG_PATH environment variable if your libraries are in a nonstandard prefix so pkg-config can find them.)

```
brew install speex
```



## help links

list :
https://www.cnblogs.com/welhzh/p/6782297.html

redicertion in pjsip:
https://trac.pjsip.org/repos/wiki/SIP_Redirection?format=pdf

For pjsip : 

INCOMING 

if answer is 101-199 
EARLY  

if answer is 200
CONFIRMED
