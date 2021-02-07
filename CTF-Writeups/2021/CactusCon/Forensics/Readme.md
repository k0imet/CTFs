#The Sleuth Fairy
###### tags: `ctf` `cactuscon` `forensics` 
### solves 11
### Challenge Description
I accidentally deleted an important file. I have attached the disk image. Can you recover the deleted file `fragments` for me?

<a href="https://drive.google.com/file/d/1HLK47KOuw4Ki3puPraupbU-gOsZBsijn/view?usp=sharing">File</a>

### Solution 
for this solution i used The Sleuth Kit, and specifically the tool tsk_recover
this was recommended by a teammate,
thats after foremost and binwalk failed me ...
...
```tsk_recover -i raw -e image.dd .```
using the above command on challenge file we got 7 recovered files...
but no flag yet ... 
![](files.png)

but wait we can see `_rag1.dat, _rag2.dat` fragmented chunks as per the challenge description 
and we all get a third one `frag3.dat` from _ir1,dir2_ folders ... 
 
a close look at `_rag1.dat` reveals it to be a corrupt jpeg image
....
strings confirms it 
```
$strings _rag1.dat 
JFIF
(ICC_PROFILE
mntrRGB XYZ 
acsp
	desc
trXYZ
gXYZ
```

the 3 fragmnents together will reveal the flag ... 

```
base64 < _rag1.dat > frag1.txt
base64 < _rag2.dat > frag2.txt
base64 < frag3.dat > frag3.txt
```

appending all the txt files together and decoding recovers the image with the flag 
`cat frag.txt frag2.txt frag3.txt > final.txt`

`cat final.txt | base64 -d > flag.jpg`

recovers the image plus a visible flag
![](flag.jpg)

> flag : {santiano_the_drunk_punching_bag}
 