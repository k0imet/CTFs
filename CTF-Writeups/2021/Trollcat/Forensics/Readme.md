# Forbidden

### points 100

###### tags : `trollcat` `ctf` `forensics` `steg` 

### challenge description

Agent Troll recieved some file but not able to read the data can you help us?

Author: White_Wolf
<a href="https://ctf.cscodershub.tech/files/c46ffc7ac0a5a27387b4a35f04671302/trollcats.car?token=eyJ1c2VyX2lkIjo1MzQsInRlYW1faWQiOjIwNCwiZmlsZV9pZCI6Mzh9.YB_E5g.YXCbkcpWJzJFP-paREvdycYRN0k">Forbidden</a> (link is dead but file is attached)

### solution

we are given a `trollcats.car` 

```
$file trollcats.car 
trollcats.car: data
```

on further investigation 

```
$binwalk trollcats.car 

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
50            0x32            bzip2 compressed data, block size = 900k

```


extracting the file 

```
$binwalk -e trollcats.car 

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
50            0x32            bzip2 compressed data, block size = 900k

┌─[@parrot]─[~/Desktop/CTFs/TrollCAT/Forensics]
└──╼ $cd _trollcats.car.extracted/
┌─[skoki@parrot]─[~/Desktop/CTFs/TrollCAT/Forensics/_trollcats.car.extracted]
└──╼ $ls
32
┌─[@parrot]─[~/Desktop/CTFs/TrollCAT/Forensics/_trollcats.car.extracted]
└──╼ $cat 32 
Trollcat{M0zilla_Archive_maaaarls}
```
> flag : Trollcat{M0zilla_Archive_maaaarls}




# the_sus_agent

### points 251

### challenge description
One of our agent is doing something suspicious on the network can you find out?

file Hint: If you got a string it's useful somewhere but it's not a flag

Author : white_wolf
<a href="https://mega.nz/file/DxUmUToR#ckGf6JffCW2M7TixQzcfQNx9Ki-66gXyNSA4lUX5Ooc">Mega link</a>

### solution

we are given a `sus_agent.pcapng`

opening the pcap in wireshark 
> file > export objects > http > save all 

gives us a bunch of files but two are important in this case
`secret.jpg` and `welcome.jpg`

secret.jpg contains a base64 string 
```
$cat secret.jpg 

aWhvcGV5b3VkaWRub3R0cmllZHRvYnJ1dGVmb3JjZWl0
```

decoded to 

```
$cat secret.jpg | base64 -d
ihopeyoudidnottriedtobruteforceit
```

which was the steghide password for `welcome.jpg`

![](welcome.jpg)

```
[@parrot]─[~/Desktop/CTFs/TrollCAT/sus]
└──╼ $steghide extract -sf welcome.jpg
Enter passphrase: 
the file "foryou" does already exist. overwrite ? (y/n) y
wrote extracted data to "foryou".
┌─[@parrot]─[~/Desktop/CTFs/TrollCAT/sus]
└──╼ $cat foryou 
Trollcat{this_challenge_was_easy_right???}
```

> flag : Trollcat{this_challenge_was_easy_right???}

# s3cr3t

### points 495

### challenge description

After getting trolled alot by Mr.Troll we finally got some files and now he's hiding some secret with him your mission is to find that secret.

<a href="https://mega.nz/file/PtsFHYzY#tKDykxlC1Uj5FniYU947AMRFJubc8OL11l0jmMbxmbA">Challenge file link</a>

Author: White_Wolf

<b>NB://I did not solve this challenge on time</b>


### solution

we are given a file `trollcat.E01` of type

```
$file trollcat.E01
trollcat.E01: EWF/Expert Witness/EnCase image file format
```
using binwalk and other file carving tools will not be effective in this case
so i decided to mount the image 

```
sudo mkdir rawimage
sudo mkdir mountpoint

ewfmount file trollcat.E01 rawimage/

mount rawimage/ewf1 mountpoint/ -o ro,loop,show_sys_files,streams_interface=windows
```

the drive is now accesible and we can navigate through it 
we get a `topsecret.zip`
under 
`favorites/drive`

which contains an encrypted vhdx `topsecret.vhdx`
the following writeup was quite useful 
<a href="https://stuxnet999.github.io/2021/02/06/trollcat-secret.html">https://stuxnet999.github.io/2021/02/06/trollcat-secret.html</a> 

