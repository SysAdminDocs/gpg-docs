gpg-docs
========

##Encryption

##Decryption

###Automate/Batch Decrypt File

GPG _should_ automatically find the correct secret key, however one __can__ be defined if required.

```shell
$ gpg --batch --yes --passphrase "SecretSquirrel" -o ~/outputs/encryptedFile.txt -d ~/encrypted/encryptedFile.txt.gpg
```
