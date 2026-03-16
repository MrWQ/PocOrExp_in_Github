# Update 2026-03-16
## CVE-2026-31802
 node-tar is a full-featured Tar for Node.js. Prior to version 7.5.11, tar (npm) can be tricked into creating a symlink that points outside the extraction directory by using a drive-relative symlink target such as C:../../../target.txt, which enables file overwrite outside cwd during normal tar.x() extraction. This vulnerability is fixed in 7.5.11.

- [https://github.com/Jvr2022/CVE-2026-31802](https://github.com/Jvr2022/CVE-2026-31802) :  ![starts](https://img.shields.io/github/stars/Jvr2022/CVE-2026-31802.svg) ![forks](https://img.shields.io/github/forks/Jvr2022/CVE-2026-31802.svg)


## CVE-2026-29000
 pac4j-jwt versions prior to 4.5.9, 5.7.9, and 6.3.3 contain an authentication bypass vulnerability in JwtAuthenticator when processing encrypted JWTs that allows remote attackers to forge authentication tokens. Attackers who possess the server's RSA public key can create a JWE-wrapped PlainJWT with arbitrary subject and role claims, bypassing signature verification to authenticate as any user including administrators.

- [https://github.com/FranzAlvis/Cve_2026_29000_exploit](https://github.com/FranzAlvis/Cve_2026_29000_exploit) :  ![starts](https://img.shields.io/github/stars/FranzAlvis/Cve_2026_29000_exploit.svg) ![forks](https://img.shields.io/github/forks/FranzAlvis/Cve_2026_29000_exploit.svg)


## CVE-2026-27944
 Nginx UI is a web user interface for the Nginx web server. Prior to version 2.3.3, the /api/backup endpoint is accessible without authentication and discloses the encryption keys required to decrypt the backup in the X-Backup-Security response header. This allows an unauthenticated attacker to download a full system backup containing sensitive data (user credentials, session tokens, SSL private keys, Nginx configurations) and decrypt it immediately. This issue has been patched in version 2.3.3.

- [https://github.com/Skynoxk/CVE-2026-27944](https://github.com/Skynoxk/CVE-2026-27944) :  ![starts](https://img.shields.io/github/stars/Skynoxk/CVE-2026-27944.svg) ![forks](https://img.shields.io/github/forks/Skynoxk/CVE-2026-27944.svg)


## CVE-2026-26117
 Authentication bypass using an alternate path or channel in Azure Windows Virtual Machine Agent allows an authorized attacker to elevate privileges locally.

- [https://github.com/j-dahl7/arc-cloud-c2-sentinel](https://github.com/j-dahl7/arc-cloud-c2-sentinel) :  ![starts](https://img.shields.io/github/stars/j-dahl7/arc-cloud-c2-sentinel.svg) ![forks](https://img.shields.io/github/forks/j-dahl7/arc-cloud-c2-sentinel.svg)


## CVE-2026-25177
 Improper restriction of names for files and other resources in Active Directory Domain Services allows an authorized attacker to elevate privileges over a network.

- [https://github.com/danaug23/detect_CVE-2026-25177](https://github.com/danaug23/detect_CVE-2026-25177) :  ![starts](https://img.shields.io/github/stars/danaug23/detect_CVE-2026-25177.svg) ![forks](https://img.shields.io/github/forks/danaug23/detect_CVE-2026-25177.svg)


## CVE-2026-4092
 Path Traversal in Clasp impacting versions  3.2.0 allows a remote attacker to perform remote code execution via a malicious Google Apps Script project containing specially crafted filenames with directory traversal sequences.

- [https://github.com/g0w6y/CVE-2026-4092](https://github.com/g0w6y/CVE-2026-4092) :  ![starts](https://img.shields.io/github/stars/g0w6y/CVE-2026-4092.svg) ![forks](https://img.shields.io/github/forks/g0w6y/CVE-2026-4092.svg)


## CVE-2026-1312
Django would like to thank Solomon Kebede for reporting this issue.

- [https://github.com/sw0rd1ight/CVE-2026-1312](https://github.com/sw0rd1ight/CVE-2026-1312) :  ![starts](https://img.shields.io/github/stars/sw0rd1ight/CVE-2026-1312.svg) ![forks](https://img.shields.io/github/forks/sw0rd1ight/CVE-2026-1312.svg)


## CVE-2025-68926
 RustFS is a distributed object storage system built in Rust. In versions prior to 1.0.0-alpha.78, RustFS implements gRPC authentication using a hardcoded static token `"rustfs rpc"` that is publicly exposed in the source code repository, hardcoded on both client and server sides, non-configurable with no mechanism for token rotation, and universally valid across all RustFS deployments. Any attacker with network access to the gRPC port can authenticate using this publicly known token and execute privileged operations including data destruction, policy manipulation, and cluster configuration changes. Version 1.0.0-alpha.78 contains a fix for the issue.

- [https://github.com/materaj2/CVE-2025-68926-repo](https://github.com/materaj2/CVE-2025-68926-repo) :  ![starts](https://img.shields.io/github/stars/materaj2/CVE-2025-68926-repo.svg) ![forks](https://img.shields.io/github/forks/materaj2/CVE-2025-68926-repo.svg)


## CVE-2025-60787
 MotionEye v0.43.1b4 and before is vulnerable to OS Command Injection in configuration parameters such as image_file_name. Unsanitized user input is written to Motion configuration files, allowing remote authenticated attackers with admin access to achieve code execution when Motion is restarted.

- [https://github.com/agent-skywalker/CVE-2025-60787](https://github.com/agent-skywalker/CVE-2025-60787) :  ![starts](https://img.shields.io/github/stars/agent-skywalker/CVE-2025-60787.svg) ![forks](https://img.shields.io/github/forks/agent-skywalker/CVE-2025-60787.svg)


## CVE-2025-60690
 A stack-based buffer overflow exists in the get_merge_ipaddr function of the httpd binary on Linksys E1200 v2 routers (Firmware E1200_v2.0.11.001_us.tar.gz). The function concatenates up to four user-supplied CGI parameters matching parameter_0~3 into a fixed-size buffer (a2) without bounds checking. Remote attackers can exploit this vulnerability via specially crafted HTTP requests to execute arbitrary code or cause denial of service without authentication.

- [https://github.com/Jarrettgohxz/CVE-research](https://github.com/Jarrettgohxz/CVE-research) :  ![starts](https://img.shields.io/github/stars/Jarrettgohxz/CVE-research.svg) ![forks](https://img.shields.io/github/forks/Jarrettgohxz/CVE-research.svg)


## CVE-2025-56399
 alexusmai laravel-file-manager 3.3.1 and before allows an authenticated attacker to achieve Remote Code Execution (RCE) through a crafted file upload. A file with a '.png` extension containing PHP code can be uploaded via the file manager interface. Although the upload appears to fail client-side validation, the file is still saved on the server. The attacker can then use the rename API to change the file extension to `.php`, and upon accessing it via a public URL, the server executes the embedded code.

- [https://github.com/im-hanzou/CVE-2025-56399](https://github.com/im-hanzou/CVE-2025-56399) :  ![starts](https://img.shields.io/github/stars/im-hanzou/CVE-2025-56399.svg) ![forks](https://img.shields.io/github/forks/im-hanzou/CVE-2025-56399.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/Heimd411/CVE-2025-29927-PoC](https://github.com/Heimd411/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/Heimd411/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/Heimd411/CVE-2025-29927-PoC.svg)


## CVE-2025-15467
OpenSSL 1.1.1 and 1.0.2 are not affected by this issue.

- [https://github.com/materaj2/cve-2025-15467](https://github.com/materaj2/cve-2025-15467) :  ![starts](https://img.shields.io/github/stars/materaj2/cve-2025-15467.svg) ![forks](https://img.shields.io/github/forks/materaj2/cve-2025-15467.svg)


## CVE-2025-5548
 A vulnerability, which was classified as critical, was found in FreeFloat FTP Server 1.0. Affected is an unknown function of the component NOOP Command Handler. The manipulation leads to buffer overflow. It is possible to launch the attack remotely. The exploit has been disclosed to the public and may be used.

- [https://github.com/alfa8sa/CVE-2025-5548](https://github.com/alfa8sa/CVE-2025-5548) :  ![starts](https://img.shields.io/github/stars/alfa8sa/CVE-2025-5548.svg) ![forks](https://img.shields.io/github/forks/alfa8sa/CVE-2025-5548.svg)
- [https://github.com/celiagomezserra/CVE-2025-5548](https://github.com/celiagomezserra/CVE-2025-5548) :  ![starts](https://img.shields.io/github/stars/celiagomezserra/CVE-2025-5548.svg) ![forks](https://img.shields.io/github/forks/celiagomezserra/CVE-2025-5548.svg)
- [https://github.com/ZoneToolsCiber/Explotando-FreeFloatFTP-CVE-2025-5548](https://github.com/ZoneToolsCiber/Explotando-FreeFloatFTP-CVE-2025-5548) :  ![starts](https://img.shields.io/github/stars/ZoneToolsCiber/Explotando-FreeFloatFTP-CVE-2025-5548.svg) ![forks](https://img.shields.io/github/forks/ZoneToolsCiber/Explotando-FreeFloatFTP-CVE-2025-5548.svg)


## CVE-2025-4517
Note that none of these vulnerabilities significantly affect the installation of source distributions which are tar archives as source distributions already allow arbitrary code execution during the build process. However when evaluating source distributions it's important to avoid installing source distributions with suspicious links.

- [https://github.com/AzureADTrent/CVE-2025-4517-POC](https://github.com/AzureADTrent/CVE-2025-4517-POC) :  ![starts](https://img.shields.io/github/stars/AzureADTrent/CVE-2025-4517-POC.svg) ![forks](https://img.shields.io/github/forks/AzureADTrent/CVE-2025-4517-POC.svg)


## CVE-2024-23897
 Jenkins 2.441 and earlier, LTS 2.426.2 and earlier does not disable a feature of its CLI command parser that replaces an '@' character followed by a file path in an argument with the file's contents, allowing unauthenticated attackers to read arbitrary files on the Jenkins controller file system.

- [https://github.com/classic130/CVE-2024-23897-Jenkins-4.441](https://github.com/classic130/CVE-2024-23897-Jenkins-4.441) :  ![starts](https://img.shields.io/github/stars/classic130/CVE-2024-23897-Jenkins-4.441.svg) ![forks](https://img.shields.io/github/forks/classic130/CVE-2024-23897-Jenkins-4.441.svg)


## CVE-2024-8198
 Heap buffer overflow in Skia in Google Chrome prior to 128.0.6613.113 allowed a remote attacker who had compromised the renderer process to potentially exploit heap corruption via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/HyHy100/Chrome-Skia-CVE-2024-8198](https://github.com/HyHy100/Chrome-Skia-CVE-2024-8198) :  ![starts](https://img.shields.io/github/stars/HyHy100/Chrome-Skia-CVE-2024-8198.svg) ![forks](https://img.shields.io/github/forks/HyHy100/Chrome-Skia-CVE-2024-8198.svg)


## CVE-2024-8118
 In Grafana, the wrong permission is applied to the alert rule write API endpoint, allowing users with permission to write external alert instances to also write alert rules.

- [https://github.com/nurarifin05/POC-CVE-2024-8118](https://github.com/nurarifin05/POC-CVE-2024-8118) :  ![starts](https://img.shields.io/github/stars/nurarifin05/POC-CVE-2024-8118.svg) ![forks](https://img.shields.io/github/forks/nurarifin05/POC-CVE-2024-8118.svg)


## CVE-2023-46604
which fixes this issue.

- [https://github.com/sangrok-jeon/CVE-2023-46604-Analysis](https://github.com/sangrok-jeon/CVE-2023-46604-Analysis) :  ![starts](https://img.shields.io/github/stars/sangrok-jeon/CVE-2023-46604-Analysis.svg) ![forks](https://img.shields.io/github/forks/sangrok-jeon/CVE-2023-46604-Analysis.svg)


## CVE-2023-27524
Alternatively you can set it with `SUPERSET_SECRET_KEY` environment variable.

- [https://github.com/sumaiyafathima-code/CVE-2023-27524](https://github.com/sumaiyafathima-code/CVE-2023-27524) :  ![starts](https://img.shields.io/github/stars/sumaiyafathima-code/CVE-2023-27524.svg) ![forks](https://img.shields.io/github/forks/sumaiyafathima-code/CVE-2023-27524.svg)


## CVE-2022-31630
 In PHP versions prior to 7.4.33, 8.0.25 and 8.1.12, when using imageloadfont() function in gd extension, it is possible to supply a specially crafted font file, such as if the loaded font is used with imagechar() function, the read outside allocated buffer will be used. This can lead to crashes or disclosure of confidential information. 

- [https://github.com/sepkascurty-cpu/php-exploit_cve-2022-31630](https://github.com/sepkascurty-cpu/php-exploit_cve-2022-31630) :  ![starts](https://img.shields.io/github/stars/sepkascurty-cpu/php-exploit_cve-2022-31630.svg) ![forks](https://img.shields.io/github/forks/sepkascurty-cpu/php-exploit_cve-2022-31630.svg)
- [https://github.com/sepkascurty-cpu/CVE-2022-31630---Proof-of-Concept-Exploit-untuk-PHP-7.4.33](https://github.com/sepkascurty-cpu/CVE-2022-31630---Proof-of-Concept-Exploit-untuk-PHP-7.4.33) :  ![starts](https://img.shields.io/github/stars/sepkascurty-cpu/CVE-2022-31630---Proof-of-Concept-Exploit-untuk-PHP-7.4.33.svg) ![forks](https://img.shields.io/github/forks/sepkascurty-cpu/CVE-2022-31630---Proof-of-Concept-Exploit-untuk-PHP-7.4.33.svg)


## CVE-2022-2585
 It was discovered that when exec'ing from a non-leader thread, armed POSIX CPU timers would be left on a list but freed, leading to a use-after-free.

- [https://github.com/pirenga/2022-LPE-UAF](https://github.com/pirenga/2022-LPE-UAF) :  ![starts](https://img.shields.io/github/stars/pirenga/2022-LPE-UAF.svg) ![forks](https://img.shields.io/github/forks/pirenga/2022-LPE-UAF.svg)
- [https://github.com/konoha279/2022-LPE-UAF](https://github.com/konoha279/2022-LPE-UAF) :  ![starts](https://img.shields.io/github/stars/konoha279/2022-LPE-UAF.svg) ![forks](https://img.shields.io/github/forks/konoha279/2022-LPE-UAF.svg)


## CVE-2020-15099
 In TYPO3 CMS greater than or equal to 9.0.0 and less than 9.5.20, and greater than or equal to 10.0.0 and less than 10.4.6, in a case where an attacker manages to generate a valid cryptographic message authentication code (HMAC-SHA1) - either by using a different existing vulnerability or in case the internal encryptionKey was exposed - it is possible to retrieve arbitrary files of a TYPO3 installation. This includes the possibility to fetch typo3conf/LocalConfiguration.php, which again contains the encryptionKey as well as credentials of the database management system being used. In case a database server is directly accessible either via internet or in a shared hosting network, this allows the ability to completely retrieve, manipulate or delete database contents. This includes creating an administration user account - which can be used to trigger remote code execution by injecting custom extensions. This has been patched in versions 9.5.20 and 10.4.6.

- [https://github.com/StillSoul/CVE-2020-15099](https://github.com/StillSoul/CVE-2020-15099) :  ![starts](https://img.shields.io/github/stars/StillSoul/CVE-2020-15099.svg) ![forks](https://img.shields.io/github/forks/StillSoul/CVE-2020-15099.svg)


## CVE-2019-1253
 An elevation of privilege vulnerability exists when the Windows AppX Deployment Server improperly handles junctions.To exploit this vulnerability, an attacker would first have to gain execution on the victim system, aka 'Windows Elevation of Privilege Vulnerability'. This CVE ID is unique from CVE-2019-1215, CVE-2019-1278, CVE-2019-1303.

- [https://github.com/padovah4ck/CVE-2019-1253](https://github.com/padovah4ck/CVE-2019-1253) :  ![starts](https://img.shields.io/github/stars/padovah4ck/CVE-2019-1253.svg) ![forks](https://img.shields.io/github/forks/padovah4ck/CVE-2019-1253.svg)
- [https://github.com/rogue-kdc/CVE-2019-1253](https://github.com/rogue-kdc/CVE-2019-1253) :  ![starts](https://img.shields.io/github/stars/rogue-kdc/CVE-2019-1253.svg) ![forks](https://img.shields.io/github/forks/rogue-kdc/CVE-2019-1253.svg)
- [https://github.com/sgabe/CVE-2019-1253](https://github.com/sgabe/CVE-2019-1253) :  ![starts](https://img.shields.io/github/stars/sgabe/CVE-2019-1253.svg) ![forks](https://img.shields.io/github/forks/sgabe/CVE-2019-1253.svg)
- [https://github.com/offsec-ttps/CVE2019-1253-Compiled](https://github.com/offsec-ttps/CVE2019-1253-Compiled) :  ![starts](https://img.shields.io/github/stars/offsec-ttps/CVE2019-1253-Compiled.svg) ![forks](https://img.shields.io/github/forks/offsec-ttps/CVE2019-1253-Compiled.svg)
- [https://github.com/likekabin/CVE-2019-1253](https://github.com/likekabin/CVE-2019-1253) :  ![starts](https://img.shields.io/github/stars/likekabin/CVE-2019-1253.svg) ![forks](https://img.shields.io/github/forks/likekabin/CVE-2019-1253.svg)


## CVE-2017-1000487
 Plexus-utils before 3.0.16 is vulnerable to command injection because it does not correctly process the contents of double quoted strings.

- [https://github.com/dawetmaster/CVE-2017-1000487-plexus-utils-vulnerable](https://github.com/dawetmaster/CVE-2017-1000487-plexus-utils-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-1000487-plexus-utils-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-1000487-plexus-utils-vulnerable.svg)


## CVE-2017-1000209
 The Java WebSocket client nv-websocket-client does not verify that the server hostname matches a domain name in the subject's Common Name (CN) or subjectAltName field of the X.509 certificate, which allows man-in-the-middle attackers to spoof SSL/TLS servers via an arbitrary valid certificate.

- [https://github.com/dawetmaster/CVE-2017-1000209-nv-websocket-client-vulnerable](https://github.com/dawetmaster/CVE-2017-1000209-nv-websocket-client-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-1000209-nv-websocket-client-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-1000209-nv-websocket-client-vulnerable.svg)


## CVE-2017-1000208
 A vulnerability in Swagger-Parser's (version = 1.0.30) yaml parsing functionality results in arbitrary code being executed when a maliciously crafted yaml Open-API specification is parsed. This in particular, affects the 'generate' and 'validate' command in swagger-codegen (= 2.2.2) and can lead to arbitrary code being executed when these commands are used on a well-crafted yaml specification.

- [https://github.com/dawetmaster/CVE-2017-1000208-swagger-parser-vulnerable](https://github.com/dawetmaster/CVE-2017-1000208-swagger-parser-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-1000208-swagger-parser-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-1000208-swagger-parser-vulnerable.svg)


## CVE-2017-1000207
 A vulnerability in Swagger-Parser's version = 1.0.30 and Swagger codegen version = 2.2.2 yaml parsing functionality results in arbitrary code being executed when a maliciously crafted yaml Open-API specification is parsed. This in particular, affects the 'generate' and 'validate' command in swagger-codegen (= 2.2.2) and can lead to arbitrary code being executed when these commands are used on a well-crafted yaml specification.

- [https://github.com/dawetmaster/CVE-2017-1000207-swagger-parser-vulnerable](https://github.com/dawetmaster/CVE-2017-1000207-swagger-parser-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-1000207-swagger-parser-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-1000207-swagger-parser-vulnerable.svg)


## CVE-2017-18640
 The Alias feature in SnakeYAML before 1.26 allows entity expansion during a load operation, a related issue to CVE-2003-1564.

- [https://github.com/dawetmaster/CVE-2017-18640-snakeyaml-vulnerable](https://github.com/dawetmaster/CVE-2017-18640-snakeyaml-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-18640-snakeyaml-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-18640-snakeyaml-vulnerable.svg)


## CVE-2017-17485
 FasterXML jackson-databind through 2.8.10 and 2.9.x through 2.9.3 allows unauthenticated remote code execution because of an incomplete fix for the CVE-2017-7525 deserialization flaw. This is exploitable by sending maliciously crafted JSON input to the readValue method of the ObjectMapper, bypassing a blacklist that is ineffective if the Spring libraries are available in the classpath.

- [https://github.com/dawetmaster/CVE-2017-17485-jackson-databind-vulnerable](https://github.com/dawetmaster/CVE-2017-17485-jackson-databind-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-17485-jackson-databind-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-17485-jackson-databind-vulnerable.svg)


## CVE-2017-15717
 A flaw in the way URLs are escaped and encoded in the org.apache.sling.xss.impl.XSSAPIImpl#getValidHref and org.apache.sling.xss.impl.XSSFilterImpl#isValidHref allows special crafted URLs to pass as valid, although they carry XSS payloads. The affected versions are Apache Sling XSS Protection API 1.0.4 to 1.0.18, Apache Sling XSS Protection API Compat 1.1.0 and Apache Sling XSS Protection API 2.0.0.

- [https://github.com/dawetmaster/CVE-2017-15717-sling-org-apache-sling-xss-vulnerable](https://github.com/dawetmaster/CVE-2017-15717-sling-org-apache-sling-xss-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-15717-sling-org-apache-sling-xss-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-15717-sling-org-apache-sling-xss-vulnerable.svg)


## CVE-2017-15700
 A flaw in the org.apache.sling.auth.core.AuthUtil#isRedirectValid method in Apache Sling Authentication Service 1.4.0 allows an attacker, through the Sling login form, to trick a victim to send over their credentials.

- [https://github.com/dawetmaster/CVE-2017-15700-sling-org-apache-sling-auth-core-vulnerable](https://github.com/dawetmaster/CVE-2017-15700-sling-org-apache-sling-auth-core-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-15700-sling-org-apache-sling-auth-core-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-15700-sling-org-apache-sling-auth-core-vulnerable.svg)


## CVE-2017-15095
 A deserialization flaw was discovered in the jackson-databind in versions before 2.8.10 and 2.9.1, which could allow an unauthenticated user to perform code execution by sending the maliciously crafted input to the readValue method of the ObjectMapper. This issue extends the previous flaw CVE-2017-7525 by blacklisting more classes that could be used maliciously.

- [https://github.com/dawetmaster/CVE-2017-15095-jackson-databind-vulnerable](https://github.com/dawetmaster/CVE-2017-15095-jackson-databind-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-15095-jackson-databind-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-15095-jackson-databind-vulnerable.svg)


## CVE-2017-14063
 Async Http Client (aka async-http-client) before 2.0.35 can be tricked into connecting to a host different from the one extracted by java.net.URI if a '?' character occurs in a fragment identifier. Similar bugs were previously identified in cURL (CVE-2016-8624) and Oracle Java 8 java.net.URL.

- [https://github.com/dawetmaster/CVE-2017-14063-async-http-client-vulnerable](https://github.com/dawetmaster/CVE-2017-14063-async-http-client-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-14063-async-http-client-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-14063-async-http-client-vulnerable.svg)


## CVE-2017-12197
 It was found that libpam4j up to and including 1.8 did not properly validate user accounts when authenticating. A user with a valid password for a disabled account would be able to bypass security restrictions and possibly access sensitive information.

- [https://github.com/dawetmaster/CVE-2017-12197-libpam4j-vulnerable](https://github.com/dawetmaster/CVE-2017-12197-libpam4j-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-12197-libpam4j-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-12197-libpam4j-vulnerable.svg)


## CVE-2017-12165
 It was discovered that Undertow before 1.4.17, 1.3.31 and 2.0.0 processes http request headers with unusual whitespaces which can cause possible http request smuggling.

- [https://github.com/dawetmaster/CVE-2017-12165-undertow-vulnerable](https://github.com/dawetmaster/CVE-2017-12165-undertow-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-12165-undertow-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-12165-undertow-vulnerable.svg)


## CVE-2017-9801
 When a call-site passes a subject for an email that contains line-breaks in Apache Commons Email 1.0 through 1.4, the caller can add arbitrary SMTP headers.

- [https://github.com/dawetmaster/CVE-2017-9801-commons-email-vulnerable](https://github.com/dawetmaster/CVE-2017-9801-commons-email-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-9801-commons-email-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-9801-commons-email-vulnerable.svg)


## CVE-2017-9798
 Apache httpd allows remote attackers to read secret data from process memory if the Limit directive can be set in a user's .htaccess file, or if httpd.conf has certain misconfigurations, aka Optionsbleed. This affects the Apache HTTP Server through 2.2.34 and 2.4.x through 2.4.27. The attacker sends an unauthenticated OPTIONS HTTP request when attempting to read secret data. This is a use-after-free issue and thus secret data is not always sent, and the specific data depends on many factors including configuration. Exploitation with .htaccess can be blocked with a patch to the ap_limit_section function in server/core.c.

- [https://github.com/suli99/options-scanner](https://github.com/suli99/options-scanner) :  ![starts](https://img.shields.io/github/stars/suli99/options-scanner.svg) ![forks](https://img.shields.io/github/forks/suli99/options-scanner.svg)


## CVE-2017-7957
 XStream through 1.4.9, when a certain denyTypes workaround is not used, mishandles attempts to create an instance of the primitive type 'void' during unmarshalling, leading to a remote application crash, as demonstrated by an xstream.fromXML("void/") call.

- [https://github.com/dawetmaster/CVE-2017-7957-xstream-vulnerable](https://github.com/dawetmaster/CVE-2017-7957-xstream-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-7957-xstream-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-7957-xstream-vulnerable.svg)


## CVE-2017-7662
 Apache CXF Fediz ships with an OpenId Connect (OIDC) service which has a Client Registration Service, which is a simple web application that allows clients to be created, deleted, etc. A CSRF (Cross Style Request Forgery) style vulnerability has been found in this web application in Apache CXF Fediz prior to 1.4.0 and 1.3.2, meaning that a malicious web application could create new clients, or reset secrets, etc, after the admin user has logged on to the client registration service and the session is still active.

- [https://github.com/dawetmaster/CVE-2017-7662-cxf-fediz-vulnerable](https://github.com/dawetmaster/CVE-2017-7662-cxf-fediz-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-7662-cxf-fediz-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-7662-cxf-fediz-vulnerable.svg)


## CVE-2017-7661
 Apache CXF Fediz ships with a number of container-specific plugins to enable WS-Federation for applications. A CSRF (Cross Style Request Forgery) style vulnerability has been found in the Spring 2, Spring 3, Jetty 8 and Jetty 9 plugins in Apache CXF Fediz prior to 1.4.0, 1.3.2 and 1.2.4.

- [https://github.com/dawetmaster/CVE-2017-7661-cxf-fediz-vulnerable](https://github.com/dawetmaster/CVE-2017-7661-cxf-fediz-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-7661-cxf-fediz-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-7661-cxf-fediz-vulnerable.svg)


## CVE-2017-7561
 Red Hat JBoss EAP version 3.0.7 through before 4.0.0.Beta1 is vulnerable to a server-side cache poisoning or CORS requests in the JAX-RS component resulting in a moderate impact.

- [https://github.com/dawetmaster/CVE-2017-7561-Resteasy-vulnerable](https://github.com/dawetmaster/CVE-2017-7561-Resteasy-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-7561-Resteasy-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-7561-Resteasy-vulnerable.svg)


## CVE-2017-7559
 In Undertow 2.x before 2.0.0.Alpha2, 1.4.x before 1.4.17.Final, and 1.3.x before 1.3.31.Final, it was found that the fix for CVE-2017-2666 was incomplete and invalid characters are still allowed in the query string and path parameters. This could be exploited, in conjunction with a proxy that also permitted the invalid characters but with a different interpretation, to inject data into the HTTP response. By manipulating the HTTP response the attacker could poison a web-cache, perform an XSS attack, or obtain sensitive information from requests other than their own.

- [https://github.com/dawetmaster/CVE-2017-7559-undertow-vulnerable](https://github.com/dawetmaster/CVE-2017-7559-undertow-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-7559-undertow-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-7559-undertow-vulnerable.svg)


## CVE-2017-5929
 QOS.ch Logback before 1.2.0 has a serialization vulnerability affecting the SocketServer and ServerSocketReceiver components.

- [https://github.com/dawetmaster/CVE-2017-5929-logback-vulnerable](https://github.com/dawetmaster/CVE-2017-5929-logback-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-5929-logback-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-5929-logback-vulnerable.svg)


## CVE-2017-2666
 It was discovered in Undertow that the code that parsed the HTTP request line permitted invalid characters. This could be exploited, in conjunction with a proxy that also permitted the invalid characters but with a different interpretation, to inject data into the HTTP response. By manipulating the HTTP response the attacker could poison a web-cache, perform an XSS attack, or obtain sensitive information from requests other than their own.

- [https://github.com/dawetmaster/CVE-2017-2666-undertow-vulnerable](https://github.com/dawetmaster/CVE-2017-2666-undertow-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-2666-undertow-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-2666-undertow-vulnerable.svg)


## CVE-2017-2649
 It was found that the Active Directory Plugin for Jenkins up to and including version 2.2 did not verify certificates of the Active Directory server, thereby enabling Man-in-the-Middle attacks.

- [https://github.com/dawetmaster/CVE-2017-2649-active-directory-plugin-vulnerable](https://github.com/dawetmaster/CVE-2017-2649-active-directory-plugin-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2017-2649-active-directory-plugin-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2017-2649-active-directory-plugin-vulnerable.svg)


## CVE-2016-1000031
 Apache Commons FileUpload before 1.3.3 DiskFileItem File Manipulation Remote Code Execution

- [https://github.com/dawetmaster/CVE-2016-1000031-commons-fileupload-vulnerable](https://github.com/dawetmaster/CVE-2016-1000031-commons-fileupload-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-1000031-commons-fileupload-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-1000031-commons-fileupload-vulnerable.svg)


## CVE-2016-9606
 JBoss RESTEasy before version 3.1.2 could be forced into parsing a request with YamlProvider, resulting in unmarshalling of potentially untrusted data which could allow an attacker to execute arbitrary code with RESTEasy application permissions.

- [https://github.com/dawetmaster/CVE-2016-9606-Resteasy-vulnerable](https://github.com/dawetmaster/CVE-2016-9606-Resteasy-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-9606-Resteasy-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-9606-Resteasy-vulnerable.svg)


## CVE-2016-9589
 Undertow in Red Hat wildfly before version 11.0.0.Beta1 is vulnerable to a resource exhaustion resulting in a denial of service. Undertow keeps a cache of seen HTTP headers in persistent connections. It was found that this cache can easily exploited to fill memory with garbage, up to "max-headers" (default 200) * "max-header-size" (default 1MB) per active TCP connection.

- [https://github.com/dawetmaster/CVE-2016-9589-undertow-vulnerable](https://github.com/dawetmaster/CVE-2016-9589-undertow-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-9589-undertow-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-9589-undertow-vulnerable.svg)


## CVE-2016-9177
 Directory traversal vulnerability in Spark 2.5 allows remote attackers to read arbitrary files via a .. (dot dot) in the URI.

- [https://github.com/dawetmaster/CVE-2016-9177-perwendel-spark-vulnerable](https://github.com/dawetmaster/CVE-2016-9177-perwendel-spark-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-9177-perwendel-spark-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-9177-perwendel-spark-vulnerable.svg)


## CVE-2016-8744
 Apache Brooklyn uses the SnakeYAML library for parsing YAML inputs. SnakeYAML allows the use of YAML tags to indicate that SnakeYAML should unmarshal data to a Java type. In the default configuration in Brooklyn before 0.10.0, SnakeYAML will allow unmarshalling to any Java type available on the classpath. This could provide an authenticated user with a means to cause the JVM running Brooklyn to load and run Java code without detection by Brooklyn. Such code would have the privileges of the Java process running Brooklyn, including the ability to open files and network connections, and execute system commands. There is known to be a proof-of-concept exploit using this vulnerability.

- [https://github.com/dawetmaster/CVE-2016-8744-brooklyn-server-vulnerable](https://github.com/dawetmaster/CVE-2016-8744-brooklyn-server-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-8744-brooklyn-server-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-8744-brooklyn-server-vulnerable.svg)


## CVE-2016-8741
 The Apache Qpid Broker for Java can be configured to use different so called AuthenticationProviders to handle user authentication. Among the choices are the SCRAM-SHA-1 and SCRAM-SHA-256 AuthenticationProvider types. It was discovered that these AuthenticationProviders in Apache Qpid Broker for Java 6.0.x before 6.0.6 and 6.1.x before 6.1.1 prematurely terminate the SCRAM SASL negotiation if the provided user name does not exist thus allowing remote attacker to determine the existence of user accounts. The Vulnerability does not apply to AuthenticationProviders other than SCRAM-SHA-1 and SCRAM-SHA-256.

- [https://github.com/dawetmaster/CVE-2016-8741-qpid-broker-j-vulnerable](https://github.com/dawetmaster/CVE-2016-8741-qpid-broker-j-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-8741-qpid-broker-j-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-8741-qpid-broker-j-vulnerable.svg)


## CVE-2016-7051
 XmlMapper in the Jackson XML dataformat component (aka jackson-dataformat-xml) before 2.7.8 and 2.8.x before 2.8.4 allows remote attackers to conduct server-side request forgery (SSRF) attacks via vectors related to a DTD.

- [https://github.com/dawetmaster/CVE-2016-7051-jackson-dataformat-xml-vulnerable](https://github.com/dawetmaster/CVE-2016-7051-jackson-dataformat-xml-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-7051-jackson-dataformat-xml-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-7051-jackson-dataformat-xml-vulnerable.svg)


## CVE-2016-6809
 Apache Tika before 1.14 allows Java code execution for serialized objects embedded in MATLAB files. The issue exists because Tika invokes JMatIO to do native deserialization.

- [https://github.com/dawetmaster/CVE-2016-6809-tika-vulnerable](https://github.com/dawetmaster/CVE-2016-6809-tika-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-6809-tika-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-6809-tika-vulnerable.svg)


## CVE-2016-6802
 Apache Shiro before 1.3.2 allows attackers to bypass intended servlet filters and gain access by leveraging use of a non-root servlet context path.

- [https://github.com/dawetmaster/CVE-2016-6802-shiro-vulnerable](https://github.com/dawetmaster/CVE-2016-6802-shiro-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-6802-shiro-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-6802-shiro-vulnerable.svg)


## CVE-2016-6801
 Cross-site request forgery (CSRF) vulnerability in the CSRF content-type check in Jackrabbit-Webdav in Apache Jackrabbit 2.4.x before 2.4.6, 2.6.x before 2.6.6, 2.8.x before 2.8.3, 2.10.x before 2.10.4, 2.12.x before 2.12.4, and 2.13.x before 2.13.3 allows remote attackers to hijack the authentication of unspecified victims for requests that create a resource via an HTTP POST request with a (1) missing or (2) crafted Content-Type header.

- [https://github.com/dawetmaster/CVE-2016-6801-jackrabbit-vulnerable](https://github.com/dawetmaster/CVE-2016-6801-jackrabbit-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-6801-jackrabbit-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-6801-jackrabbit-vulnerable.svg)


## CVE-2016-4974
 Apache Qpid AMQP 0-x JMS client before 6.0.4 and JMS (AMQP 1.0) before 0.10.0 does not restrict the use of classes available on the classpath, which might allow remote authenticated users with permission to send messages to deserialize arbitrary objects and execute arbitrary code by leveraging a crafted serialized object in a JMS ObjectMessage that is handled by the getObject function.

- [https://github.com/dawetmaster/CVE-2016-4974-qpid-broker-j-vulnerable](https://github.com/dawetmaster/CVE-2016-4974-qpid-broker-j-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-4974-qpid-broker-j-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-4974-qpid-broker-j-vulnerable.svg)


## CVE-2016-4464
 The application plugins in Apache CXF Fediz 1.2.x before 1.2.3 and 1.3.x before 1.3.1 do not match SAML AudienceRestriction values against configured audience URIs, which might allow remote attackers to have bypass intended restrictions and have unspecified other impact via a crafted SAML token with a trusted signature.

- [https://github.com/dawetmaster/CVE-2016-4464-cxf-fediz-vulnerable](https://github.com/dawetmaster/CVE-2016-4464-cxf-fediz-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-4464-cxf-fediz-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-4464-cxf-fediz-vulnerable.svg)


## CVE-2016-3092
 The MultipartStream class in Apache Commons Fileupload before 1.3.2, as used in Apache Tomcat 7.x before 7.0.70, 8.x before 8.0.36, 8.5.x before 8.5.3, and 9.x before 9.0.0.M7 and other products, allows remote attackers to cause a denial of service (CPU consumption) via a long boundary string.

- [https://github.com/dawetmaster/CVE-2016-3092-commons-fileupload-vulnerable](https://github.com/dawetmaster/CVE-2016-3092-commons-fileupload-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2016-3092-commons-fileupload-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2016-3092-commons-fileupload-vulnerable.svg)


## CVE-2015-6748
 Cross-site scripting (XSS) vulnerability in jsoup before 1.8.3.

- [https://github.com/dawetmaster/CVE-2015-6748-jsoup-vulnerable](https://github.com/dawetmaster/CVE-2015-6748-jsoup-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2015-6748-jsoup-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2015-6748-jsoup-vulnerable.svg)


## CVE-2015-6254
 The (1) Service Provider (SP) and (2) Identity Provider (IdP) in PicketLink before 2.7.0 does not ensure that the Destination attribute in a Response element in a SAML assertion matches the location from which the message was received, which allows remote attackers to have unspecified impact via unknown vectors.  NOTE: this identifier was SPLIT from CVE-2015-0277 per ADT2 due to different vulnerability types.

- [https://github.com/dawetmaster/CVE-2015-6254-picketlink-bindings-vulnerable](https://github.com/dawetmaster/CVE-2015-6254-picketlink-bindings-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2015-6254-picketlink-bindings-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2015-6254-picketlink-bindings-vulnerable.svg)


## CVE-2015-5253
 The SAML Web SSO module in Apache CXF before 2.7.18, 3.0.x before 3.0.7, and 3.1.x before 3.1.3 allows remote authenticated users to bypass authentication via a crafted SAML response with a valid signed assertion, related to a "wrapping attack."

- [https://github.com/dawetmaster/CVE-2015-5253-cxf-vulnerable](https://github.com/dawetmaster/CVE-2015-5253-cxf-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2015-5253-cxf-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2015-5253-cxf-vulnerable.svg)


## CVE-2015-3271
 Apache Tika server (aka tika-server) in Apache Tika 1.9 might allow remote attackers to read arbitrary files via the HTTP fileUrl header.

- [https://github.com/dawetmaster/CVE-2015-3271-tika-vulnerable](https://github.com/dawetmaster/CVE-2015-3271-tika-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2015-3271-tika-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2015-3271-tika-vulnerable.svg)


## CVE-2015-2913
 server/network/protocol/http/OHttpSessionManager.java in the Studio component in OrientDB Server Community Edition before 2.0.15 and 2.1.x before 2.1.1 improperly relies on the java.util.Random class for generation of random Session ID values, which makes it easier for remote attackers to predict a value by determining the internal state of the PRNG in this class.

- [https://github.com/dawetmaster/CVE-2015-2913-orientdb-vulnerable](https://github.com/dawetmaster/CVE-2015-2913-orientdb-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2015-2913-orientdb-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2015-2913-orientdb-vulnerable.svg)


## CVE-2015-2912
 The JSONP endpoint in the Studio component in OrientDB Server Community Edition before 2.0.15 and 2.1.x before 2.1.1 does not properly restrict callback values, which allows remote attackers to conduct cross-site request forgery (CSRF) attacks, and obtain sensitive information, via a crafted HTTP request.

- [https://github.com/dawetmaster/CVE-2015-2912-orientdb-vulnerable](https://github.com/dawetmaster/CVE-2015-2912-orientdb-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2015-2912-orientdb-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2015-2912-orientdb-vulnerable.svg)


## CVE-2015-2156
 Netty before 3.9.8.Final, 3.10.x before 3.10.3.Final, 4.0.x before 4.0.28.Final, and 4.1.x before 4.1.0.Beta5 and Play Framework 2.x before 2.3.9 might allow remote attackers to bypass the httpOnly flag on cookies and obtain sensitive information by leveraging improper validation of cookie name and value characters.

- [https://github.com/dawetmaster/CVE-2015-2156-netty-vulnerable](https://github.com/dawetmaster/CVE-2015-2156-netty-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2015-2156-netty-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2015-2156-netty-vulnerable.svg)


## CVE-2014-7816
 Directory traversal vulnerability in JBoss Undertow 1.0.x before 1.0.17, 1.1.x before 1.1.0.CR5, and 1.2.x before 1.2.0.Beta3, when running on Windows, allows remote attackers to read arbitrary files via a .. (dot dot) in a resource URI.

- [https://github.com/dawetmaster/CVE-2014-7816-undertow-vulnerable](https://github.com/dawetmaster/CVE-2014-7816-undertow-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2014-7816-undertow-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2014-7816-undertow-vulnerable.svg)


## CVE-2014-3651
 JBoss KeyCloak before 1.0.3.Final allows remote attackers to cause a denial of service (resource consumption) via a large value in the size parameter to auth/qrcode, related to QR code generation.

- [https://github.com/dawetmaster/CVE-2014-3651-keycloak-vulnerable](https://github.com/dawetmaster/CVE-2014-3651-keycloak-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2014-3651-keycloak-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2014-3651-keycloak-vulnerable.svg)


## CVE-2014-3488
 The SslHandler in Netty before 3.9.2 allows remote attackers to cause a denial of service (infinite loop and CPU consumption) via a crafted SSLv2Hello message.

- [https://github.com/dawetmaster/CVE-2014-3488-netty-vulnerable](https://github.com/dawetmaster/CVE-2014-3488-netty-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2014-3488-netty-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2014-3488-netty-vulnerable.svg)


## CVE-2014-0050
 MultipartStream.java in Apache Commons FileUpload before 1.3.1, as used in Apache Tomcat, JBoss Web, and other products, allows remote attackers to cause a denial of service (infinite loop and CPU consumption) via a crafted Content-Type header that bypasses a loop's intended exit conditions.

- [https://github.com/dawetmaster/CVE-2014-0050-commons-fileupload-vulnerable](https://github.com/dawetmaster/CVE-2014-0050-commons-fileupload-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2014-0050-commons-fileupload-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2014-0050-commons-fileupload-vulnerable.svg)


## CVE-2013-6465
 Multiple cross-site scripting (XSS) vulnerabilities in JBPM KIE Workbench 6.0.x allow remote authenticated users to inject arbitrary web script or HTML via vectors related to task name html inputs.

- [https://github.com/dawetmaster/CVE-2013-6465-jjbpm-wbbpm-vulnerable](https://github.com/dawetmaster/CVE-2013-6465-jjbpm-wbbpm-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2013-6465-jjbpm-wbbpm-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2013-6465-jjbpm-wbbpm-vulnerable.svg)


## CVE-2013-5960
 The authenticated-encryption feature in the symmetric-encryption implementation in the OWASP Enterprise Security API (ESAPI) for Java 2.x before 2.1.0.1 does not properly resist tampering with serialized ciphertext, which makes it easier for remote attackers to bypass intended cryptographic protection mechanisms via an attack against the intended cipher mode in a non-default configuration, a different vulnerability than CVE-2013-5679.

- [https://github.com/dawetmaster/CVE-2013-5960-esapi-java-legacy-vulnerable](https://github.com/dawetmaster/CVE-2013-5960-esapi-java-legacy-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2013-5960-esapi-java-legacy-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2013-5960-esapi-java-legacy-vulnerable.svg)


## CVE-2013-5679
 The authenticated-encryption feature in the symmetric-encryption implementation in the OWASP Enterprise Security API (ESAPI) for Java 2.x before 2.1.0 does not properly resist tampering with serialized ciphertext, which makes it easier for remote attackers to bypass intended cryptographic protection mechanisms via an attack against authenticity in the default configuration, involving a null MAC and a zero MAC length.

- [https://github.com/dawetmaster/CVE-2013-5679-esapi-java-legacy-vulnerable](https://github.com/dawetmaster/CVE-2013-5679-esapi-java-legacy-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2013-5679-esapi-java-legacy-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2013-5679-esapi-java-legacy-vulnerable.svg)


## CVE-2013-4517
 Apache Santuario XML Security for Java before 1.5.6, when applying Transforms, allows remote attackers to cause a denial of service (memory consumption) via crafted Document Type Definitions (DTDs), related to signatures.

- [https://github.com/dawetmaster/CVE-2013-4517-santuario-java-vulnerable](https://github.com/dawetmaster/CVE-2013-4517-santuario-java-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2013-4517-santuario-java-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2013-4517-santuario-java-vulnerable.svg)


## CVE-2013-2186
 The DiskFileItem class in Apache Commons FileUpload, as used in Red Hat JBoss BRMS 5.3.1; JBoss Portal 4.3 CP07, 5.2.2, and 6.0.0; and Red Hat JBoss Web Server 1.0.2 allows remote attackers to write to arbitrary files via a NULL byte in a file name in a serialized instance.

- [https://github.com/dawetmaster/CVE-2013-2186-commons-fileupload-vulnerable](https://github.com/dawetmaster/CVE-2013-2186-commons-fileupload-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2013-2186-commons-fileupload-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2013-2186-commons-fileupload-vulnerable.svg)


## CVE-2013-2172
 jcp/xml/dsig/internal/dom/DOMCanonicalizationMethod.java in Apache Santuario XML Security for Java 1.4.x before 1.4.8 and 1.5.x before 1.5.5 allows context-dependent attackers to spoof an XML Signature by using the CanonicalizationMethod parameter to specify an arbitrary weak "canonicalization algorithm to apply to the SignedInfo part of the Signature."

- [https://github.com/dawetmaster/CVE-2013-2172-santuario-java-vulnerable](https://github.com/dawetmaster/CVE-2013-2172-santuario-java-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2013-2172-santuario-java-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2013-2172-santuario-java-vulnerable.svg)


## CVE-2011-4367
 Multiple directory traversal vulnerabilities in MyFaces JavaServer Faces (JSF) in Apache MyFaces Core 2.0.x before 2.0.12 and 2.1.x before 2.1.6 allow remote attackers to read arbitrary files via a .. (dot dot) in the (1) ln parameter to faces/javax.faces.resource/web.xml or (2) the PATH_INFO to faces/javax.faces.resource/.

- [https://github.com/dawetmaster/CVE-2011-4367-myfaces-vulnerable](https://github.com/dawetmaster/CVE-2011-4367-myfaces-vulnerable) :  ![starts](https://img.shields.io/github/stars/dawetmaster/CVE-2011-4367-myfaces-vulnerable.svg) ![forks](https://img.shields.io/github/forks/dawetmaster/CVE-2011-4367-myfaces-vulnerable.svg)

