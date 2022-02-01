#### Crackme 1

We found this password hash, can you somehow crack it? The hash is also available in the file hash1.txt via he web based terminal.  
87dfc97a7654b4b7ad9f04767361eca9  
Hint: Use the john the ripper tool using the rockyou.txt wordlist

Flag: cartoonnetwork

#### Crackme 2

We heard they added some sort of salt now. The hash is also available in the file hash2.txt via he web based terminal.  
$2a$04$R3woFi8JQxib7WYkzCeLFeSk2Kbuq3qcddLKGZi4te1TluMX2y/cm  
Hint: Use the john the ripper tool using the rockyou.txt wordlist

john hash2.txt --wordlist=rockyou.txt

Flag: patience