## CVE-2012-6636
 The Android API before 17 does not properly restrict the WebView.addJavascriptInterface method, which allows remote attackers to execute arbitrary methods of Java objects by using the Java Reflection API within crafted JavaScript code that is loaded into the WebView component in an application targeted to API level 16 or earlier, a related issue to CVE-2013-4710.



- [https://github.com/xckevin/AndroidWebviewInjectDemo](https://github.com/xckevin/AndroidWebviewInjectDemo) :  ![starts](https://img.shields.io/github/stars/xckevin/AndroidWebviewInjectDemo.svg) ![forks](https://img.shields.io/github/forks/xckevin/AndroidWebviewInjectDemo.svg)

- [https://github.com/Snip3R69/CVE-2013-4710-WebView-RCE-Vulnerability](https://github.com/Snip3R69/CVE-2013-4710-WebView-RCE-Vulnerability) :  ![starts](https://img.shields.io/github/stars/Snip3R69/CVE-2013-4710-WebView-RCE-Vulnerability.svg) ![forks](https://img.shields.io/github/forks/Snip3R69/CVE-2013-4710-WebView-RCE-Vulnerability.svg)

## CVE-2012-6066
 freeSSHd.exe in freeSSHd through 1.2.6 allows remote attackers to bypass authentication via a crafted session, as demonstrated by an OpenSSH client with modified versions of ssh.c and sshconnect2.c.



- [https://github.com/bongbongco/CVE-2012-6066](https://github.com/bongbongco/CVE-2012-6066) :  ![starts](https://img.shields.io/github/stars/bongbongco/CVE-2012-6066.svg) ![forks](https://img.shields.io/github/forks/bongbongco/CVE-2012-6066.svg)

## CVE-2012-5960
 Stack-based buffer overflow in the unique_service_name function in ssdp/ssdp_server.c in the SSDP parser in the portable SDK for UPnP Devices (aka libupnp, formerly the Intel SDK for UPnP devices) before 1.6.18 allows remote attackers to execute arbitrary code via a long UDN (aka upnp:rootdevice) field in a UDP packet.



- [https://github.com/finn79426/CVE-2012-5960-PoC](https://github.com/finn79426/CVE-2012-5960-PoC) :  ![starts](https://img.shields.io/github/stars/finn79426/CVE-2012-5960-PoC.svg) ![forks](https://img.shields.io/github/forks/finn79426/CVE-2012-5960-PoC.svg)

## CVE-2012-5959
 Stack-based buffer overflow in the unique_service_name function in ssdp/ssdp_server.c in the SSDP parser in the portable SDK for UPnP Devices (aka libupnp, formerly the Intel SDK for UPnP devices) before 1.6.18 allows remote attackers to execute arbitrary code via a long UDN (aka uuid) field within a string that contains a :: (colon colon) in a UDP packet.



- [https://github.com/lochiiconnectivity/vulnupnp](https://github.com/lochiiconnectivity/vulnupnp) :  ![starts](https://img.shields.io/github/stars/lochiiconnectivity/vulnupnp.svg) ![forks](https://img.shields.io/github/forks/lochiiconnectivity/vulnupnp.svg)

- [https://github.com/finn79426/CVE-2012-5960-PoC](https://github.com/finn79426/CVE-2012-5960-PoC) :  ![starts](https://img.shields.io/github/stars/finn79426/CVE-2012-5960-PoC.svg) ![forks](https://img.shields.io/github/forks/finn79426/CVE-2012-5960-PoC.svg)

## CVE-2012-5958
 Stack-based buffer overflow in the unique_service_name function in ssdp/ssdp_server.c in the SSDP parser in the portable SDK for UPnP Devices (aka libupnp, formerly the Intel SDK for UPnP devices) before 1.6.18 allows remote attackers to execute arbitrary code via a UDP packet with a crafted string that is not properly handled after a certain pointer subtraction.



- [https://github.com/lochiiconnectivity/vulnupnp](https://github.com/lochiiconnectivity/vulnupnp) :  ![starts](https://img.shields.io/github/stars/lochiiconnectivity/vulnupnp.svg) ![forks](https://img.shields.io/github/forks/lochiiconnectivity/vulnupnp.svg)

## CVE-2012-5664
 DO NOT USE THIS CANDIDATE NUMBER. ConsultIDs: CVE-2012-6496, CVE-2012-6497. Reason: this candidate was intended for one issue, but the candidate was publicly used to label concerns about multiple products. Notes: All CVE users should consult CVE-2012-6496 and CVE-2012-6497 to determine which ID is appropriate. All references and descriptions in this candidate have been removed to prevent accidental usage.



- [https://github.com/phusion/rails-cve-2012-5664-test](https://github.com/phusion/rails-cve-2012-5664-test) :  ![starts](https://img.shields.io/github/stars/phusion/rails-cve-2012-5664-test.svg) ![forks](https://img.shields.io/github/forks/phusion/rails-cve-2012-5664-test.svg)

## CVE-2012-5613
 MySQL 5.5.19 and possibly other versions, and MariaDB 5.5.28a and possibly other versions, when configured to assign the FILE privilege to users who should not have administrative privileges, allows remote authenticated users to gain privileges by leveraging the FILE privilege to create files as the MySQL administrator. NOTE: the vendor disputes this issue, stating that this is only a vulnerability when the administrator does not follow recommendations in the product's installation documentation. NOTE: it could be argued that this should not be included in CVE because it is a configuration issue.



- [https://github.com/Hood3dRob1n/MySQL-Fu.rb](https://github.com/Hood3dRob1n/MySQL-Fu.rb) :  ![starts](https://img.shields.io/github/stars/Hood3dRob1n/MySQL-Fu.rb.svg) ![forks](https://img.shields.io/github/forks/Hood3dRob1n/MySQL-Fu.rb.svg)

- [https://github.com/w4fz5uck5/UDFPwn-CVE-2012-5613](https://github.com/w4fz5uck5/UDFPwn-CVE-2012-5613) :  ![starts](https://img.shields.io/github/stars/w4fz5uck5/UDFPwn-CVE-2012-5613.svg) ![forks](https://img.shields.io/github/forks/w4fz5uck5/UDFPwn-CVE-2012-5613.svg)

## CVE-2012-5575
 Apache CXF 2.5.x before 2.5.10, 2.6.x before CXF 2.6.7, and 2.7.x before CXF 2.7.4 does not verify that a specified cryptographic algorithm is allowed by the WS-SecurityPolicy AlgorithmSuite definition before decrypting, which allows remote attackers to force CXF to use weaker cryptographic algorithms than intended and makes it easier to decrypt communications, aka "XML Encryption backwards compatibility attack."



- [https://github.com/tafamace/CVE-2012-5575](https://github.com/tafamace/CVE-2012-5575) :  ![starts](https://img.shields.io/github/stars/tafamace/CVE-2012-5575.svg) ![forks](https://img.shields.io/github/forks/tafamace/CVE-2012-5575.svg)

## CVE-2012-5519
 CUPS 1.4.4, when running in certain Linux distributions such as Debian GNU/Linux, stores the web interface administrator key in /var/run/cups/certs/0 using certain permissions, which allows local users in the lpadmin group to read or write arbitrary files as root by leveraging the web interface.



- [https://github.com/p1ckzi/CVE-2012-5519](https://github.com/p1ckzi/CVE-2012-5519) :  ![starts](https://img.shields.io/github/stars/p1ckzi/CVE-2012-5519.svg) ![forks](https://img.shields.io/github/forks/p1ckzi/CVE-2012-5519.svg)

## CVE-2012-5321
 tiki-featured_link.php in TikiWiki CMS/Groupware 8.3 allows remote attackers to load arbitrary web site pages into frames and conduct phishing attacks via the url parameter, aka "frame injection."



- [https://github.com/Cappricio-Securities/CVE-2012-5321](https://github.com/Cappricio-Securities/CVE-2012-5321) :  ![starts](https://img.shields.io/github/stars/Cappricio-Securities/CVE-2012-5321.svg) ![forks](https://img.shields.io/github/forks/Cappricio-Securities/CVE-2012-5321.svg)

## CVE-2012-5221
 Directory traversal vulnerability in the PostScript Interpreter, as used on the HP LaserJet 4xxx, 5200, 90xx, M30xx, M4345, M50xx, M90xx, P3005, and P4xxx; LaserJet Enterprise P3015; Color LaserJet 3xxx, 47xx, 5550, 9500, CM60xx, CP35xx, CP4005, and CP6015; Color LaserJet Enterprise CP4xxx; and 9250c Digital Sender with model-dependent firmware through 52.x allows remote attackers to read arbitrary files via unknown vectors.



- [https://github.com/aredspy/HPCredDumper](https://github.com/aredspy/HPCredDumper) :  ![starts](https://img.shields.io/github/stars/aredspy/HPCredDumper.svg) ![forks](https://img.shields.io/github/forks/aredspy/HPCredDumper.svg)

## CVE-2012-5106
 Stack-based buffer overflow in FreeFloat FTP Server 1.0 allows remote authenticated users to execute arbitrary code via a long string in a PUT command.



- [https://github.com/war4uthor/CVE-2012-5106](https://github.com/war4uthor/CVE-2012-5106) :  ![starts](https://img.shields.io/github/stars/war4uthor/CVE-2012-5106.svg) ![forks](https://img.shields.io/github/forks/war4uthor/CVE-2012-5106.svg)

## CVE-2012-4960
 The Huawei NE5000E, MA5200G, NE40E, NE80E, ATN, NE40, NE80, NE20E-X6, NE20, ME60, CX600, CX200, CX300, ACU, WLAN AC 6605, S9300, S7700, S2300, S3300, S5300, S3300HI, S5300HI, S5306, S6300, S2700, S3700, S5700, S6700, AR G3, H3C AR(OEM IN), AR 19, AR 29, AR 49, Eudemon100E, Eudemon200, Eudemon300, Eudemon500, Eudemon1000, Eudemon1000E-U/USG5300, Eudemon1000E-X/USG5500, Eudemon8080E/USG9300, Eudemon8160E/USG9300, Eudemon8000E-X/USG9500, E200E-C/USG2200, E200E-X3/USG2200, E200E-X5/USG2200, E200E-X7/USG2200, E200E-C/USG5100, E200E-X3/USG5100, E200E-X5/USG5100, E200E-X7/USG5100, E200E-B/USG2100, E200E-X1/USG2100, E200E-X2/USG2100, SVN5300, SVN2000, SVN5000, SVN3000, NIP100, NIP200, NIP1000, NIP2100, NIP2200, and NIP5100 use the DES algorithm for stored passwords, which makes it easier for context-dependent attackers to obtain cleartext passwords via a brute-force attack.



- [https://github.com/ghcohu/Decrypt-passwords-for-Huawei-routers-and-switches-CVE-2012-4960](https://github.com/ghcohu/Decrypt-passwords-for-Huawei-routers-and-switches-CVE-2012-4960) :  ![starts](https://img.shields.io/github/stars/ghcohu/Decrypt-passwords-for-Huawei-routers-and-switches-CVE-2012-4960.svg) ![forks](https://img.shields.io/github/forks/ghcohu/Decrypt-passwords-for-Huawei-routers-and-switches-CVE-2012-4960.svg)

## CVE-2012-4929
 The TLS protocol 1.2 and earlier, as used in Mozilla Firefox, Google Chrome, Qt, and other products, can encrypt compressed data without properly obfuscating the length of the unencrypted data, which allows man-in-the-middle attackers to obtain plaintext HTTP headers by observing length differences during a series of guesses in which a string in an HTTP request potentially matches an unknown string in an HTTP header, aka a "CRIME" attack.



- [https://github.com/mpgn/CRIME-poc](https://github.com/mpgn/CRIME-poc) :  ![starts](https://img.shields.io/github/stars/mpgn/CRIME-poc.svg) ![forks](https://img.shields.io/github/forks/mpgn/CRIME-poc.svg)

- [https://github.com/anthophilee/A2SV--SSL-VUL-Scan](https://github.com/anthophilee/A2SV--SSL-VUL-Scan) :  ![starts](https://img.shields.io/github/stars/anthophilee/A2SV--SSL-VUL-Scan.svg) ![forks](https://img.shields.io/github/forks/anthophilee/A2SV--SSL-VUL-Scan.svg)

## CVE-2012-4869
 The callme_startcall function in recordings/misc/callme_page.php in FreePBX 2.9, 2.10, and earlier allows remote attackers to execute arbitrary commands via the callmenum parameter in a c action.



- [https://github.com/AndyCyberSec/OSCP](https://github.com/AndyCyberSec/OSCP) :  ![starts](https://img.shields.io/github/stars/AndyCyberSec/OSCP.svg) ![forks](https://img.shields.io/github/forks/AndyCyberSec/OSCP.svg)

- [https://github.com/cyberdesu/Elastix-2.2.0-CVE-2012-4869](https://github.com/cyberdesu/Elastix-2.2.0-CVE-2012-4869) :  ![starts](https://img.shields.io/github/stars/cyberdesu/Elastix-2.2.0-CVE-2012-4869.svg) ![forks](https://img.shields.io/github/forks/cyberdesu/Elastix-2.2.0-CVE-2012-4869.svg)

## CVE-2012-4792
 Use-after-free vulnerability in Microsoft Internet Explorer 6 through 8 allows remote attackers to execute arbitrary code via a crafted web site that triggers access to an object that (1) was not properly allocated or (2) is deleted, as demonstrated by a CDwnBindInfo object, and exploited in the wild in December 2012.



- [https://github.com/WizardVan/CVE-2012-4792](https://github.com/WizardVan/CVE-2012-4792) :  ![starts](https://img.shields.io/github/stars/WizardVan/CVE-2012-4792.svg) ![forks](https://img.shields.io/github/forks/WizardVan/CVE-2012-4792.svg)

## CVE-2012-4681
 Multiple vulnerabilities in the Java Runtime Environment (JRE) component in Oracle Java SE 7 Update 6 and earlier allow remote attackers to execute arbitrary code via a crafted applet that bypasses SecurityManager restrictions by (1) using com.sun.beans.finder.ClassFinder.findClass and leveraging an exception with the forName method to access restricted classes from arbitrary packages such as sun.awt.SunToolkit, then (2) using "reflection with a trusted immediate caller" to leverage the getField method to access and modify private fields, as exploited in the wild in August 2012 using Gondzz.class and Gondvv.class.



- [https://github.com/benjholla/CVE-2012-4681-Armoring](https://github.com/benjholla/CVE-2012-4681-Armoring) :  ![starts](https://img.shields.io/github/stars/benjholla/CVE-2012-4681-Armoring.svg) ![forks](https://img.shields.io/github/forks/benjholla/CVE-2012-4681-Armoring.svg)

- [https://github.com/ZH3FENG/PoCs-CVE_2012_4681](https://github.com/ZH3FENG/PoCs-CVE_2012_4681) :  ![starts](https://img.shields.io/github/stars/ZH3FENG/PoCs-CVE_2012_4681.svg) ![forks](https://img.shields.io/github/forks/ZH3FENG/PoCs-CVE_2012_4681.svg)

## CVE-2012-4431
 org/apache/catalina/filters/CsrfPreventionFilter.java in Apache Tomcat 6.x before 6.0.36 and 7.x before 7.0.32 allows remote attackers to bypass the cross-site request forgery (CSRF) protection mechanism via a request that lacks a session identifier.



- [https://github.com/imjdl/CVE-2012-4431](https://github.com/imjdl/CVE-2012-4431) :  ![starts](https://img.shields.io/github/stars/imjdl/CVE-2012-4431.svg) ![forks](https://img.shields.io/github/forks/imjdl/CVE-2012-4431.svg)

## CVE-2012-4220
 diagchar_core.c in the Qualcomm Innovation Center (QuIC) Diagnostics (aka DIAG) kernel-mode driver for Android 2.3 through 4.2 allows attackers to execute arbitrary code or cause a denial of service (incorrect pointer dereference) via an application that uses crafted arguments in a local diagchar_ioctl call.



- [https://github.com/poliva/root-zte-open](https://github.com/poliva/root-zte-open) :  ![starts](https://img.shields.io/github/stars/poliva/root-zte-open.svg) ![forks](https://img.shields.io/github/forks/poliva/root-zte-open.svg)

- [https://github.com/hiikezoe/diaggetroot](https://github.com/hiikezoe/diaggetroot) :  ![starts](https://img.shields.io/github/stars/hiikezoe/diaggetroot.svg) ![forks](https://img.shields.io/github/forks/hiikezoe/diaggetroot.svg)

## CVE-2012-3716
 CoreText in Apple Mac OS X 10.7.x before 10.7.5 allows remote attackers to execute arbitrary code or cause a denial of service (out-of-bounds write or read) via a crafted text glyph.



- [https://github.com/d4rkcat/killosx](https://github.com/d4rkcat/killosx) :  ![starts](https://img.shields.io/github/stars/d4rkcat/killosx.svg) ![forks](https://img.shields.io/github/forks/d4rkcat/killosx.svg)

## CVE-2012-3576
 Unrestricted file upload vulnerability in php/upload.php in the wpStoreCart plugin before 2.5.30 for WordPress allows remote attackers to execute arbitrary code by uploading a file with an executable extension, then accessing it via a direct request to the file in uploads/wpstorecart.



- [https://github.com/Ydvmtzv/wpstorecart-exploit](https://github.com/Ydvmtzv/wpstorecart-exploit) :  ![starts](https://img.shields.io/github/stars/Ydvmtzv/wpstorecart-exploit.svg) ![forks](https://img.shields.io/github/forks/Ydvmtzv/wpstorecart-exploit.svg)

## CVE-2012-3452
 gnome-screensaver 3.4.x before 3.4.4 and 3.5.x before 3.5.4, when multiple screens are used, only locks the screen with the active focus, which allows physically proximate attackers to bypass screen locking and access an unattended workstation.



- [https://github.com/sh7alward/CVE-20121-34527-nightmare](https://github.com/sh7alward/CVE-20121-34527-nightmare) :  ![starts](https://img.shields.io/github/stars/sh7alward/CVE-20121-34527-nightmare.svg) ![forks](https://img.shields.io/github/forks/sh7alward/CVE-20121-34527-nightmare.svg)

## CVE-2012-3153
 Unspecified vulnerability in the Oracle Reports Developer component in Oracle Fusion Middleware 11.1.1.4, 11.1.1.6, and 11.1.2.0 allows remote attackers to affect confidentiality and integrity via unknown vectors related to Servlet.  NOTE: the previous information is from the October 2012 CPU. Oracle has not commented on claims from the original researcher that the PARSEQUERY function allows remote attackers to obtain database credentials via reports/rwservlet/parsequery, and that this issue occurs in earlier versions.  NOTE: this can be leveraged with CVE-2012-3152 to execute arbitrary code by uploading a .jsp file.



- [https://github.com/Mekanismen/pwnacle-fusion](https://github.com/Mekanismen/pwnacle-fusion) :  ![starts](https://img.shields.io/github/stars/Mekanismen/pwnacle-fusion.svg) ![forks](https://img.shields.io/github/forks/Mekanismen/pwnacle-fusion.svg)

## CVE-2012-3152
 Unspecified vulnerability in the Oracle Reports Developer component in Oracle Fusion Middleware 11.1.1.4, 11.1.1.6, and 11.1.2.0 allows remote attackers to affect confidentiality and integrity via unknown vectors related to Report Server Component.  NOTE: the previous information is from the October 2012 CPU. Oracle has not commented on claims from the original researcher that the URLPARAMETER functionality allows remote attackers to read and upload arbitrary files to reports/rwservlet, and that this issue occurs in earlier versions.  NOTE: this can be leveraged with CVE-2012-3153 to execute arbitrary code by uploading a .jsp file.



- [https://github.com/Mekanismen/pwnacle-fusion](https://github.com/Mekanismen/pwnacle-fusion) :  ![starts](https://img.shields.io/github/stars/Mekanismen/pwnacle-fusion.svg) ![forks](https://img.shields.io/github/forks/Mekanismen/pwnacle-fusion.svg)

## CVE-2012-3137
 The authentication protocol in Oracle Database Server 10.2.0.3, 10.2.0.4, 10.2.0.5, 11.1.0.7, 11.2.0.2, and 11.2.0.3 allows remote attackers to obtain the session key and salt for arbitrary users, which leaks information about the cryptographic hash and makes it easier to conduct brute force password guessing attacks, aka "stealth password cracking vulnerability."



- [https://github.com/r1-/cve-2012-3137](https://github.com/r1-/cve-2012-3137) :  ![starts](https://img.shields.io/github/stars/r1-/cve-2012-3137.svg) ![forks](https://img.shields.io/github/forks/r1-/cve-2012-3137.svg)

- [https://github.com/hantwister/o5logon-fetch](https://github.com/hantwister/o5logon-fetch) :  ![starts](https://img.shields.io/github/stars/hantwister/o5logon-fetch.svg) ![forks](https://img.shields.io/github/forks/hantwister/o5logon-fetch.svg)

## CVE-2012-2982
 file/show.cgi in Webmin 1.590 and earlier allows remote authenticated users to execute arbitrary commands via an invalid character in a pathname, as demonstrated by a | (pipe) character.



- [https://github.com/JohnHammond/CVE-2012-2982](https://github.com/JohnHammond/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/JohnHammond/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/JohnHammond/CVE-2012-2982.svg)

- [https://github.com/cd6629/CVE-2012-2982-Python-PoC](https://github.com/cd6629/CVE-2012-2982-Python-PoC) :  ![starts](https://img.shields.io/github/stars/cd6629/CVE-2012-2982-Python-PoC.svg) ![forks](https://img.shields.io/github/forks/cd6629/CVE-2012-2982-Python-PoC.svg)

- [https://github.com/0xTas/CVE-2012-2982](https://github.com/0xTas/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/0xTas/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/0xTas/CVE-2012-2982.svg)

- [https://github.com/OstojaOfficial/CVE-2012-2982](https://github.com/OstojaOfficial/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/OstojaOfficial/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/OstojaOfficial/CVE-2012-2982.svg)

- [https://github.com/Gvmyz/CVE-2012-2982_Python](https://github.com/Gvmyz/CVE-2012-2982_Python) :  ![starts](https://img.shields.io/github/stars/Gvmyz/CVE-2012-2982_Python.svg) ![forks](https://img.shields.io/github/forks/Gvmyz/CVE-2012-2982_Python.svg)

- [https://github.com/Ari-Weinberg/CVE-2012-2982](https://github.com/Ari-Weinberg/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/Ari-Weinberg/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/Ari-Weinberg/CVE-2012-2982.svg)

- [https://github.com/blu3ming/CVE-2012-2982](https://github.com/blu3ming/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/blu3ming/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/blu3ming/CVE-2012-2982.svg)

- [https://github.com/CpyRe/CVE-2012-2982](https://github.com/CpyRe/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/CpyRe/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/CpyRe/CVE-2012-2982.svg)

- [https://github.com/wizardy0ga/CVE_2012-2982](https://github.com/wizardy0ga/CVE_2012-2982) :  ![starts](https://img.shields.io/github/stars/wizardy0ga/CVE_2012-2982.svg) ![forks](https://img.shields.io/github/forks/wizardy0ga/CVE_2012-2982.svg)

- [https://github.com/elliotosama/CVE-2012-2982](https://github.com/elliotosama/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/elliotosama/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/elliotosama/CVE-2012-2982.svg)

- [https://github.com/lpuv/CVE-2012-2982](https://github.com/lpuv/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/lpuv/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/lpuv/CVE-2012-2982.svg)

- [https://github.com/varppi/CVE-2012-2982](https://github.com/varppi/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/varppi/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/varppi/CVE-2012-2982.svg)

- [https://github.com/0xF331-D3AD/CVE-2012-2982](https://github.com/0xF331-D3AD/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/0xF331-D3AD/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/0xF331-D3AD/CVE-2012-2982.svg)

- [https://github.com/boriitoo/CVE-2012-2982](https://github.com/boriitoo/CVE-2012-2982) :  ![starts](https://img.shields.io/github/stars/boriitoo/CVE-2012-2982.svg) ![forks](https://img.shields.io/github/forks/boriitoo/CVE-2012-2982.svg)

- [https://github.com/Shadow-Spinner/CVE-2012-2982_python](https://github.com/Shadow-Spinner/CVE-2012-2982_python) :  ![starts](https://img.shields.io/github/stars/Shadow-Spinner/CVE-2012-2982_python.svg) ![forks](https://img.shields.io/github/forks/Shadow-Spinner/CVE-2012-2982_python.svg)

- [https://github.com/SieGer05/CVE-2012-2982-Webmin-Exploit](https://github.com/SieGer05/CVE-2012-2982-Webmin-Exploit) :  ![starts](https://img.shields.io/github/stars/SieGer05/CVE-2012-2982-Webmin-Exploit.svg) ![forks](https://img.shields.io/github/forks/SieGer05/CVE-2012-2982-Webmin-Exploit.svg)

- [https://github.com/SincIDK/CVE-2012-2982-Exploit-Script](https://github.com/SincIDK/CVE-2012-2982-Exploit-Script) :  ![starts](https://img.shields.io/github/stars/SincIDK/CVE-2012-2982-Exploit-Script.svg) ![forks](https://img.shields.io/github/forks/SincIDK/CVE-2012-2982-Exploit-Script.svg)

## CVE-2012-2688
 Unspecified vulnerability in the _php_stream_scandir function in the stream implementation in PHP before 5.3.15 and 5.4.x before 5.4.5 has unknown impact and remote attack vectors, related to an "overflow."



- [https://github.com/shelld3v/CVE-2012-2688](https://github.com/shelld3v/CVE-2012-2688) :  ![starts](https://img.shields.io/github/stars/shelld3v/CVE-2012-2688.svg) ![forks](https://img.shields.io/github/forks/shelld3v/CVE-2012-2688.svg)

## CVE-2012-2661
 The Active Record component in Ruby on Rails 3.0.x before 3.0.13, 3.1.x before 3.1.5, and 3.2.x before 3.2.4 does not properly implement the passing of request data to a where method in an ActiveRecord class, which allows remote attackers to conduct certain SQL injection attacks via nested query parameters that leverage unintended recursion, a related issue to CVE-2012-2695.



- [https://github.com/r4x0r1337/-CVE-2012-2661-ActiveRecord-SQL-injection-](https://github.com/r4x0r1337/-CVE-2012-2661-ActiveRecord-SQL-injection-) :  ![starts](https://img.shields.io/github/stars/r4x0r1337/-CVE-2012-2661-ActiveRecord-SQL-injection-.svg) ![forks](https://img.shields.io/github/forks/r4x0r1337/-CVE-2012-2661-ActiveRecord-SQL-injection-.svg)

## CVE-2012-2593
 Cross-site scripting (XSS) vulnerability in the administrative interface in Atmail Webmail Server 6.4 allows remote attackers to inject arbitrary web script or HTML via the Date field of an email.



- [https://github.com/AndrewTrube/CVE-2012-2593](https://github.com/AndrewTrube/CVE-2012-2593) :  ![starts](https://img.shields.io/github/stars/AndrewTrube/CVE-2012-2593.svg) ![forks](https://img.shields.io/github/forks/AndrewTrube/CVE-2012-2593.svg)

## CVE-2012-2122
 sql/password.c in Oracle MySQL 5.1.x before 5.1.63, 5.5.x before 5.5.24, and 5.6.x before 5.6.6, and MariaDB 5.1.x before 5.1.62, 5.2.x before 5.2.12, 5.3.x before 5.3.6, and 5.5.x before 5.5.23, when running in certain environments with certain implementations of the memcmp function, allows remote attackers to bypass authentication by repeatedly authenticating with the same incorrect password, which eventually causes a token comparison to succeed due to an improperly-checked return value.



- [https://github.com/Avinza/CVE-2012-2122-scanner](https://github.com/Avinza/CVE-2012-2122-scanner) :  ![starts](https://img.shields.io/github/stars/Avinza/CVE-2012-2122-scanner.svg) ![forks](https://img.shields.io/github/forks/Avinza/CVE-2012-2122-scanner.svg)

- [https://github.com/cyberharsh/Oracle-mysql-CVE-2012-2122](https://github.com/cyberharsh/Oracle-mysql-CVE-2012-2122) :  ![starts](https://img.shields.io/github/stars/cyberharsh/Oracle-mysql-CVE-2012-2122.svg) ![forks](https://img.shields.io/github/forks/cyberharsh/Oracle-mysql-CVE-2012-2122.svg)

- [https://github.com/zhangkaibin0921/CVE-2012-2122](https://github.com/zhangkaibin0921/CVE-2012-2122) :  ![starts](https://img.shields.io/github/stars/zhangkaibin0921/CVE-2012-2122.svg) ![forks](https://img.shields.io/github/forks/zhangkaibin0921/CVE-2012-2122.svg)

- [https://github.com/subinyy/docker_CVE_2012_2122](https://github.com/subinyy/docker_CVE_2012_2122) :  ![starts](https://img.shields.io/github/stars/subinyy/docker_CVE_2012_2122.svg) ![forks](https://img.shields.io/github/forks/subinyy/docker_CVE_2012_2122.svg)

## CVE-2012-1889
 Microsoft XML Core Services 3.0, 4.0, 5.0, and 6.0 accesses uninitialized memory locations, which allows remote attackers to execute arbitrary code or cause a denial of service (memory corruption) via a crafted web site.



- [https://github.com/whu-enjoy/CVE-2012-1889](https://github.com/whu-enjoy/CVE-2012-1889) :  ![starts](https://img.shields.io/github/stars/whu-enjoy/CVE-2012-1889.svg) ![forks](https://img.shields.io/github/forks/whu-enjoy/CVE-2012-1889.svg)

- [https://github.com/l-iberty/cve-2012-1889](https://github.com/l-iberty/cve-2012-1889) :  ![starts](https://img.shields.io/github/stars/l-iberty/cve-2012-1889.svg) ![forks](https://img.shields.io/github/forks/l-iberty/cve-2012-1889.svg)

## CVE-2012-1876
 Microsoft Internet Explorer 6 through 9, and 10 Consumer Preview, does not properly handle objects in memory, which allows remote attackers to execute arbitrary code by attempting to access a nonexistent object, leading to a heap-based buffer overflow, aka "Col Element Remote Code Execution Vulnerability," as demonstrated by VUPEN during a Pwn2Own competition at CanSecWest 2012.



- [https://github.com/WizardVan/CVE-2012-1876](https://github.com/WizardVan/CVE-2012-1876) :  ![starts](https://img.shields.io/github/stars/WizardVan/CVE-2012-1876.svg) ![forks](https://img.shields.io/github/forks/WizardVan/CVE-2012-1876.svg)

- [https://github.com/ExploitCN/CVE-2012-1876-win7_x86_and_win7x64](https://github.com/ExploitCN/CVE-2012-1876-win7_x86_and_win7x64) :  ![starts](https://img.shields.io/github/stars/ExploitCN/CVE-2012-1876-win7_x86_and_win7x64.svg) ![forks](https://img.shields.io/github/forks/ExploitCN/CVE-2012-1876-win7_x86_and_win7x64.svg)

## CVE-2012-1870
 The CBC mode in the TLS protocol, as used in Microsoft Windows XP SP2 and SP3, Windows Server 2003 SP2, Windows Vista SP2, Windows Server 2008 SP2, R2, and R2 SP1, Windows 7 Gold and SP1, and other products, allows remote web servers to obtain plaintext data by triggering multiple requests to a third-party HTTPS server and sniffing the network during the resulting HTTPS session, aka "TLS Protocol Vulnerability."



- [https://github.com/dja2TaqkGEEfA45/CVE-2012-1870](https://github.com/dja2TaqkGEEfA45/CVE-2012-1870) :  ![starts](https://img.shields.io/github/stars/dja2TaqkGEEfA45/CVE-2012-1870.svg) ![forks](https://img.shields.io/github/forks/dja2TaqkGEEfA45/CVE-2012-1870.svg)

## CVE-2012-1831
 Heap-based buffer overflow in WellinTech KingView 6.53 allows remote attackers to execute arbitrary code via a crafted packet to TCP port 555.



- [https://github.com/Astrowmist/POC-CVE-2012-1831](https://github.com/Astrowmist/POC-CVE-2012-1831) :  ![starts](https://img.shields.io/github/stars/Astrowmist/POC-CVE-2012-1831.svg) ![forks](https://img.shields.io/github/forks/Astrowmist/POC-CVE-2012-1831.svg)

## CVE-2012-1823
 sapi/cgi/cgi_main.c in PHP before 5.3.12 and 5.4.x before 5.4.2, when configured as a CGI script (aka php-cgi), does not properly handle query strings that lack an = (equals sign) character, which allows remote attackers to execute arbitrary code by placing command-line options in the query string, related to lack of skipping a certain php_getopt for the 'd' case.



- [https://github.com/0xl0k1/CVE-2012-1823](https://github.com/0xl0k1/CVE-2012-1823) :  ![starts](https://img.shields.io/github/stars/0xl0k1/CVE-2012-1823.svg) ![forks](https://img.shields.io/github/forks/0xl0k1/CVE-2012-1823.svg)

- [https://github.com/tardummy01/oscp_scripts-1](https://github.com/tardummy01/oscp_scripts-1) :  ![starts](https://img.shields.io/github/stars/tardummy01/oscp_scripts-1.svg) ![forks](https://img.shields.io/github/forks/tardummy01/oscp_scripts-1.svg)

- [https://github.com/Unix13/metasploitable2](https://github.com/Unix13/metasploitable2) :  ![starts](https://img.shields.io/github/stars/Unix13/metasploitable2.svg) ![forks](https://img.shields.io/github/forks/Unix13/metasploitable2.svg)

- [https://github.com/drone789/CVE-2012-1823](https://github.com/drone789/CVE-2012-1823) :  ![starts](https://img.shields.io/github/stars/drone789/CVE-2012-1823.svg) ![forks](https://img.shields.io/github/forks/drone789/CVE-2012-1823.svg)

- [https://github.com/cyberharsh/PHP_CVE-2012-1823](https://github.com/cyberharsh/PHP_CVE-2012-1823) :  ![starts](https://img.shields.io/github/stars/cyberharsh/PHP_CVE-2012-1823.svg) ![forks](https://img.shields.io/github/forks/cyberharsh/PHP_CVE-2012-1823.svg)

- [https://github.com/Dmitri131313/CVE-2012-1823-exploit-for-https-user-password-web](https://github.com/Dmitri131313/CVE-2012-1823-exploit-for-https-user-password-web) :  ![starts](https://img.shields.io/github/stars/Dmitri131313/CVE-2012-1823-exploit-for-https-user-password-web.svg) ![forks](https://img.shields.io/github/forks/Dmitri131313/CVE-2012-1823-exploit-for-https-user-password-web.svg)

- [https://github.com/Jimmy01240397/CVE-2012-1823-Analyze](https://github.com/Jimmy01240397/CVE-2012-1823-Analyze) :  ![starts](https://img.shields.io/github/stars/Jimmy01240397/CVE-2012-1823-Analyze.svg) ![forks](https://img.shields.io/github/forks/Jimmy01240397/CVE-2012-1823-Analyze.svg)

## CVE-2012-1723
 Unspecified vulnerability in the Java Runtime Environment (JRE) component in Oracle Java SE 7 update 4 and earlier, 6 update 32 and earlier, 5 update 35 and earlier, and 1.4.2_37 and earlier allows remote attackers to affect confidentiality, integrity, and availability via unknown vectors related to Hotspot.



- [https://github.com/EthanNJC/CVE-2012-1723](https://github.com/EthanNJC/CVE-2012-1723) :  ![starts](https://img.shields.io/github/stars/EthanNJC/CVE-2012-1723.svg) ![forks](https://img.shields.io/github/forks/EthanNJC/CVE-2012-1723.svg)

## CVE-2012-1675
 The TNS Listener, as used in Oracle Database 11g 11.1.0.7, 11.2.0.2, and 11.2.0.3, and 10g 10.2.0.3, 10.2.0.4, and 10.2.0.5, as used in Oracle Fusion Middleware, Enterprise Manager, E-Business Suite, and possibly other products, allows remote attackers to execute arbitrary database commands by performing a remote registration of a database (1) instance or (2) service name that already exists, then conducting a man-in-the-middle (MITM) attack to hijack database connections, aka "TNS Poison."



- [https://github.com/bongbongco/CVE-2012-1675](https://github.com/bongbongco/CVE-2012-1675) :  ![starts](https://img.shields.io/github/stars/bongbongco/CVE-2012-1675.svg) ![forks](https://img.shields.io/github/forks/bongbongco/CVE-2012-1675.svg)

## CVE-2012-1495
 install/index.php in WebCalendar before 1.2.5 allows remote attackers to execute arbitrary code via the form_single_user_login parameter.



- [https://github.com/axelbankole/CVE-2012-1495-Webcalendar-](https://github.com/axelbankole/CVE-2012-1495-Webcalendar-) :  ![starts](https://img.shields.io/github/stars/axelbankole/CVE-2012-1495-Webcalendar-.svg) ![forks](https://img.shields.io/github/forks/axelbankole/CVE-2012-1495-Webcalendar-.svg)

## CVE-2012-0507
 Unspecified vulnerability in the Java Runtime Environment (JRE) component in Oracle Java SE 7 Update 2 and earlier, 6 Update 30 and earlier, and 5.0 Update 33 and earlier allows remote attackers to affect confidentiality, integrity, and availability via unknown vectors related to Concurrency.  NOTE: the previous information was obtained from the February 2012 Oracle CPU. Oracle has not commented on claims from a downstream vendor and third party researchers that this issue occurs because the AtomicReferenceArray class implementation does not ensure that the array is of the Object[] type, which allows attackers to cause a denial of service (JVM crash) or bypass Java sandbox restrictions.  NOTE: this issue was originally mapped to CVE-2011-3571, but that identifier was already assigned to a different issue.



- [https://github.com/frg316/cve2012-0507](https://github.com/frg316/cve2012-0507) :  ![starts](https://img.shields.io/github/stars/frg316/cve2012-0507.svg) ![forks](https://img.shields.io/github/forks/frg316/cve2012-0507.svg)

## CVE-2012-0158
 The (1) ListView, (2) ListView2, (3) TreeView, and (4) TreeView2 ActiveX controls in MSCOMCTL.OCX in the Common Controls in Microsoft Office 2003 SP3, 2007 SP2 and SP3, and 2010 Gold and SP1; Office 2003 Web Components SP3; SQL Server 2000 SP4, 2005 SP4, and 2008 SP2, SP3, and R2; BizTalk Server 2002 SP1; Commerce Server 2002 SP4, 2007 SP2, and 2009 Gold and R2; Visual FoxPro 8.0 SP1 and 9.0 SP2; and Visual Basic 6.0 Runtime allow remote attackers to execute arbitrary code via a crafted (a) web site, (b) Office document, or (c) .rtf file that triggers "system state" corruption, as exploited in the wild in April 2012, aka "MSCOMCTL.OCX RCE Vulnerability."



- [https://github.com/Sunqiz/CVE-2012-0158-reproduction](https://github.com/Sunqiz/CVE-2012-0158-reproduction) :  ![starts](https://img.shields.io/github/stars/Sunqiz/CVE-2012-0158-reproduction.svg) ![forks](https://img.shields.io/github/forks/Sunqiz/CVE-2012-0158-reproduction.svg)

- [https://github.com/RobertoLeonFR-ES/Exploit-Win32.CVE-2012-0158.F.doc](https://github.com/RobertoLeonFR-ES/Exploit-Win32.CVE-2012-0158.F.doc) :  ![starts](https://img.shields.io/github/stars/RobertoLeonFR-ES/Exploit-Win32.CVE-2012-0158.F.doc.svg) ![forks](https://img.shields.io/github/forks/RobertoLeonFR-ES/Exploit-Win32.CVE-2012-0158.F.doc.svg)

## CVE-2012-0152
 The Remote Desktop Protocol (RDP) service in Microsoft Windows Server 2008 R2 and R2 SP1 and Windows 7 Gold and SP1 allows remote attackers to cause a denial of service (application hang) via a series of crafted packets, aka "Terminal Server Denial of Service Vulnerability."



- [https://github.com/anmolksachan/MS12-020](https://github.com/anmolksachan/MS12-020) :  ![starts](https://img.shields.io/github/stars/anmolksachan/MS12-020.svg) ![forks](https://img.shields.io/github/forks/anmolksachan/MS12-020.svg)

- [https://github.com/rutvijjethwa/RDP_jammer](https://github.com/rutvijjethwa/RDP_jammer) :  ![starts](https://img.shields.io/github/stars/rutvijjethwa/RDP_jammer.svg) ![forks](https://img.shields.io/github/forks/rutvijjethwa/RDP_jammer.svg)

## CVE-2012-0056
 The mem_write function in the Linux kernel before 3.2.2, when ASLR is disabled, does not properly check permissions when writing to /proc/pid/mem, which allows local users to gain privileges by modifying process memory, as demonstrated by Mempodipper.



- [https://github.com/pythonone/CVE-2012-0056](https://github.com/pythonone/CVE-2012-0056) :  ![starts](https://img.shields.io/github/stars/pythonone/CVE-2012-0056.svg) ![forks](https://img.shields.io/github/forks/pythonone/CVE-2012-0056.svg)

- [https://github.com/srclib/CVE-2012-0056](https://github.com/srclib/CVE-2012-0056) :  ![starts](https://img.shields.io/github/stars/srclib/CVE-2012-0056.svg) ![forks](https://img.shields.io/github/forks/srclib/CVE-2012-0056.svg)

## CVE-2012-0003
 Unspecified vulnerability in winmm.dll in Windows Multimedia Library in Windows Media Player (WMP) in Microsoft Windows XP SP2 and SP3, Server 2003 SP2, Vista SP2, and Server 2008 SP2 allows remote attackers to execute arbitrary code via a crafted MIDI file, aka "MIDI Remote Code Execution Vulnerability."



- [https://github.com/k0keoyo/CVE-2012-0003_eXP](https://github.com/k0keoyo/CVE-2012-0003_eXP) :  ![starts](https://img.shields.io/github/stars/k0keoyo/CVE-2012-0003_eXP.svg) ![forks](https://img.shields.io/github/forks/k0keoyo/CVE-2012-0003_eXP.svg)

- [https://github.com/chefphenix25/vuln-rabilit-windows7](https://github.com/chefphenix25/vuln-rabilit-windows7) :  ![starts](https://img.shields.io/github/stars/chefphenix25/vuln-rabilit-windows7.svg) ![forks](https://img.shields.io/github/forks/chefphenix25/vuln-rabilit-windows7.svg)

## CVE-2012-0002
 The Remote Desktop Protocol (RDP) implementation in Microsoft Windows XP SP2 and SP3, Windows Server 2003 SP2, Windows Vista SP2, Windows Server 2008 SP2, R2, and R2 SP1, and Windows 7 Gold and SP1 does not properly process packets in memory, which allows remote attackers to execute arbitrary code by sending crafted RDP packets triggering access to an object that (1) was not properly initialized or (2) is deleted, aka "Remote Desktop Protocol Vulnerability."



- [https://github.com/zhangkaibin0921/MS12-020-CVE-2012-0002](https://github.com/zhangkaibin0921/MS12-020-CVE-2012-0002) :  ![starts](https://img.shields.io/github/stars/zhangkaibin0921/MS12-020-CVE-2012-0002.svg) ![forks](https://img.shields.io/github/forks/zhangkaibin0921/MS12-020-CVE-2012-0002.svg)
