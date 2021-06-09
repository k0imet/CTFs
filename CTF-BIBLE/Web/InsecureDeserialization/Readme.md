# Insecure-Deseralization 

![](serialize.png)

<details>
	<summary>What is insecure deserialization?</summary>

## What is insecure deserialization?

- Let’s first understand the whole picture here. When you learn a programming language, the first thing you learn is how to define variables, classes and data structures that best suit your needs. Then, you learn how to manipulate them to achieve your needs. So far, they reside in memory, but sometimes, you need to store their states or share them with other systems. That’s where serialization and deserialization come into play.

### What is Serialization?

- Let’s say that you are playing with a character in a game. While you see the character on the screen, the software sees and manipulates an object residing in memory.

- What if the game wants to store the state of that character in a file or share it with other systems? There should be a way to transform the in-memory object into a stream of bytes which can be easily stored and shared. That is what the process of serialization is all about. When the game performs the serialization of an object, we say that the object is serialized.


### What is Deserialization?

- Deserialization is the opposite of serialization. In fact, it consists of converting the serialized data into an in-memory representation which the software can then manipulate. Continuing on the previous example, when the game wants to retrieve the state of the serialized character object, it needs to deserialize it first.
What can go wrong here?

When a software deserializes user-controlled data without verification, we call it insecure deserialization. In our game example, an attacker might store a serialized file representing a malicious payload. If the developer doesn’t perform a verification before deserialization, the insecure deserialization will trigger the attacker’s code.
[Full Article](https://thehackerish.com/insecure-deserialization-explained-with-examples/)

</details>


<details>
	<summary>CTF-Writeups</summary>


## CTF-Writeups

- [2010](#2010)

- [2012](#2012)

- [2013](#2013)

- [2014](#2014)

- [2016](#2016)

- [2018](#2018)

- [2019](#2019)

- [2020](#2020)

- [2021](#2021)


### 2010 

- [hack-lu pigs](https://websec.wordpress.com/2010/10/30/hack-lu-ctf-challenge-21-writeup-pigs/)

### 2012 

- [fdfalcon : Zombie Reminder,Hack.lu ](https://sysexit.wordpress.com/2012/10/25/hacklu-ctf-2012-zombie-reminder-200-write-up/)

### 2013

- [scoding : exloit 100,VolgaCTF](https://scoding.de/volgactf-2013-writeup-exploit100)

### 2014

- [Skullsecurity : kpop bad deserialization](https://blog.skullsecurity.org/2014/plaidctf-writeup-for-web-200-kpop-bad-deserialization)

- [Plaid CTF 2014: "reeekeeeeee" 200 pts](http://security.cs.pub.ro/hexcellents/wiki/writeups/pctf2014_reekee)

### 2016 

- [TUCTF LuckyCharms. Exploiting Simple Java Deserialization Vulnerability.](https://breaking.into.systems/read/2016/TUCTF-LuckyCharms-Exploiting-simple-Java-deserialization-vuln)

- [0daylabs : PHP object Injection via Cookie unserialize() - Nuit du hack CTF Web 100 writeup](https://blog.0daylabs.com/2016/04/03/unserialize-php-object-injection)

- [hack.more : free_as_as_in_bavarian_beer](https://hack.more.systems/writeup/2016/10/02/tumctf-web50/)

### 2017

- [necst : lamermi,PoliCTF](https://toh.necst.it/polictf/pwnable/Lamermi/)

- [Apj: TSULOTT,meepwn](https://advancedpersistentjest.com/2017/07/17/writeup-tsulott-meepwn/)

- [depier " 2nd Secured Portal,AsisCTF"](https://depier.re/asis_2017_2nd_secured_portal/)


### 2018 

- [k3ramas : Challenge 4,Recon Village](https://k3ramas.blogspot.com/2018/08/recon-village-ctf-defcon-26.html)

- [cyku : Why-so-serials,Hitcon](https://cyku.tw/ctf-hitcon-2018-why-so-serials/)

- [s0cket7 : Flask Skeleton Cards,PicoCTF](https://s0cket7.com/picoctf-web/)

- [Balsn : 300-3,TrendMicro](https://balsn.tw/ctf_writeup/20180914-trendmicroctf/#300-3)

- [Pharisaeus : 300-3,TrendMicro](https://github.com/p4-team/ctf/tree/master/2018-09-15-trendmicro/misc_deserializer)

- [galdeleon : 35c3_php](https://github.com/galdeleon/35c3_php)

- [rayoflightz : 35c33_php](https://rayoflightz.github.io/writeup/web/2019/01/03/35c3-php-writeup.html) 

- [Jaimin : PHP object injection in kaspersky CTF](https://medium.com/@jaimin_gohel/ctf-writeup-php-object-injection-in-kaspersky-ctf-28a68805610d)

- [hackso : im-pickle-rick,bsidestlv](https://hackso.me/bsidestlv-web/#im-pickle-rick)

- [Terry : My Flask App,Mitre CTF](https://terryvogelsang.tech/MITRECTF2018-my-flask-app/)

- [alsn : Identify-the-function,Pwn2win](https://balsn.tw/ctf_writeup/20181130-pwn2winctf/#identify-the-function)

- [securimag :  filevault,insomnihack teaser](https://securimag.org/wp/challenges/writeup-insomnihack-teaser-2018-filevault/)

- [Jbz : 420 Quiz, MatesCTF](https://jbz.team/matesctf2018/420-Quiz)


### 2019 

- [peterjson : ISITDTU Finals ](https://peterjson.medium.com/isitdtu-ctf-final-2019-web-write-ups-c845ce85808e)

- [bananamafia : Exploiting PHP Deserialization: CCCamp19 CTF PDFCreator Challenge](https://bananamafia.dev/post/php-deserialize-cccamp19/)

- [haboob : mimeCheckr,nullcon](https://haboob.sa/ctf/nullcon-2019/mimeCheckr.html)

### 2020

- [Super Guesser : Web signin,N1CTF](https://github.com/Super-Guesser/ctf/tree/master/2020/N1CTF%202020/web/signin)

- [abinpaul1 : Too_Many_Credits,TamuCTF](https://github.com/abinpaul1/CTF-Writeups/blob/master/TAMUCTF%202020%20-%20Too_Many_Credits/README.md)


- [r3billions : writeup-defiltrate-part1](https://r3billions.com/writeup-defiltrate-part1/)

- [sqrtrev : Image uploader,3kCTF]https://vuln.live/blog/11)

- [harrier : deserializeme,UIUCTF](https://hackmd.io/@harrier/uiuctf20#deserializeme-450-3-solves-solved-by-ozetta-and-harrier)

- [RB : L5D,Balsn 2020](https://blog.rb363.tw/2020/12/04/Balsn-CTF-2020-L5D/)

- [eine : Official Business,Nahamcon](https://eine.tistory.com/entry/NahamCON-CTF-2020-Write-ups)

- [Saudi : CyberTalents Weekend CTF-gu55y writeup](https://trevorsaudi.medium.com/cybertalents-weekend-ctf-gu55y-writeup-php-object-injection-dfe173d9f446)

### 2021 

- [f5,Old System,RealWorldCTF](https://f5.pm/go-53869.html)


</details>

<details>
	<summary>Further-Reading</summary>

### Further-Reading 

- [Exploiting PHP Phar Deserialization Vulnerabilities](https://blogs.keysight.com/blogs/tech/nwvs.entry.html/2019/06/26/exploiting_php_phar-PRD7.html)

- [Apache Tomcat RCE by deserialization (CVE-2020-9484) – write-up and exploit](https://www.redtimmy.com/apache-tomcat-rce-by-deserialization-cve-2020-9484-write-up-and-exploit/)

- [Exploiting Node.js deserialization bugfor Remote Code Execution(CVE-2017-5941)](https://www.exploit-db.com/docs/english/41289-exploiting-node.js-deserialization-bug-for-remote-code-execution.pdf)


- [Hessian deserialization and related gadget chains](https://paper.seebug.org/1137/)


- [Practical PHP Object Injection](https://insomniasec.com/cdn-assets/Practical_PHP_Object_Injection.pdf)


- [Understanding & practicing java deserialization exploits](https://diablohorn.com/2017/09/09/understanding-practicing-java-deserialization-exploits/)

- [Automated Discovery of Deserialization Gadget Chains](https://i.blackhat.com/us-18/Thu-August-9/us-18-Haken-Automated-Discovery-of-Deserialization-Gadget-Chains-wp.pdf)

- [awae preparation](https://z-r0crypt.github.io/blog/2020/01/22/oswe/awae-preparation/)


- [PHP Object Injection Cheatsheet](https://nitesculucian.github.io/2018/10/05/php-object-injection-cheat-sheet/)

</details>