# Mr_evilpepo_1


### points 400

We have caught Mr.EvilPepo and now it is time for you to investigate him we searched his house and we got not much proof we got some report from OSINT department and Our OSINT Investigator told us that he mentioned on his socials "Hack Me if you can, i use same password Everywhere" we have dumped his computer memory and for further investigation we need your help. he typed the flag command somewhere and now he forgot it. can you find it?

File: https://mega.nz/file/y90gWRJa#6lJ4qpKw3bfLKvbcTuvcOgGdDpYS9AapC_mwKM-4Zg4

Flag Format: Trolcat{}

Author: White_wolf


### solution

in this we get a memory dump file `evilpepo.vmem` 

from the hint : `he typed the flag command somewhere and now he forgot it`
we will use `cmdscan` plugin to recover the flag 

```
─[@parrot]─[~/Desktop/CTFs/TrollCAT/forensics]
└──╼ $volatility -f evilpepo.vmem --profile=Win7SP1x64 cmdscan
Volatility Foundation Volatility Framework 2.6
**************************************************
CommandProcess: conhost.exe Pid: 992
CommandHistory: 0x39eb60 Application: cmd.exe Flags: Allocated, Reset
CommandCount: 37 LastAdded: 36 LastDisplayed: 36
FirstCommand: 0 CommandCountMax: 50
ProcessHandle: 0x60
Cmd #0 @ 0x37e550: helo
Cmd #1 @ 0x37e570: troollll
Cmd #2 @ 0x37e590: caaat
Cmd #3 @ 0x37e5b0: yooooo
Cmd #4 @ 0x39de90: T
Cmd #5 @ 0x39dcd0: r
Cmd #6 @ 0x3a2f00: o
Cmd #7 @ 0x3a2f20: l
Cmd #8 @ 0x3a2f40: c
Cmd #9 @ 0x3a2f60: a
Cmd #10 @ 0x3a2fb0: t
Cmd #11 @ 0x3a2fc0: {
Cmd #12 @ 0x3a2fd0: c
Cmd #13 @ 0x3a2fe0: o
Cmd #14 @ 0x3a2ff0: m
Cmd #15 @ 0x3a3000: a
Cmd #16 @ 0x3a3010: n
Cmd #17 @ 0x3a3020: d
Cmd #18 @ 0x3a3030: s
Cmd #19 @ 0x3a3040: _
Cmd #20 @ 0x3a3050: 4
Cmd #21 @ 0x3a3060: r
Cmd #22 @ 0x3a3070: 3
Cmd #23 @ 0x3a3080: _
Cmd #24 @ 0x3a3090: i
Cmd #25 @ 0x3a30a0: m
Cmd #26 @ 0x3a30b0: p
Cmd #27 @ 0x3a30c0: o
Cmd #28 @ 0x3a30d0: r
Cmd #29 @ 0x3a30e0: t
Cmd #30 @ 0x3a30f0: a
Cmd #31 @ 0x3a3100: n
Cmd #32 @ 0x3a3110: t
Cmd #33 @ 0x3a3120: }
Cmd #34 @ 0x3a33b0: hope you got it 
Cmd #35 @ 0x377860: "are you trying to run strings?"
Cmd #36 @ 0x3a33e0: lolololololol
```

> flag : Trolcat{commands_4r3_important}


# Mr_evilpepo_2


### points 496


### challenge description


Now After some good beating, Mr.EvilPepo saying he hides something on the internet. find it

Note: Use the file provided in Mr.EvilPepo Part-1

AUTHOR: WHITE_WOLF

### solution

same file as above for this challenge
from the hint `...he hides something on the internet. find it`
we need to check through some browswer history 

