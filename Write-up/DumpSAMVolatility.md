
Dumps passwords hashes (LM/NTLM) from memory

```sh
$ python vol.py -f ~/memdump/infected.img hivelist
Volatile Systems Volatility Framework 2.2
Virtual    Physical   Name
---------- ---------- ----
0xe2084008 0x0fe6b008 \Device\HarddiskVolume1\Documents and Settings\pilou\Local Settings\Application Data\Microsoft\Windows\UsrClass.dat
0xe1d1fb60 0x0db99b60 \Device\HarddiskVolume1\Documents and Settings\pilou\NTUSER.DAT
0xe19d8380 0x0d091380 \Device\HarddiskVolume1\Documents and Settings\LocalService\Local Settings\Application Data\Microsoft\Windows\UsrClass.dat
0xe1c19508 0x0d644508 \Device\HarddiskVolume1\Documents and Settings\LocalService\NTUSER.DAT
0xe17206d0 0x0cad76d0 \Device\HarddiskVolume1\Documents and Settings\NetworkService\Local Settings\Application Data\Microsoft\Windows\UsrClass.dat
0xe19fb008 0x0d403008 \Device\HarddiskVolume1\Documents and Settings\NetworkService\NTUSER.DAT
0xe196c6b8 0x0a9ca6b8 \Device\HarddiskVolume1\WINDOWS\system32\config\software
0xe1599b60 0x04870b60 \Device\HarddiskVolume1\WINDOWS\system32\config\default
0xe196cb60 0x0a9cab60 \Device\HarddiskVolume1\WINDOWS\system32\config\SECURITY
0xe195eb60 0x0a6e2b60 \Device\HarddiskVolume1\WINDOWS\system32\config\SAM
0xe134f350 0x02f00350 [no name]
0xe1035b60 0x02aa3b60 \Device\HarddiskVolume1\WINDOWS\system32\config\system
0xe102e008 0x02a9d008 [no name]
0x806717a8 0x006717a8 [no name]
```
Then dump the hashes as follows:

```sh
$ python vol.py -f ~/memdump/infected.img hashdump -s 0xe195eb60 -y 0xe1035b60
Volatile Systems Volatility Framework 2.2
Administrateur:500:e039e3178e07d0c9a6e1e67c15d6275b:b246b548b6f17e45f349aa2214a5f6aa:::
```

You can then use online resources to crack the hash.
