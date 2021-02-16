# SSRF

![](ssrf.jpg)

## Intro to SSRFs 
>> server-side request forgery
In computer security, server-side request forgery (SSRF) is a type of exploit where an attacker abuses the functionality of a server causing it to access or manipulate information in the realm of that server that would otherwise not be directly accessible to the attacker.

<a href="https://en.wikipedia.org/wiki/Server-side_request_forgery">SSRF</a>



<details>
  <summary>CTF Writeups</summary> 
 
### CTF Writeups
  
- [2018](#2018)

- [2019](#2019)

- [2020](#2020)

- [2021](#2021)

- [other-reads](#other-interesting-reads)

- [Bug-Bounty](#Bug-Bounty-and-RVDs)


### 2018

- <a href="https://qiita.com/no1zy_sec/items/03b8f335e84995fec3e3">noizy_sec : HamaCTF xmlvalidator writeup</a>

- <a href="https://blog.cal1.cn/post/RealWorldCTF%20PrintMD%20writeup">cal1 : RealWorldCTF 2018 PrintMD</a>

- <a href="https://fireshellsecurity.team/nonamectf-convert/">fireshell : nonamectf-convert</a>

- <a href="https://spyclub.tech/2018/10/08/2018-10-08-inctf2018-web-challenge-writeup/">Spyclub : inctf2018 GoSqlv1</a>

### 2019

- <a href="https://github.com/10secTW/ctf-writeup/blob/master/2019/ASIS%20CTF%20quals/Web%20-%20Baby%20SSRF.md">10secTW : Baby SSRF ASIS QUALS 2019</a>

- <a href="https://abcdsh.blogspot.com/2019/04/writeup-asis-2019-quals-baby-ssrf.html">csi : Baby SSRF ASIS QUALS 2019</a>

- <a href="https://systemoverlord.com/2019/03/07/bsides-sf-ctf-author-writeup-cloud2clown.html">systemoverlord : bsides-sf cloud2clown

- <a href="https://movrment.blogspot.com/2019/10/balsn-ctf-2019-web-warmup.html">movrment : Balsn 2019 Web Warmup</a>

- <a href="https://https://fireshellsecurity.team/bytebandits-imgaccess/">fireshell : bytebandits 2019 imgaccess</a>

- <a href="https://github.com/will-lynas/writeups/blob/master/ctf/de1ctf-2019/SSRF_me.md">will-lynas: de1ctf-2019/SSRF_me</a>

- <a href="https://samirettali.com/writeups/de1ctf/ssrfme">Samirettali: de1ctf-2019 SSRF-ME</a>

- <a href="https://blog.bi0s.in/2019/10/16/Web/inctfi19-web-writeups/">bi0s: inctf2019 GoSQLv2</a>

- <a href="https://nytr0gen.github.io/writeups/ctf/2019/09/09/defcamp-ctf-quals-2019.html#imgur-202p-web">nytrogen : defcamp quals 2019 imgur</a>

- <a href="https://github.com/De1ta-team/De1CTF2019/tree/master/writeup/web/SSRF%20Me">De1ta-team : De1CTF2019/SSRF_ME</a>

### 2020

- <a href="https://hackerone.com/reports/776634">manoelt : [H1-415 2020] CTF Writeup</a>

- <a href="https://lbherrera.github.io/lab/h1415-ctf-writeup.html">lbherrera : [H1-415 2020] CTF Writeup</a>

- <a href="https://r3billions.com/writeup-split-second/">r3billions : split-second Nullcon 2020/</a>

- <a href="http://blog.zeddyu.info/2020/04/20/Plaid-CTF-2020-Web-1/">zeddyu : Plaid-CTF-2020-Web-1</a>

- <a href="https://balsn.tw/ctf_writeup/20200418-plaidctf2020/#contrived-web-problem">Bookgin : PlaidCTF 2020 contrived web problem</a>

- <a href="https://github.com/perfectblue/ctf-writeups/tree/master/2020/plaidctf-2020/contrived-web">ret2jazzy : PlaidCTF 2020 contrived web</a>

- <a href="https://ahmed-belkahla.me/post/fword-ctf2020/">ahmed : Fword 2020 PastaXSS</a>

- <a href="https://rmb122.com/2020/12/30/hxp-CTF-resonator-Writeup-SSRF-via-file-put-contents/">rmb122 : hxp 2020 reasonator</a>

- <a href="https://spyclub.tech/2020/08/02/inctf2020-gosqlv3-challenge-writeup/">spyclub : inctf 2020 GoSQLv3</a>

- <a href="http://jackson-t.ca/metasploitctf-2020-rmf.html">jackson-t : MetasploitCTF 2020</a>

- <a href="https://hackmd.io/@mystiz/twctf-2020-writeup#urlcheck-v1-Web-98-points">mystiz : urlcheck-v1 TokyoWesterns 2020</a>	

- <a href="https://hackmd.io/@mystiz/twctf-2020-writeup#urlcheck-v2-Web-128-points">mystiz : urlcheck-v2 TokyoWesterns 2020 </a>

### 2021

- <a href="https://blog.brycec.me/posts/starctf2021_writeups/">brycec : *CTF 2021</a>

- <a href="https://github.com/sambrow/ctf-writeups-2021/tree/master/bamboo-fox/ssrfrog">sambrow : SSRFrog Bamboofox2021</a>

- <a href="https://maxdamage.dev/posts/bctf-ssrfrog.html">maxdamage : SSRFrog Bamboofox2021</a>

- <a href="https://eine.tistory.com/entry/BambooCTF-2021-web-SSRFrog-Time-to-Draw-write-up"> Einstrasse : SSRFrog Bamboofox2021</a>
  
</details>

<details>
  <summary>Other interesting reads</summary>
  
### Other interesting reads

- <a href="https://www.blackhat.com/docs/us-17/thursday/us-17-Tsai-A-New-Era-Of-SSRF-Exploiting-URL-Parser-In-Trending-Programming-Languages.pdf">Orange Tsai : Blackhat Talk</a>

- <a href="https://www.netsparker.com/blog/web-security/server-side-request-forgery-vulnerability-ssrf/">netsparker: server-side-request-forgery-vulnerability-ssrf</a>

- <a href="https://medium.com/swlh/intro-to-ssrf-beb35857771f">Vicki Li : Intro to SSRFs</a>

- <a href="https://github.com/jdonsec/AllThingsSSRF">jdonsec : AllThingsSSRF</a>

- <a href="https://medium.com/seconset/all-about-ssrf-524f41ab96df">Tushar Verma : All about SSRF</a>

- <a href="https://book.hacktricks.xyz/pentesting-web/ssrf-server-side-request-forgery">Hacktricks : ssrf-server-side-request-forgery</a>
</details>

<details>
  <summary>Bug Bounty and RVDs</summary>

### Bug Bounty and RVDs

- <a href="https://www.corben.io/hackertarget/">Corben : Hackertarget</a>

- <a href="https://pwning.re/2018/05/23/shopify-ssrf-to-rce/">Andre : shopify-ssrf-to-rce</a>

- <a href="https://fireshellsecurity.team/1000-ssrf-in-slack/">$1000-ssrf-in-slack</a>

- [From SSRF to $4000](https://thehackerish.com/bug-bounty-write-up-from-ssrf-to-4000/)

- [Escalate SSRF to RCE](https://sanderwind.medium.com/escalating-ssrf-to-rce-7c0147371c40)

- [Story Behind Sweet SSRF](https://rohit-soni.medium.com/story-behind-sweet-ssrf-40c705f13053)

- [$10000 Facebook SSRF](https://medium.com/@amineaboud/10000-facebook-ssrf-bug-bounty-402bd21e58e5)

- [31k$ SSRF in Google Cloud Monitoring led to metadata exposure](https://nechudav.blogspot.com/2020/11/31k-ssrf-in-google-cloud-monitoring.html)
</details>