```
┌─[skoki@parrot]─[~/Desktop/CTFs/TrollCAT/forensics]
└──╼ $volatility -f evilpepo.vmem --profile=Win7SP1x64 pstree 
Volatility Foundation Volatility Framework 2.6
Name                                                  Pid   PPid   Thds   Hnds Time
-------------------------------------------------- ------ ------ ------ ------ ----
 0xfffffa8000ca0ae0:System                              4      0     78    506 2021-01-12 13:13:38 UTC+0000
. 0xfffffa8001bf6470:smss.exe                         256      4      2     29 2021-01-12 13:13:38 UTC+0000
 0xfffffa80028a7630:csrss.exe                         388    368     11    338 2021-01-12 13:13:53 UTC+0000
. 0xfffffa8000f0d060:conhost.exe                      992    388      2     51 2021-01-12 13:20:09 UTC+0000
 0xfffffa80028f9480:winlogon.exe                      420    368      3    109 2021-01-12 13:13:53 UTC+0000
 0xfffffa800344fb30:explorer.exe                     1568   1548     32    895 2021-01-12 13:14:47 UTC+0000
. 0xfffffa80020de060:notepad.exe                     3120   1568      1     61 2021-01-12 13:22:27 UTC+0000
. 0xfffffa8003428a30:cmd.exe                         1492   1568      1     19 2021-01-12 13:20:08 UTC+0000
. 0xfffffa8003673b30:chrome.exe                      1932   1568     34    856 2021-01-12 13:15:05 UTC+0000
.. 0xfffffa80036d6b30:chrome.exe                      912   1932      8     84 2021-01-12 13:15:12 UTC+0000
.. 0xfffffa8000ee9b30:chrome.exe                     1292   1932     13    204 2021-01-12 13:16:11 UTC+0000
.. 0xfffffa8000e9ab30:chrome.exe                     2324   1932     13    255 2021-01-12 13:16:05 UTC+0000
.. 0xfffffa8000da1b30:chrome.exe                     2352   1932     20    248 2021-01-12 13:15:37 UTC+0000
.. 0xfffffa8000e5cb30:chrome.exe                     2896   1932      8    181 2021-01-12 13:15:54 UTC+0000
.. 0xfffffa8000d97b30:chrome.exe                     2556   1932      7    131 2021-01-12 13:15:38 UTC+0000
. 0xfffffa8000fc0060:KeePass.exe                     3908   1568     12    324 2021-01-12 13:18:05 UTC+0000
 0xfffffa80028ba060:csrss.exe                         328    320      8    405 2021-01-12 13:13:52 UTC+0000
 0xfffffa80027ddb30:wininit.exe                       376    320      3     74 2021-01-12 13:13:53 UTC+0000
. 0xfffffa8002da0b30:services.exe                     472    376     11    192 2021-01-12 13:13:59 UTC+0000
.. 0xfffffa8003180890:svchost.exe                     268    472     19    484 2021-01-12 13:14:12 UTC+0000
.. 0xfffffa8002fab440:svchost.exe                     668    472      8    261 2021-01-12 13:14:06 UTC+0000
.. 0xfffffa800142db30:sppsvc.exe                     1456    472      4    142 2021-01-12 13:16:56 UTC+0000
.. 0xfffffa8003236610:svchost.exe                    4016    472     16    344 2021-01-12 13:18:10 UTC+0000
.. 0xfffffa80030d5b30:svchost.exe                     808    472     16    311 2021-01-12 13:14:06 UTC+0000
... 0xfffffa8003441b30:dwm.exe                       1556    808      3     80 2021-01-12 13:14:47 UTC+0000
.. 0xfffffa8003146b30:svchost.exe                     968    472     29    448 2021-01-12 13:14:11 UTC+0000
.. 0xfffffa8003229570:svchost.exe                     948    472     21    332 2021-01-12 13:14:18 UTC+0000
.. 0xfffffa80032145c0:spoolsv.exe                     832    472     13    265 2021-01-12 13:14:17 UTC+0000
.. 0xfffffa80030d3b30:svchost.exe                     836    472     41   1162 2021-01-12 13:14:06 UTC+0000
.. 0xfffffa8003091370:svchost.exe                     716    472     26    521 2021-01-12 13:14:06 UTC+0000
... 0xfffffa8003116060:audiodg.exe                    916    716      6    131 2021-01-12 13:14:09 UTC+0000
.. 0xfffffa800347b890:taskhost.exe                   1748    472      8    142 2021-01-12 13:14:48 UTC+0000
.. 0xfffffa8002feb970:svchost.exe                     600    472     10    348 2021-01-12 13:14:05 UTC+0000
... 0xfffffa8000ff1060:dllhost.exe                   2920    600      9    198 2021-01-12 13:19:42 UTC+0000
... 0xfffffa8000ea3060:dllhost.exe                   1852    600      6     89 2021-01-12 13:22:36 UTC+0000
... 0xfffffa8000dc3b30:WmiPrvSE.exe                  3400    600      7    114 2021-01-12 13:19:14 UTC+0000
.. 0xfffffa80023e2060:svchost.exe                     784    472     25    264 2021-01-12 13:15:13 UTC+0000
.. 0xfffffa800183f650:wmpnetwk.exe                   1640    472     11    218 2021-01-12 13:15:01 UTC+0000
.. 0xfffffa80032173b0:SearchIndexer.                 1832    472     12    702 2021-01-12 13:15:00 UTC+0000
... 0xfffffa8003696b30:SearchProtocol                1960   1832      8    387 2021-01-12 13:15:05 UTC+0000
... 0xfffffa8000d9bb30:SearchFilterHo                1504   1832      6    150 2021-01-12 13:20:40 UTC+0000
. 0xfffffa8002811b30:lsass.exe                        480    376      7    553 2021-01-12 13:13:59 UTC+0000
. 0xfffffa80020b7b30:lsm.exe                          488    376     10    149 2021-01-12 13:13:59 UTC+0000
```
we can see two browsers in use 
`explorer` and `chrome`

