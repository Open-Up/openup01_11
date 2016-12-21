# Practical work : Hashing and encryption

## GPG 

1/ Create a couple of private/public key

2/ Exchange your public key with your neightbour

3/ Send him a signed text

4/ verify the signature sent by your neightbour

5/ Send him an encrypted text

6/ Read the encrypted text sent by your neightbour

7/ Sign your neughtbour key

Symetric signatures : 

8/ Exchange an encrypted, symetrically encrypted text. What are the trade off between asymetric / symetric ancryptions ? Can you demonstrate it with the time command ?

9/ Revoke your key

## Hashing

0/ Create a SHA-1 hash for the file toto.txt with the content you like

1/ Give the file and the SH1-1 to your neightbour

2/ Was the text file corrupted during transfer ?

## Scripting (easy)

0/ Automating signing and hashing

As part of my work on the Apache foundation I must often upload a binary file, its MD5 and SHA-1 signature, as well as all signatures. 

I want a script, taking as a parameter the file to validate. I want a variable in it I can set to the key I am using.

The script will then ask me my passphrase for the key.

It will generate hashes for the file (MD5 and SHA-1) then sign the file, the MD5 sum, the SHA-1 sum

1/ Create a script for automatically verifying information specified above (signatures and hash sums).

## Automation (middle)

I have a sensitive service running on my computer.

To modelize it, run every minute the command 'echo "Very private information" >> /var/log/sensitive.log'

You should, on log rotation, compress then encrypt the target file.

Run manually logrotate to demonstrate your configuration.

## Scripting : correcting the scripting contest
