# SQL Injections 

![](sql-injection.svg)


## Intro to SQLi 

```
SQL injection is a web security vulnerability that allows an attacker to interfere with the queries that an application makes to its database. It generally allows an attacker to view data that they are not normally able to retrieve. This might include data belonging to other users, or any other data that the application itself is able to access. In many cases, an attacker can modify or delete this data, causing persistent changes to the application's content or behavior.
```
[What is SQL injection](https://portswigger.net/web-security/sql-injection)

<details>
	<summary>CTF-Writeups</summary>

## CTF-Writeups

- [2013](#2013)


- [2014](#2014)


- [2015](#2015)


- [2016](#2016)


- [2017](#2017)


- [2018](#2018)


- [2019](#2019)


- [2020](#2020)


- [2021](#2021)


- [further-reading](#further-reading)

- [some labs](#some-labs)

### 2013

- [Reiners, Secuinside](https://websec.wordpress.com/2013/05/26/secuinside-ctf-2013-writeup-the-bank-robber/)


### 2014 

- [Dr0ptix : Web50,backdoorCTF 2014](https://ctftime.org/writeup/969)

- [ctf : injection3,PicoCTF](https://github.com/ctfs/write-ups-2014/tree/master/pico-ctf-2014/web-exploitation/injection-3-130)

- [skullsec : web 100,plaidCTF](https://blog.skullsecurity.org/2014/plaidctf-writeup-for-web-100-blind-sql-injection)

- [skullsec : web 100,PolygonShift](https://blog.skullsecurity.org/2014/plaidctf-writeup-for-web-100-blind-sql-injection)



### 2015 


- [insomihack: 2015writeups](https://insomnihack.ch/wp-content/uploads/2016/01/Hacking_like_in_the_movies.pdf)


- [hacklu 2015](https://en.internetwache.org/hacklu-ctf-2015-writeups-22-10-2015/)


- [orange : AIS3](https://blog.orange.tw/2015/09/ais3-final-ctf-web-writeup-race.html)

- [Brett : Web 500(weebdate)](https://buer.haus/2015/09/20/csaw-2015-web-500-weebdate-writeup/)



### 2016 

- [corb3nik : Homework,AliCTF](https://ctftime.org/writeup/3518)

- [0day : Good morning](https://0day.work/boston-key-party-ctf-2016-writeups/)

- [szurek : SharifCTF 7](https://security.szurek.pl/en/sharifctf-7-web-writeup/)

- [0daylabs](https://blog.0daylabs.com/2016/09/05/mongo-db-password-extraction-mmactf-100/)


### 2017 

- [HackThisSite : Injection2,EasyCTF](https://github.com/HackThisSite/CTF-Writeups/tree/master/2017/EasyCTF/Injection-2)

- [ymgve : Baby Sqli,Bctf](https://github.com/ymgve/ctf-writeups/tree/master/bctf2017/web-babysqli-kittyshop)

- [reznok : TetShopping,AceBear](https://github.com/reznok/CTFWriteUps/blob/master/AceBear_2018/TetShopping/README.md)

- [justcallmedude : Meetpwn 2017](https://babyphd.net/2017/07/meepwnctf-2017-br0kenmysql1-2-3/)


- [w0y : yacs,ucsb-ictf](https://w0y.at/writeup/2017/04/20/ucsb-ictf-2017-yacs.html)


- [inshall'hack : SqlSRF,SECCON](https://inshallhack.org/sqlsrf_seccon/)

- [hxp : Web150,hxp CTF 2017](https://hxp.io/blog/36/hxp-CTF-2017-web150-web_of_ages-writeup/)


- [Martin : SquareCTF 2017](https://martinmelhus.com/squarectf-2017-writeup)

- [securityinsider : nuit-du-hack](https://www.securityinsider-wavestone.com/2017/07/nuit-du-hack-2017-ctf-writeup--p1.html)


### 2018

- [kazkiti : RuAdmin,HackIT ](https://ctftime.org/writeup/11017)

- [arminius : Nodepad,Teaser Dragon CTF](https://ctftime.org/writeup/11452)

- [iodbh: the vault,picoctf](http://blog.iodbh.net/picoctf2018-web-the-vault.html)

- [argaz: Weird Blog,Jordan & Tunisia](https://ctftime.org/writeup/10374)

- [kazkiti : Old School,Bsides Delhi 2018](https://ctftime.org/writeup/11953)

- [iodbh :Irish name repo,PicoCTF](http://blog.iodbh.net/picoctf2018-web-irish-name-repo.html)

- [Aaditya : Event Registeration](https://ctftime.org/writeup/9712)

- [tonkatsu : Nodepad,Teaser Dragon ](https://blog.tonkatsu.info/ctf/2018/10/04/dsctf-2018-teaser.html)

- [mdeditor : PicoCTF 2018](https://www.mdeditor.tw/pl/2OL3)

- [Spyclub : InCTF-2018](https://spyclub.tech/2018/10/08/2018-10-08-inctf2018-web-challenge-writeup/)

### 2019 


- [Dvd848 : Irish-Name-Repo, picoCTF](https://github.com/Dvd848/CTFs/blob/4f288117c2261b73e125f2338931c86a3641de1c/2019_picoCTF/Irish-Name-Repo_2.md)

- [Dvd848 : 1337 Security, TamuCTF](https://github.com/Dvd848/CTFs/blob/4f288117c2261b73e125f2338931c86a3641de1c/2019_TAMUctf/1337_Secur1ty.md)

- [m3ssap0 : SQL Injected,Securinets Prequals](https://github.com/m3ssap0/CTF-Writeups/blob/master/Securinets%20Prequals%20CTF%202019/SQL%20Injected/README.md)

- [Dvd848 : Not Another SQLi Challenge, TamuCTF](https://github.com/Dvd848/CTFs/blob/4f288117c2261b73e125f2338931c86a3641de1c/2019_TAMUctf/Not_Another_SQLi_Challenge.md)

- [Xh4H : file magician,hxp 36c3](https://ctftime.org/writeup/17890)


- [kazkiti : Vault,EncryptCTF](https://ctftime.org/writeup/14337)


- [m3ssap0 : Execute-No-Evil,Xmas](https://github.com/m3ssap0/CTF-Writeups/blob/master/X-MAS%20CTF%202019/Execute%20No%20Evil/README.md)


- [h0ffayyy : SQL, TamuCTF](https://github.com/h0ffayyy/CTF/blob/master/TAMU_CTF_2019/SQL/writeup.md)


- [PDKT-Team: hr-admin,fbctf](https://github.com/PDKT-Team/ctf/blob/master/fbctf2019/hr-admin-module/README.md)


- [alejandro : Bird Box,TamuCTF](https://ctftime.org/writeup/13860)


- [viblo : efiens 2019](https://viblo.asia/p/efiens-ctf-2019-write-up-tu-sql-injection-toi-rce-va-get-root-oOVlYom4K8W)


- [W0y : Trees For Future,hack.lu](https://w0y.at/writeup/2019/10/28/hacklu-2019-trees-for-future.html)


- [Bookgin : Defcon 27 Quals ](https://bookgin.tw/2019/05/17/defcon-27-qual-ctf-web-writeups/)


- [Ines : NeverLAN](https://git.fh-campuswien.ac.at/CampusCyberSecurityTeam/ctfs/blob/e6a1fdadfb6832aadb0cb8b3ad4771c203e841eb/writeups/2019/neverlan2019.md)


- [graneed :  CryptixCTF](https://graneed.hatenablog.com/entry/2019/10/13/214515)


### 2020 

- [mrnoobot : Bobby,TGHack](https://mrnoobot.com/tg20-bobby-web-challenge-sql-injection-sqli/)


- [terjanq : Secure System,TetCTF](https://medium.com/@terjanq/blind-sql-injection-without-an-in-1e14ba1d4952)


- [ZSECURE : Data Store,CyberYoddha](https://github.com/CTSecUK/CyberYoddha-CTF-2020/blob/main/Write-ups/Data%20Store.md)


- [TwentyOneCool : Pandora, PragyanCTF](https://ctftime.org/writeup/18485)


- [Kahla : The after-Prequel,Securinets QUals](https://ctftime.org/writeup/19077)


- [Aneesh, File Magician,36C3](https://anee.me/file-magician-36c3-ctf-6cb5964c3238)


- [itzone : Efiens CTF](https://itzone.com.vn/vi/article/efiens-ctf-2019-write-up-tu-sql-injection-toi-rce-va-get-root/)


- [sqrtrev : ASIS CTF 2020 Write up(Author View)](https://vuln.live/blog/10)


- [bi0s : XQli,InCTF](https://blog.bi0s.in/2020/08/26/Web/InCTF20%20-%20XQLi/)


- [p1 : login page,UIUCTF](https://blog.p1.gs/ctf/2020/07/20/UIUCTF-2020-writeup/)


- [dreamhack : Dobby_is_free, 2020 christmas ctf](https://dreamhack.io/ctf/writeups/47)

- [SanXML :got-stacks ](https://drive.google.com/file/d/1hIcHVX3Pbv_EVpmbWUVctpBv7tsPJ_y5/view?usp=sharing)


## 2021

- [MrFrey : Cartooner,DCTF](https://mrfey.fr/CTFS//DragonSec%20SI%20CTF%20-%202021/Web/Cartooner)

- [y011d4 : Sea of Quills 1, angstrom](https://https://y011d4.netlify.app/20210408-angstromctf-writeup/#sea-of-quills)

- [y011d4 : Sea of Quills 1, angstrom](https://y011d4.netlify.app/20210408-angstromctf-writeup/#sea-of-quills-2)

- [sqrtrev : DarkCon Challs,VKL_SQL DarkCON](https://vuln.live/blog/12)

- [SamXML : mysqlimit, TetCTF](https://drive.google.com/file/d/1vZEsnFT37qzlsMkfFqaYioxUPepdEpVY/view)

- [qxxb : meet the union committee,UnionCTF](https://github.com/qxxxb/ctf/tree/master/2021/union_ctf/meet_the_union_committee)

- [pwnthenope : Gauntlet2&3, PicoCTF](https://pwnthenope.pythonanywhere.com/writeups/web_gauntlet.html)

- [th3jackers : Trashbin,Bsides Algiers Quals](https://ctftime.org/writeup/25437)
	
- [ianjelot : art-gallery2,shakti](https://thegoonies.github.io/2021/04/04/shakti-ctf-2021-art-gallery-2/)
	
- [albertofdr : emoji-voting,CyberApocalypse](https://albertofdr.github.io/ctf/htb/en/2021/04/24/ctf-htb.html#emoji-voting)
	
- [kblagoev : emoji-voting, CyberApocalypse](https://kblagoev.com/blog/emoji-voting-cyberapocalypse-2021-ctf/)
	
- [noob3xploiter : AlexFanClub](https://noob3xploiter.medium.com/lit-ctf-alex-fan-club-sql-injection-with-strict-blacklist-7abbcd402751)
	
- [bi0s : Vuln-Drive, InCTF](https://blog.bi0s.in/2021/08/15/Web/Vuln-Drive-InCTF-Internationals-2021/) :fire:




</details>


<details>
	<summary>further-reading</summary>

### further-reading 

- [Faith : Regex-based Blind SQL Injection Attacks](https://faraz.faith/2019-07-28-regex-based-blind-sql-injection-attacks/)


- [chivato : Taking SQL Injections Further](https://0x00sec.org/t/taking-sql-injections-further-blind-second-order-sql-injection-tmhc-ctf-shitter-writeup/18122)


- [hackingarticles : exploiting form based sqli using sqlmap](https://www.hackingarticles.in/exploiting-form-based-sql-injection-using-sqlmap/)

- [Beyond SQLi: Obfuscate and Bypass](https://www.exploit-db.com/papers/17934)

- [Preventing 'SQLi'...](https://blogs.tunelko.com/2013/12/12/preventing-sqli-cheatsheet-during-attack-defense-ctf-basic-approach/)

- [Sql Injection Payload list](https://ismailtasdelen.medium.com/sql-injection-payload-list-b97656cfd66b)

- [Identifying & Exploiting SQL Injections: Manual & Automated](https://infosecwriteups.com/identifying-exploiting-sql-injection-manual-automated-79c932f0c9b5)

- [SQL Injections 😈](https://medium.com/faun/sql-injections-e8bc9a14c95)

- [Learn About SQL Injection Attacks](https://betterprogramming.pub/learn-about-sql-injection-attacks-ce9f8940a5ab)

- [exploiting sqli](https://medium.com/dev-genius/exploiting-sql-injection-vulnerabilities-76df9b85dd7)

- [SQL Injection Attack — it might pain!](https://medium.com/spidernitt/sql-injection-attack-it-might-pain-44ab11056f6c)

</details>


<details>
	<summary>some-labs</summary>

### some-labs 

- [beginner sqli](https://github.com/ryotosaito/beginner-sqli)	

</details>
