# XXE 

### What is XML external entity injection?

![](xxe-injection.svg)

XML external entity injection (also known as XXE) is a web security vulnerability that allows an attacker to interfere with an application's processing of XML data. It often allows an attacker to view files on the application server filesystem, and to interact with any back-end or external systems that the application itself can access.

In some situations, an attacker can escalate an XXE attack to compromise the underlying server or other back-end infrastructure, by leveraging the XXE vulnerability to perform [server-side request forgery](.././SSRF) attacks.
[Read more](https://portswigger.net/web-security/xxe) 

<details>
	<summary>CTF-Writeups</summary>

### CTF Writeups

- [2017](#2017)

- [2018](#2018)

- [2019](#2019)

- [2020](#2020)

- [2021](#2021)

- [read-more](#other-interesting-reads)


#### 2017

- [Aaditya : upl0ad3r,inCTF](https://aadityapurani.com/2017/12/17/inctf/)

- [qiita : xmlvalidator,HamaCTF](https://qiita.com/no1zy_sec/items/03b8f335e84995fec3e3)


#### 2018

- [vladtoie: message-board,pwn2win](https://medium.com/@vladtoie/message-board-first-flag-pwn2win-ctf-2018-writeup-5627ae5daed4)

- [honoki : From blind XXE to root-level file read access](https://honoki.net/2018/12/12/from-blind-xxe-to-root-level-file-read-access/)

- [Balsn : Berg’s Club,Pwn2win ](https://balsn.tw/ctf_writeup/20181130-pwn2winctf/#berg%E2%80%99s-club)

- [Thibaud : santahacklaus](https://thibaud-robin.fr/writeups/santhacklaus-2018/archdrive/)

- [nettitude : derbycon ](https://labs.nettitude.com/blog/derbycon-2018-ctf-write-up/)

- [Dvd848 : blind, 35C3](https://github.com/Dvd848/CTFs/blob/4f288117c2261b73e125f2338931c86a3641de1c/2018_35C3_Junior/blind.md)

#### 2019

- [pointhi : Baby Recruitor,Pwn2Win](https://www.sigflag.at/blog/2019/writeup-pwn2win-baby-recruiter/)

- [ctrsec : BNV,Google CTF ](https://ctrsec.io/wp-content/uploads/2019/06/Google-CTF-2019-Writeups-Web-BNV.pdf)

- [Bushwhackers : Gphotos,Google CTF](https://blog.bushwhackers.ru/googlectf-2019-gphotos-writeup/)

- [w0u : Household,RuCTFE](https://w0y.at/writeup/2019/11/23/ructfe-2019-household.html)

- [rawsec : Securinets Quals](https://rawsec.ml/en/SecurinetsCTF-2019-Quals-write-up/)

- [rawsec : Wrestler Name Generator, SunshineCTF](https://rawsec.ml/en/Sunshine-CTF-2019-write-ups/)

- [jaime : Wrestler Name Generator, SunshineCTF](https://jaimelightfoot.com/blog/sunshinectf/)

- [m09ic : Ogeek CTF Quals](https://m09ic.top/posts/45148/)

- [bookgin : Defcon27 Quals](https://bookgin.tw/2019/05/17/defcon-27-qual-ctf-web-writeups/)

- [noistar : Juice Shop](https://noirstar.tistory.com/232)

- [midnight : j2x2j,TokyoWesterns](https://syn-ack.hatenablog.com/entry/2019/09/05/104038)

- [st98 :j2x2j,TokyoWesterns](https://st98.github.io/diary/posts/2019-09-14-tokyowesterns-ctf-5th-2019.html#j2x2j-web-59)

- [Dead && end : ncc2019](https://d3adend.org/blog/posts/cloudiot-write-ups/)

- [alevsk : bad injections.fireshell](https://www.alevsk.com/2019/01/fireshell-ctf-2019-bad-injections-web/)

- [anemone : fireshell](https://anemone.top/ctf-2019fireshell%E4%B8%80%E9%81%93%E4%BB%8Exxe%E5%88%B0ssrf%E9%A2%98/)

- [secpulse : OGeekCTF ](https://www.secpulse.com/archives/111370.html)

- [s1r1us : Unagi,CSAW ](https://www.s1r1us.ninja/2019/09/csaw-ctf19-quals-writeup.html)

- [zhaoj : ByteCTF](https://www.zhaoj.in/read-6310.html)


#### 2020 

- [asd007: XXExternalXX,SharkyCTF](https://ctftime.org/writeup/20569)

- [jai : XXExternalXX,SharkyCTF](https://jaiguptanick.github.io/Blog/blog/SharkyCTF_Writeup_web/)

- [szymanski : ratctf](https://szymanski.ninja/en/ctfwriteups/2020/ratctf2020/)

- [sqrtrev : wwww,3k](https://wrecktheline.com/writeups/3kctf-2020/)

- [jaiguptanick : Traffic Lights W,HSCTF](https://jaiguptanick.github.io/Blog/blog/HSCTF7_2020_Writeups/)

- [Bigpick : ExtraTerestrial,Nahamcon](https://bigpick.github.io/TodayILearned/articles/2020-06/nahamConCTF-writeups)

- [ptr-yudai : A payload to rule them all,Pwn2win](https://ptr-yudai.hatenablog.com/entry/2020/06/01/102049)

- [progpilot :spooky store,UTCTF](https://www.progpilot.com/writeups/nc2020/spook/)

- [st98 : JACC](https://st98.github.io/diary/posts/2020-04-13-hexion-ctf-2020-online.html)

- [hamayan : File Reader,DarkCTF](https://www.hamayanhamayan.com/entry/2020/09/28/233549)

- [bootplug :Syntax check,defcamp](https://github.com/bootplug/writeups/blob/master/2020/defcamp/writeups.md#syntax-check)

### 2021 

- [SamXML : Special order 2, 0x41414141](https://github.com/sambrow/ctf-writeups-2021/tree/master/0x41414141/special-order-pt2)

- [Letronghoangminh : Alex Fan Club,LITCTF](https://github.com/letronghoangminh/CTF-Writeups/tree/master/Web/LITCTF%202021%20-%20Alex%20Fan%20Club%20API%20(500))

- [Synacktiv : entituber, HTB-Business](https://github.com/synacktiv/CTF-Write-ups/blob/main/HTB-Business-CTF-2021/fullpwn/entituber.md)

- [Greybtw : Include me, eHaCON](https://github.com/greybtw/writeup-CTF_2021/blob/master/eHaCON%20CTF%202K21/Include%20me.md)

- [Thalium : Artillery, CyberApocalypse](https://thalium.github.io/blog/posts/apocalypse2021-artillery/)

- [Szymanski : indead2, Hackpack](https://szymanski.ninja/en/ctfwriteups/2021/hackpack/indead-v2/)

- [PwnProphecy : Leaky-logs, Cybergames](https://github.com/PwnProphecy/ctf/blob/main/metactf-cybergames2021/Leaky-Logs.md)

- [Terawiz : special-order-pt2, 0x41414141](https://github.com/terawhiz/CTF-Writeups/blob/main/0x41414141-CTF/web/special-oreder-pt2/README.md#special-order-pt2---490-pts)

</details>


<details>
	<summary>other interesting reads</summary>

### other interesting reads

- [Intigriti : XXE](https://blog.intigriti.com/hackademy/xml-external-entity-processing-xxe/)

- [mohemiv : exploiting xxe with local dtd files](https://mohemiv.com/all/exploiting-xxe-with-local-dtd-files/)

- [hacktricks : XXE ](https://book.hacktricks.xyz/pentesting-web/xxe-xee-xml-external-entity)

- [tohacking : basic ways to exploit xxe](https://tohacking.com/til/the-basic-ways-to-exploit-xxe/)

- [acunetix : OOB-XXE](https://www.acunetix.com/blog/articles/band-xml-external-entity-oob-xxe/)

- [wallarm : XXE that Can bypass waf](https://lab.wallarm.com/xxe-that-can-bypass-waf-protection-98f679452ce0/)

- [r00thunt : blind OOB-XXE ](https://r00thunt.com/2018/10/05/blind-xml-external-entities-out-of-band-channel-vulnerability-paypal-case-study/)

- [XXE Wiki](https://csea-iitb.github.io/IITBreachers-wiki/2020/07/22/XXE.html)

</details>