volatility lacks an inbuilt plugin for firefox and chrome so we will use a third party for the same 

>guide and plugins

<a href="https://blog.superponible.com/2014/08/31/volatility-plugin-chrome-history/">https://blog.superponible.com/2014/08/31/volatility-plugin-chrome-history/</a>

<a href="https://github.com/superponible/volatility-plugins">https://github.com/superponible/volatility-plugins</a>


```
volatility --plugins=volatility-pluginss/ -f evilpepo.vmem --profile=Win7SP1x64  chromehistory
Volatility Foundation Volatility Framework 2.6
Index  URL
https://defuse.ca/b/sOOqp4UunTdD0oUjidJFlz                                       Defuse Security's Encrypted Pastebin                                                  2     1 2021-01-12 08:23:00.706346        N/A       
```
> snipped for readability

following the links gives us an encrypted pastebin which needs a password to reveal the flag 
.....
![](pastebin.png)

> flag : Trollcat{secret_hidden_0nn_th3_1ntern3t}

looking back at the `pstree` results we can see  `lsass.exe`

<a href="https://en.wikipedia.org/wiki/Local_Security_Authority_Subsystem_Service">Local Security Authority Subsystem Service (LSASS) is a process in Microsoft Windows operating systems that is responsible for enforcing the security policy on the system. It verifies users logging on to a Windows computer or server, handles password changes, and creates access tokens</a>

for this i will use the `hashdump` plugin to recover NTLM hashes for all users

```
┌─[✗]─[@parrot]─[~/Desktop/CTFs/TrollCAT/forensics]
└──╼ $volatility -f evilpepo.vmem --profile=Win7SP1x64  hashdump
Volatility Foundation Volatility Framework 2.6
Administrator:500:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
Guest:501:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
WhiteWolf:1000:aad3b435b51404eeaad3b435b51404ee:2e6a7cf5aabb33a044684dd9c97e88a7:::
```

user WhiteWolf since he was the author

```
echo "2e6a7cf5aabb33a044684dd9c97e88a7"
hashcat -m 1000 /usr/share/wordlists/rockyou.txt --force
```
cracking the NTLM hash for user `WhiteWolf` reveals the password as `abracadabra`
using the password we can now decrypt our encrypted pastebin to reveal the flag 

alternatively you can use mimikatz plugin 

<a href="https://medium.com/@ali.bawazeeer/using-mimikatz-to-get-cleartext-password-from-offline-memory-dump-76ed09fd3330">https://medium.com/@ali.bawazeeer/using-mimikatz-to-get-cleartext-password-from-offline-memory-dump-76ed09fd3330</a>


# Mr_evilpepo_3


### points 498

### challenge description


The Top Secret file of Mr.EvilPepo is still not discovered this is your last mission of finding the top secret file related to Mr.EvilPepo Good Luck

Note: Use the file provided in Mr.EvilPepo Part-1

AUTHOR: WHITE_WOLF

_i did not solve this challenge on time,_

i do recommend reading the following writeup

<a href="https://stuxnet999.github.io/2021/02/06/trollcat-mrevilpepo.html">https://stuxnet999.github.io/2021/02/06/trollcat-mrevilpepo.html</a>


.....
Thank you for your time,hope you learnt something new :)

