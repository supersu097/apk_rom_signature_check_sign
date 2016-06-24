## apk_rom_signature_check_sign
Feature:  
1. show and check android apk and rom's signature  
2. sign random apk and rom  

```
USAGE:
./dersa OPTION FILENAME
./dersa OPTION(-s) KEYPAIR_NAME
./dersa OPTION(-c) PUBLIC_KEY_DIR FILENAME

OPTION:
-h|--help         : display this help and exit
-w|--whole        : Show whole public key info
-p|--part         : Show part public key info of apk or zip file
-s|--sign         : Sign any .apk or .zip file
-c|--check        : check any .apk or .zip file whether it matches the keypair which the user assigned.
-m|--make         : Invoke AOSP's script to creat four key pairs

EXAMPLES:
./dersa -w ~/Download/dialer.apk
./dersa -p ~/Download/dialer.apk
./dersa -s ~/Download/media ~/Download/dialer.apk
./dersa -c ~/Download/certkey/ ~/Download/dialer.apk
```
