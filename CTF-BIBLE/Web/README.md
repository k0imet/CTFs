# TOC
## Topics 
- [LFI](./LFI)

- [SSRF](./SSRF)

- [SSTI](./SSTI)

- [XXE](./XXE)

- [SQLi](./SQLi)

- [XSS](./XSS)

- [InsecureDeserialization](./InsecureDeserialization)


<details>
  

  <summary>Vulnerabilities in Web Applications</summary>

### Introduction

How is private information leaked from social networking sites? How can someone’s bank account get compromised by just clicking on a link in an email? Why are we advised to not use the same password on different sites? What are those annoying “accept cookie banners” that pop up every time? How do characters in movies get into their school’s database to change their grade?

If you’ve ever encountered any of the above questions and wanted to learn how these things happen, we’ve got you covered. In these tutorials we will be discussing about common vulnerabilities in web applications and how can those be exploited by attackers. But these tutorials cover a lot more than that. They will help you gain a deeper understanding into how stuff works, and if you are a developer, will help you to make more robust applications!

### What does a vulnerability mean?

A website vulnerability is a weakness or misconfiguration in a website or web application code that allows an attacker to gain some level of control of the site, and possibly the hosting server.

#### What kind of harm does it pose?

There are different types of vulnerabilities, targetting different functions of a web application like gaining access to the database of a website revealing personal information of users, running a script in the background to access data from your computer, or a script that transfers money from your bank account!

##### Types of Vulnerabilities

Different kinds of attacks are possible on web applications, but here we’ll be listing the top 10 according to the OWASP(Open Web Application Security Project, or OWASP, is an international non-profit organization dedicated to web application security.) report.
Injection

Injection attacks happen when untrusted data is sent to a code interpreter through a form input or some other data submission to a web application. For example, an attacker could enter SQL database code into a form that expects a plaintext username. If that form input is not properly secured, this would result in that SQL code being executed. This is known as an SQL injection attack. Injection attacks can be prevented by validating and/or sanitizing user-submitted data. (Validation means rejecting suspicious-looking data, while sanitization refers to cleaning up the suspicious-looking parts of the data.) In addition, a database admin can set controls to minimize the amount of information an injection attack can expose.
### Broken Authentication

Vulnerabilities in authentication (login) systems can give attackers access to user accounts and even the ability to compromise an entire system using an admin account. For example, an attacker can take a list containing thousands of known username/password combinations obtained during a data breach and use a script to try all those combinations on a login system to see if there are any that work. Not even this, there are potential vulnerabilities in 2 Factor Authentication as well!

### Sensitive Data Exposure

If web applications don’t protect sensitive data such as financial information and passwords, attackers can gain access to that data and sellor utilize it for nefarious purposes. One popular method for stealing sensitive information is using a man-in-the-middle attack. So, the applications generally store this sensitive data in encrypted format.

### XML External Entities (XXE)

XML external entity injection (also known as XXE) is a web security vulnerability that allows an attacker to interfere with an application’s processing of XML data. It often allows an attacker to view files on the application server filesystem, and to interact with any backend or external systems that the application itself can access. The best ways to prevent XEE attacks are to have web applications accept a less complex type of data, such as JSON, or at the very least to patch XML parsers and disable the use of external entities (An ‘external entity’ in this context refers to a storage unit, such as a hard drive.) in an XML application.
### Broken Access Control

Access control refers a system that controls access to information or functionality. Broken access controls allow attackers to bypass authorization and perform tasks as though they were privileged users such as administrators. For example a web application could allow a user to change which account they are logged in as simply by changing part of a url, without any other verification.

### Security Misconfiguration

Security misconfiguration is the most common vulnerability, and is often the result of using default configurations or displaying excessively verbose errors. For instance, an application could show a user overly-descriptive errors which may reveal vulnerabilities in the application. This can be mitigated by removing any unused features in the code and ensuring that error messages are more general (like Internal Server Error or Bad Request).

### Cross-Site Scripting

Cross-site scripting vulnerabilities occur when web applications allow users to add custom code into a url path or onto a website that will be seen by other users. This vulnerability can be exploited to run malicious JavaScript code on a victim’s browser. For example, an attacker could send an email to a victim that appears to be from a trusted bank, with a link to that bank’s website. This link could have some malicious JavaScript code tagged onto the end of the url. If the bank’s site is not properly protected against cross-site scripting, then that malicious code will be run in the victim’s web browser when they click on the link. Mitigation strategies for cross-site scripting include escaping untrusted HTTP requests as well as validating and/or sanitizing user-generated content. Using modern web development frameworks like ReactJS and Ruby on Rails also provides some built-in cross-site scripting protection.

### Insecure Deserialization

This threat targets the many web applications which frequently serialize and deserialize data. Serialization means taking objects from the application code and converting them into a format that can be used for another purpose, such as storing the data to disk or streaming it. Deserialization is just the opposite: converting serialized data back into objects the application can use. Serialization is sort of like packing furniture away into boxes before a move, and deserialization is like unpacking the boxes and assembling the furniture after the move. An insecure deserialization attack is like having the movers tamper with the contents of the boxes before they are unpacked.

### Using Components With Known Vulnerabilities

Many modern web developers use components such as libraries and frameworks in their web applications. These components are pieces of software that help developers avoid redundant work and provide needed functionality; common example include front-end frameworks like React and smaller libraries that used to add share icons or a/b testing. Some attackers look for vulnerabilities in these components which they can then use to orchestrate attacks. Some of the more popular components are used on hundreds of thousands of websites; an attacker finding a security hole in one of these components could leave hundreds of thousands of sites vulnerable to exploit.

### Insufficient Logging And Monitoring

Many web applications are not taking enough steps to detect data breaches. The average discovery time for a breach is around 200 days after it has happened. This gives attackers a lot of time to cause damage before there is any response. OWASP recommends that web developers should implement logging and monitoring as well as incident response plans to ensure that they are made aware of attacks on their applications.

<a href="https://csea-iitb.github.io/IITBreachers-wiki/2020/07/22/Web-Vulnerabilities.html">Read More</a>
</details>
