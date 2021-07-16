# XSS

![](xss.png)


## Cross-site Scripting (XSS)

`Cross-site Scripting (XSS) is a client-side code injection attack. The attacker aims to execute malicious scripts in a web browser of the victim by including malicious code in a legitimate web page or web application. The actual attack occurs when the victim visits the web page or web application that executes the malicious code. The web page or web application becomes a vehicle to deliver the malicious script to the user’s browser. Vulnerable vehicles that are commonly used for Cross-site Scripting attacks are forums, message boards, and web pages that allow comments.`
`A web page or web application is vulnerable to XSS if it uses unsanitized user input in the output that it generates. This user input must then be parsed by the victim’s browser. XSS attacks are possible in VBScript, ActiveX, Flash, and even CSS. However, they are most common in JavaScript, primarily because JavaScript is fundamental to most browsing experiences.`

[Read more](https://www.acunetix.com/websitesecurity/cross-site-scripting/)

<details>
	<summary>CTF-Writeups</summary>

## CTF-Writeups 


- [2014](#2014)


- [2015](#2015)


- [2016](#2016)


- [2017](#2017)


- [2018](#2018)


- [2019](#2019)


- [2020](#2020)


- [2021](#2021)


### 2014 

- [tasteless : Page Builder,31C3](https://www.tasteless.eu/post/2014/12/31c3-ctf-page-builder-writeup/)

### 2015 

- [NorthSec](http://holyvier.blogspot.com/2015/05/northsec-xss-challenge-writeups.html)

### 2016

- [ulimateshi : XSS 2,ISITDTU](https://ctftime.org/writeup/3448)

- [Runesec : Charizard,Pentest Cyprus](https://blog.runesec.com/2016/10/10/charizard/)

- [gokulkrishna01 : sect-ctf](https://gokulkrishna01.wordpress.com/2016/09/09/admin-i-web-100-xss-sect-ctf-2016/)


### 2017

- [d90pwn : SimpleXss,0ctf Quals](https://ctftime.org/writeup/5956)


- [kyprizel : Complicated Xss,0ctf Quals](https://ctftime.org/writeup/5957)


- [dirty_vish : joe,GoogleCTF Quals](https://ctftime.org/writeup/6824)

- [l4w, The X sanitizer :Google CTF](https://l4w.io/2017/06/google-ctf-the-x-sanitizer-%E2%80%92-writeup/)


- [Pharisaeus : The Great Escape part-2, Insomni'hack](https://ctftime.org/writeup/5301)

- [chq-matteo : Mistune](https://theromanxpl0it.github.io/ctf_hacklu17/2017/10/19/mistune.html)

- [maniffin : LLC,Defcamp Quals](https://steemit.com/ctf/@maniffin/defcamp-ctf-quals-2017-llc-webchall-writeup)


### 2018 

- [EmpireCTF : Dot-free,Real World CTF quals](https://github.com/EmpireCTF/empirectf/blob/master/writeups/2018-07-28-Real-World-CTF-Quals/README.md#105-web--dot-free)

- [arminius : Nodepad,Teaser DragonCTF](https://ctftime.org/writeup/11452)

- [itsZN : bbs,Google Quals](https://ctftime.org/writeup/10369)

- [DragonSector : bbs,Google Quals](https://blog.dragonsector.pl/2018/07/google-ctf-2018-quals-bbs.html)

- [Askaholic : Excesss,Security Fest ](https://ctftime.org/writeup/10193)


- [kazkiti : rBlog 2018,RCTF](https://ctftime.org/writeup/10100)

- [kazkiti : idIoT: Action,PlaidCTF](https://ctftime.org/writeup/9987)

- [Orange : gCalc,Google CTF](https://blog.orange.tw/2018/06/google-ctf-2018-quals-web-gcalc.html)


- [LoRexxar : TCTF/OCTF Xss](https://blog.knownsec.com/2018/04/tctf0ctf2018-xss-writeup/)

- [TCTF/0CTF Quals](https://paper.seebug.org/574/)

- [i heard you like xss,PlaidCTF](https://dttw.tech/posts/r1wFutMCf)

### 2019 


- [terjanq : Do You Even XSS?,Hack.lu](https://gist.github.com/terjanq/fdb23ae109446b826a4b37df88efae07#file-xss_hard-js)

- [Alain_K : Numtonce,Hack.lu](https://ctftime.org/writeup/17065)

- [XeR : hCorem - Real World CTF 2019 Quals](https://ctftime.org/writeup/16642)

- [ajdumanhug : csaw-babycsp](https://github.com/ajdumanhug/ctf/blob/master/web/xss/csaw-babycsp-web-50.md)

- [bilith : P0stMan,KipodAfterFree](https://ctftime.org/writeup/17694)

- [jbz : Bypasses Everywhere,Ins'Hack](https://jbz.team/inshack2019/Bypasses_Everywhere)

- [hasp0t : Intigriti may challenge](https://0x00sec.org/t/intigriti-xss-challenge-solution/13896)

- [NaruseJun : TSG CTF](https://hackmd.io/@sekai/HJhnHwTiE?type=view)

- [L'Amore : My Cats, CONfidence 2019](https://www.gem-love.com/ctf/2019.html)

- [Renaud : Intigriti April XSS challenge](https://renaudmarti.net/posts/intigriti-xss-challenge/)

- [0xc0ffee : SecretNote Keeper,Facebook CTF](http://0xc0ffee.io/blog/FacebookCTF-SecretNote)

- [cybermouflons : nevernotecsp, csaw](https://cybermouflons.com/red-csaw19-nevernotecsp/)

### 2020

- [Kazkiti : MusicBlog,Zer0pts](https://ctftime.org/writeup/18604)

- [Sigflag : Notes App,ByteBandits](https://www.sigflag.at/blog/2020/writeup-bytebandits2020-notes-app/)

- [jmg-duarte : Chatt with Bratt,UTCTF](https://jmg-duarte.github.io/posts/ctfs/utctf/chatt/)


- [invalid-email-address : User Center,Volga Quals](https://github.com/corax/writeups/blob/master/VolgaCTF2020/Web/User%20Center/README.md)

- [m417z : StuckOverflow,AppSec-IL](https://ctftime.org/writeup/24403)

- [m3rc1fulcameron : flag-sharer,redpwn CTF](https://ctftime.org/writeup/21990)

- [zup : viper,redpwn](https://ctftime.org/writeup/21819)

- [Challenge writer POV: BSidesSF 2020 CTF](https://medium.com/@itsc0rg1/challenge-writer-pov-bsidessf-2020-ctf-ea84980b8d79)

- [p6 : CSP, codegate preliminary](https://blog.p6.is/codegate-ctf-2020-preliminary/)

- [p6 : Bsides SF](https://blog.p6.is/BSidesSF-2020-CTF/)

- [LiveOverFlow : Pasteurize,Google CTF](https://www.youtube.com/watch?v=Tw7ucd2lKBk)

- [LiveOverFlow : Tech Support,Google CTF](https://www.youtube.com/watch?v=Tw7ucd2lKBk)

- [0xparrot : PastaXSS,FwordCTF](https://github.com/parrot409/writeups/tree/master/Fword2020/pastaxss)

- [Nguyen : Intigriti Dec Xss challenge](https://viblo.asia/p/write-up-intigritis-december-xss-challenge-2020-GrLZDD0gZk0)

- [klefz : BugPoC November Xss Challenge](https://klefz.se/2020/11/10/bugpoc-xss-ctf-november-2020-write-up/)

- [Brett : Trash the Cache,Nahamcon](https://buer.haus/2020/06/14/nahamcon-trash-the-cache-write-up-web-1000/)

- [y4y : Static Pastebin,Redpwn](https://y4y.space/2020/06/27/redpwn-ctf-2020-web-pastebin-challenge-writeup/)

- [0x90AL : User Center,Volga Quals](https://blog.pwn.al/ctf/web/challenge/xss/jquery/2020/03/29/volgactf-web-challenge.html)

- [iboynton : Intigriti easter challenge](https://lboynton.com/2020/04/20/intigriti-easter-xss-challenge-2020-write-up/)

- [kitctf : Xmas Store,AllesCTF](https://kitctf.de/writeups/cscg20/xmas-store)

- [terjanq : Bfnote,TokyoWesterns](https://kitctf.de/writeups/cscg20/xmas-store)

### 2021 

- [tkaixiang : Babier CSP,DiceCTF](https://ctftime.org/writeup/25984)

- [terjanq : justCTF2020](https://hackmd.io/@terjanq/justCTF2020-writeups)

- [ptr-yudai :Carmen Sandiego Season 2,PlaidCTF ](https://ptr-yudai.hatenablog.com/entry/2021/04/19/140802)

- [k0imet : Support Ticket 2,CAT CTF](https://k0imet.github.io/2021/04/27/CAT-CTF.ae-WEB-Writeups.html)

- [k0imet : Bug report,CyberApocalypse 2021](https://k0imet.github.io/2021/04/26/CyberApocalypse-Writeups.html)

- [Ryn0K : Notes, RedPwn](https://github.com/Ryn0K/CTF_Writeups/tree/master/redpwn/web/notes/notes)

- [jokr: Notes, RedPwn](https://jokrhub.github.io/2021/06/13/redpwnCTF-2021-notes.html)

- [maple3142 : pastebin2, RedPwn](https://blog.maple3142.net/2021/07/13/redpwnctf-2021-writeups/#pastebin-2-social-edition)

- [maple3142 : pastebin3, RedPwn](https://blog.maple3142.net/2021/07/13/redpwnctf-2021-writeups/#pastebin-3)

- [Pocas : Original Store,Zh3r0](https://pocas.kr/2021/06/06/2021-06-05-Zh3r0-2021-CTF/#Web-Original-Store-842-pts)
	
- [Pocas : Original Store v2,Zh3r0](https://pocas.kr/2021/06/06/2021-06-05-Zh3r0-2021-CTF/#Web-Original-Store-v2-871-pts)
	
- [Pocas : bxss,Zh3r0](https://pocas.kr/2021/06/06/2021-06-05-Zh3r0-2021-CTF/#Web-bxss-100pts)
	
- [qxxxb : imgfiltrate,CCC](https://github.com/qxxxb/ctf_challenges/tree/master/2021/ccc/web/imgfiltrate/solve)
	
- [qxxxb : stickynotes, CCC](https://github.com/qxxxb/ctf_challenges/tree/master/2021/ccc/web/sticky_notes/solve)
	
</details>



<details>
	<summary>further-reading</summary>
	


## further-reading 

- [hacktricks : CSP Bypass](https://book.hacktricks.xyz/pentesting-web/content-security-policy-csp-bypass)

- [hackingarticles : comprehensive guide on Xss](https://www.hackingarticles.in/comprehensive-guide-on-cross-site-scripting-xss/)


- [xss for beginners](https://medium.com/swlh/xss-for-beginners-6752b1b1487d)

- [Guidance to Cross-Site Scripting for beginners- I: Reflected XSS](https://medium.com/infosec/guidance-to-cross-site-scripting-for-beginners-i-reflected-xss-591c950b87d7)

- [What is Cross-Site Scripting](https://chawdamrunal.medium.com/what-is-xss-c91d460375bb)

- [Learning XSS: Part 1 — Reflected XSS (Brief Concept, Techniques, Challenge Walkthrough)](https://medium.com/@onehackman/learning-xss-part-1-reflected-xss-brief-concept-techniques-challenge-walkthrough-85f6b165541b)

- [How to Detect Blind XSS Vulnerabilities](https://www.acunetix.com/websitesecurity/detecting-blind-xss-vulnerabilities/)

</details>
