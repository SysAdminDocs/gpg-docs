gpg-docs
========

## General

### Import Local GPG Public Key

```shell
$ gpg --import ~/keys/pub/tom.asc
```

### Editing Trust Levels

You can change the trust level of a private/public key very easily using the following.

```shell
$ gpg --edit-key <Key_ID> trust
```

At the prompt select a number between 1...5 depending on your level of trust of the key.

## Encryption

## Decryption

### Automate/Batch Decrypt File

GPG _should_ automatically find the correct secret key, however one __can__ be defined if required.

```shell
$ gpg --batch --yes --passphrase "SecretSquirrel" -o ~/outputs/encryptedFile.txt -d ~/encrypted/encryptedFile.txt.gpg
```
