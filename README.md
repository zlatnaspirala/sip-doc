----------------------------------------------------------
----------------------------------------------------------
# sip-doc
----------------------------------------------------------
----------------------------------------------------------


## Nikola Lukic tests

----------------------------------------------------------
## Theory

- ITSPs (Internet Telephony Service Providers). 
- FQDN (fully qualified domain name).

 -The public switched telephone network (PSTN) is the aggregate of the world's circuit-switched telephone networks that are operated by national, regional, or local telephony operators, providing infrastructure and services for public telecommunication.

A "User Agent" ("UA") is an application used for handling a certain network protocol; the network protocol in <b>Sofia's</b> case is SIP. Sofia is the general name of any User Agent in FreeSWITCH using the SIP network protocol.

DSN : Data Source Names. 

A.C.L. stands for Access Control List and is a list of permissions associated with an object. The list defines what network entities are allowed to access the object.

ESL Program

## list :
https://www.cnblogs.com/welhzh/p/6782297.html
----------------------------------------------------------



----------------------------------------------------------
## manual for FREESwitch master (1.8)

"Don't modify it while freeswitch is running" conf/freeswitch.xml .

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

Note : 

Also you should NEVER override local_ip_v4, it will only get reset at some point. 

tool from bin 
'/usr/local/freeswitch/certs/CA/cakey.pem'

writing new private key to '/tmp/fs-ca-1230-20181207135330.key'

LIKE ECHO (from freeswitch terminal)
eval $${local_ip_v4}

Database connections are defined with DSN in XML configuration parameters like "core-db-dsn" and "odbc-dsn".

CMD : 

sofia status


CLI <=> event socket <=> FREESwitch


----------------------------------------------------------

----------------------------------------------------------
## PJSIP


redicertion in pjsip:
https://trac.pjsip.org/repos/wiki/SIP_Redirection?format=pdf

For pjsip : 

INCOMING 

if answer is 101-199 
EARLY  

if answer is 200
CONFIRMED

to the 6xx 


----------------------------------------------------------


About log from android device : 

Since Android 7.0, logcat has --pid filter option, and pidof command is available, replace com.example.app to your package name.
(ubuntu terminal / Since Android 7.0)

adb logcat --pid=`adb shell pidof -s com.example.app`
or

adb logcat --pid=$(adb shell pidof -s com.example.app)

