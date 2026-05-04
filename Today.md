# Update 2026-05-04
## CVE-2026-42779
Applications using Apache MINA are advised to upgrade.

- [https://github.com/dinosn/CVE-2026-42779](https://github.com/dinosn/CVE-2026-42779) :  ![starts](https://img.shields.io/github/stars/dinosn/CVE-2026-42779.svg) ![forks](https://img.shields.io/github/forks/dinosn/CVE-2026-42779.svg)


## CVE-2026-42167
 mod_sql in ProFTPD before 1.3.9a allows remote attackers to execute arbitrary code via a username, in scenarios where there is logging of USER requests with an expansion such as %U, and the SQL backend allows commands (e.g., COPY TO PROGRAM).

- [https://github.com/efeanilarslan/CVE-2026-42167-Exploit](https://github.com/efeanilarslan/CVE-2026-42167-Exploit) :  ![starts](https://img.shields.io/github/stars/efeanilarslan/CVE-2026-42167-Exploit.svg) ![forks](https://img.shields.io/github/forks/efeanilarslan/CVE-2026-42167-Exploit.svg)
- [https://github.com/jimmexploit/CVE-2026-42167-PoC](https://github.com/jimmexploit/CVE-2026-42167-PoC) :  ![starts](https://img.shields.io/github/stars/jimmexploit/CVE-2026-42167-PoC.svg) ![forks](https://img.shields.io/github/forks/jimmexploit/CVE-2026-42167-PoC.svg)


## CVE-2026-41940
 cPanel and WHM versions after 11.40 contain an authentication bypass vulnerability in the login flow that allows unauthenticated remote attackers to gain unauthorized access to the control panel.

- [https://github.com/YudaSamuel/cpanel-vuln-scanner](https://github.com/YudaSamuel/cpanel-vuln-scanner) :  ![starts](https://img.shields.io/github/stars/YudaSamuel/cpanel-vuln-scanner.svg) ![forks](https://img.shields.io/github/forks/YudaSamuel/cpanel-vuln-scanner.svg)
- [https://github.com/Ishanoshada/CVE-2026-41940-Exploit-PoC](https://github.com/Ishanoshada/CVE-2026-41940-Exploit-PoC) :  ![starts](https://img.shields.io/github/stars/Ishanoshada/CVE-2026-41940-Exploit-PoC.svg) ![forks](https://img.shields.io/github/forks/Ishanoshada/CVE-2026-41940-Exploit-PoC.svg)
- [https://github.com/dennisec/CVE-2026-41940](https://github.com/dennisec/CVE-2026-41940) :  ![starts](https://img.shields.io/github/stars/dennisec/CVE-2026-41940.svg) ![forks](https://img.shields.io/github/forks/dennisec/CVE-2026-41940.svg)
- [https://github.com/MrOplus/CVE-2026-41940](https://github.com/MrOplus/CVE-2026-41940) :  ![starts](https://img.shields.io/github/stars/MrOplus/CVE-2026-41940.svg) ![forks](https://img.shields.io/github/forks/MrOplus/CVE-2026-41940.svg)
- [https://github.com/ThatNotEasy/CVE-2026-41940](https://github.com/ThatNotEasy/CVE-2026-41940) :  ![starts](https://img.shields.io/github/stars/ThatNotEasy/CVE-2026-41940.svg) ![forks](https://img.shields.io/github/forks/ThatNotEasy/CVE-2026-41940.svg)
- [https://github.com/linko-iheb/cve-2026-41940-scanner](https://github.com/linko-iheb/cve-2026-41940-scanner) :  ![starts](https://img.shields.io/github/stars/linko-iheb/cve-2026-41940-scanner.svg) ![forks](https://img.shields.io/github/forks/linko-iheb/cve-2026-41940-scanner.svg)
- [https://github.com/3tternp/CVE-2026-41940---cPanel-WHM-check](https://github.com/3tternp/CVE-2026-41940---cPanel-WHM-check) :  ![starts](https://img.shields.io/github/stars/3tternp/CVE-2026-41940---cPanel-WHM-check.svg) ![forks](https://img.shields.io/github/forks/3tternp/CVE-2026-41940---cPanel-WHM-check.svg)


## CVE-2026-41200
 STIG Manager is an API and web client for managing  Security Technical Implementation Guides (STIG) assessments of Information Systems. Versions 1.5.10 through 1.6.7 have a reflected Cross-Site Scripting (XSS) vulnerability in the OIDC authentication error handling code in `src/init.js` and `public/reauth.html`. During the OIDC redirect flow, the `error` and `error_description` query parameters returned by the OIDC provider are written directly to the DOM via `innerHTML` without HTML escaping. An attacker who can craft a malicious redirect URL and convince a user to follow it can execute arbitrary JavaScript in the application's origin context. The vulnerability is most severe when the targeted user has an active STIG Manager session running in another browser tab — injected code executes in the same origin and can communicate with the SharedWorker managing the active access token, enabling authenticated API requests on behalf of the victim including reading and modifying collection data. The vulnerability is patched in version 1.6.8. There is no workaround short of upgrading. Deployments behind a web application firewall that filters reflected XSS payloads in query parameters may have partial mitigation, but this is not a substitute for patching.

- [https://github.com/Hunt-Benito/cve-2026-41200-stig-manager-oidc-reflected-xss](https://github.com/Hunt-Benito/cve-2026-41200-stig-manager-oidc-reflected-xss) :  ![starts](https://img.shields.io/github/stars/Hunt-Benito/cve-2026-41200-stig-manager-oidc-reflected-xss.svg) ![forks](https://img.shields.io/github/forks/Hunt-Benito/cve-2026-41200-stig-manager-oidc-reflected-xss.svg)


## CVE-2026-41044
Users are recommended to upgrade to version 6.2.5 or 5.19.6, which fixes the issue.

- [https://github.com/mrillicit/CVE-2026-41044](https://github.com/mrillicit/CVE-2026-41044) :  ![starts](https://img.shields.io/github/stars/mrillicit/CVE-2026-41044.svg) ![forks](https://img.shields.io/github/forks/mrillicit/CVE-2026-41044.svg)


## CVE-2026-39387
 BoidCMS is an open-source, PHP-based flat-file CMS for building simple websites and blogs, using JSON as its database. Versions prior to 2.1.3 are vulnerable to a critical Local File Inclusion (LFI) attack via the tpl parameter, which can lead to Remote Code Execution (RCE).The application fails to sanitize the tpl (template) parameter during page creation and updates. This parameter is passed directly to a require_once() statement without path validation. An authenticated administrator can exploit this by injecting path traversal sequences (../) into the tpl value to escape the intended theme directory and include arbitrary files — specifically, files from the server's media/ directory. When combined with the file upload functionality, this becomes a full RCE chain: an attacker can first upload a file with embedded PHP code (e.g., disguised as image data), then use the path traversal vulnerability to include that file via require_once(), executing the embedded code with web server privileges. This issue has been fixed in version 2.1.3.

- [https://github.com/xp1tr/CVE-2026-39387](https://github.com/xp1tr/CVE-2026-39387) :  ![starts](https://img.shields.io/github/stars/xp1tr/CVE-2026-39387.svg) ![forks](https://img.shields.io/github/forks/xp1tr/CVE-2026-39387.svg)


## CVE-2026-33825
 Insufficient granularity of access control in Microsoft Defender allows an authorized attacker to elevate privileges locally.

- [https://github.com/Joe1sn/CVE-2026-33825](https://github.com/Joe1sn/CVE-2026-33825) :  ![starts](https://img.shields.io/github/stars/Joe1sn/CVE-2026-33825.svg) ![forks](https://img.shields.io/github/forks/Joe1sn/CVE-2026-33825.svg)


## CVE-2026-31431
AD directly.

- [https://github.com/MartinPham/copy-fail-CVE-2026-31431-php](https://github.com/MartinPham/copy-fail-CVE-2026-31431-php) :  ![starts](https://img.shields.io/github/stars/MartinPham/copy-fail-CVE-2026-31431-php.svg) ![forks](https://img.shields.io/github/forks/MartinPham/copy-fail-CVE-2026-31431-php.svg)
- [https://github.com/qi4L/CVE-2026-31431-Container-Escape](https://github.com/qi4L/CVE-2026-31431-Container-Escape) :  ![starts](https://img.shields.io/github/stars/qi4L/CVE-2026-31431-Container-Escape.svg) ![forks](https://img.shields.io/github/forks/qi4L/CVE-2026-31431-Container-Escape.svg)
- [https://github.com/haydenjames/CVE-2026-31431-check](https://github.com/haydenjames/CVE-2026-31431-check) :  ![starts](https://img.shields.io/github/stars/haydenjames/CVE-2026-31431-check.svg) ![forks](https://img.shields.io/github/forks/haydenjames/CVE-2026-31431-check.svg)
- [https://github.com/malwarekid/CVE-2026-31431](https://github.com/malwarekid/CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/malwarekid/CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/malwarekid/CVE-2026-31431.svg)
- [https://github.com/mahdi13830510/CVE-2026-31431-mitigation-suite](https://github.com/mahdi13830510/CVE-2026-31431-mitigation-suite) :  ![starts](https://img.shields.io/github/stars/mahdi13830510/CVE-2026-31431-mitigation-suite.svg) ![forks](https://img.shields.io/github/forks/mahdi13830510/CVE-2026-31431-mitigation-suite.svg)
- [https://github.com/M4xSec/CVE-2026-31431-RCE-Exploit](https://github.com/M4xSec/CVE-2026-31431-RCE-Exploit) :  ![starts](https://img.shields.io/github/stars/M4xSec/CVE-2026-31431-RCE-Exploit.svg) ![forks](https://img.shields.io/github/forks/M4xSec/CVE-2026-31431-RCE-Exploit.svg)
- [https://github.com/scriptzteam/Paranoid-Copy-Fail-CVE-2026-31431](https://github.com/scriptzteam/Paranoid-Copy-Fail-CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/scriptzteam/Paranoid-Copy-Fail-CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/scriptzteam/Paranoid-Copy-Fail-CVE-2026-31431.svg)
- [https://github.com/rippsec/cve-2026-31431](https://github.com/rippsec/cve-2026-31431) :  ![starts](https://img.shields.io/github/stars/rippsec/cve-2026-31431.svg) ![forks](https://img.shields.io/github/forks/rippsec/cve-2026-31431.svg)
- [https://github.com/Sl4cK0TH/CVE-2026-31431-PoC](https://github.com/Sl4cK0TH/CVE-2026-31431-PoC) :  ![starts](https://img.shields.io/github/stars/Sl4cK0TH/CVE-2026-31431-PoC.svg) ![forks](https://img.shields.io/github/forks/Sl4cK0TH/CVE-2026-31431-PoC.svg)
- [https://github.com/KanbaraAkihito/CVE-2026-31431-copyfail-rs](https://github.com/KanbaraAkihito/CVE-2026-31431-copyfail-rs) :  ![starts](https://img.shields.io/github/stars/KanbaraAkihito/CVE-2026-31431-copyfail-rs.svg) ![forks](https://img.shields.io/github/forks/KanbaraAkihito/CVE-2026-31431-copyfail-rs.svg)
- [https://github.com/AvPrince26/copy-fail-CVE-2026-31431-Python-Golfing](https://github.com/AvPrince26/copy-fail-CVE-2026-31431-Python-Golfing) :  ![starts](https://img.shields.io/github/stars/AvPrince26/copy-fail-CVE-2026-31431-Python-Golfing.svg) ![forks](https://img.shields.io/github/forks/AvPrince26/copy-fail-CVE-2026-31431-Python-Golfing.svg)
- [https://github.com/krish-foren6/CVE-2026-31431-Report-Copy-fail-Vulnerability-](https://github.com/krish-foren6/CVE-2026-31431-Report-Copy-fail-Vulnerability-) :  ![starts](https://img.shields.io/github/stars/krish-foren6/CVE-2026-31431-Report-Copy-fail-Vulnerability-.svg) ![forks](https://img.shields.io/github/forks/krish-foren6/CVE-2026-31431-Report-Copy-fail-Vulnerability-.svg)
- [https://github.com/3jee/copy-fail-go](https://github.com/3jee/copy-fail-go) :  ![starts](https://img.shields.io/github/stars/3jee/copy-fail-go.svg) ![forks](https://img.shields.io/github/forks/3jee/copy-fail-go.svg)
- [https://github.com/suominen/CVE-2026-31431](https://github.com/suominen/CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/suominen/CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/suominen/CVE-2026-31431.svg)
- [https://github.com/pedromizz/copy-fail](https://github.com/pedromizz/copy-fail) :  ![starts](https://img.shields.io/github/stars/pedromizz/copy-fail.svg) ![forks](https://img.shields.io/github/forks/pedromizz/copy-fail.svg)


## CVE-2026-7671
 A vulnerability has been found in CodeWise Tornet Scooter Mobile App 4.75 on iOS/Android. The impacted element is an unknown function of the file /TwoFactor. Such manipulation leads to improper restriction of excessive authentication attempts. The attack may be performed from remote. Attacks of this nature are highly complex. The exploitability is regarded as difficult. The exploit has been disclosed to the public and may be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/CaginKyr/CVE-2026-7671](https://github.com/CaginKyr/CVE-2026-7671) :  ![starts](https://img.shields.io/github/stars/CaginKyr/CVE-2026-7671.svg) ![forks](https://img.shields.io/github/forks/CaginKyr/CVE-2026-7671.svg)


## CVE-2026-7567
 The Temporary Login plugin for WordPress is vulnerable to Authentication Bypass in versions up to and including 1.0.0. This is due to improper input validation in the maybe_login_temporary_user() function, which fails to verify that the 'temp-login-token' GET parameter is a scalar string before processing it. When the parameter is supplied as an array, PHP's empty() check is bypassed and sanitize_key() returns an empty string, which is then passed as the meta_value to get_users(). WordPress ignores an empty meta_value and returns all users matching the meta_key '_temporary_login_token', allowing authentication without a valid token. This makes it possible for unauthenticated attackers to authenticate as any active temporary login user by sending a single crafted GET request.

- [https://github.com/amirhosseinjamshidi64/CVE-2026-7567-POC](https://github.com/amirhosseinjamshidi64/CVE-2026-7567-POC) :  ![starts](https://img.shields.io/github/stars/amirhosseinjamshidi64/CVE-2026-7567-POC.svg) ![forks](https://img.shields.io/github/forks/amirhosseinjamshidi64/CVE-2026-7567-POC.svg)


## CVE-2025-69985
 FUXA 1.2.8 and prior contains an Authentication Bypass vulnerability leading to Remote Code Execution (RCE). The vulnerability exists in the server/api/jwt-helper.js middleware, which improperly trusts the HTTP "Referer" header to validate internal requests. A remote unauthenticated attacker can bypass JWT authentication by spoofing the Referer header to match the server's host. Successful exploitation allows the attacker to access the protected /api/runscript endpoint and execute arbitrary Node.js code on the server.

- [https://github.com/ladybugsaga/CVE-2025-69985-FUXA-Exploit](https://github.com/ladybugsaga/CVE-2025-69985-FUXA-Exploit) :  ![starts](https://img.shields.io/github/stars/ladybugsaga/CVE-2025-69985-FUXA-Exploit.svg) ![forks](https://img.shields.io/github/forks/ladybugsaga/CVE-2025-69985-FUXA-Exploit.svg)


## CVE-2025-58726
 Improper access control in Windows SMB Server allows an authorized attacker to elevate privileges over a network.

- [https://github.com/jonaslejon/ad-autopwn](https://github.com/jonaslejon/ad-autopwn) :  ![starts](https://img.shields.io/github/stars/jonaslejon/ad-autopwn.svg) ![forks](https://img.shields.io/github/forks/jonaslejon/ad-autopwn.svg)


## CVE-2025-57819
 FreePBX is an open-source web-based graphical user interface. FreePBX 15, 16, and 17 endpoints are vulnerable due to insufficiently sanitized user-supplied data allowing unauthenticated access to FreePBX Administrator leading to arbitrary database manipulation and remote code execution. This issue has been patched in endpoint versions 15.0.66, 16.0.89, and 17.0.3.

- [https://github.com/fuckyourheroes/CVE-2025-57819](https://github.com/fuckyourheroes/CVE-2025-57819) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-57819.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-57819.svg)


## CVE-2025-54309
 CrushFTP 10 before 10.8.5 and 11 before 11.3.4_23, when the DMZ proxy feature is not used, mishandles AS2 validation and consequently allows remote attackers to obtain admin access via HTTPS, as exploited in the wild in July 2025.

- [https://github.com/fuckyourheroes/CVE-2025-54309](https://github.com/fuckyourheroes/CVE-2025-54309) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-54309.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-54309.svg)


## CVE-2025-53694
 Exposure of Sensitive Information to an Unauthorized Actor vulnerability in Sitecore Sitecore Experience Manager (XM), Sitecore Experience Platform (XP).This issue affects Sitecore Experience Manager (XM): from 9.2 through 10.4; Experience Platform (XP): from 9.2 through 10.4.

- [https://github.com/fuckyourheroes/CVE-2025-53694](https://github.com/fuckyourheroes/CVE-2025-53694) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-53694.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-53694.svg)
- [https://github.com/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691](https://github.com/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691.svg)


## CVE-2025-53693
 Use of Externally-Controlled Input to Select Classes or Code ('Unsafe Reflection') vulnerability in Sitecore Sitecore Experience Manager (XM), Sitecore Experience Platform (XP) allows Cache Poisoning.This issue affects Sitecore Experience Manager (XM): from 9.0 through 9.3, from 10.0 through 10.4; Experience Platform (XP): from 9.0 through 9.3, from 10.0 through 10.4.

- [https://github.com/fuckyourheroes/CVE-2025-53693](https://github.com/fuckyourheroes/CVE-2025-53693) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-53693.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-53693.svg)


## CVE-2025-53691
 Deserialization of Untrusted Data vulnerability in Sitecore Experience Manager (XM), Sitecore Experience Platform (XP) allows Remote Code Execution (RCE).This issue affects Experience Manager (XM): from 9.0 through 9.3, from 10.0 through 10.4; Experience Platform (XP): from 9.0 through 9.3, from 10.0 through 10.4.

- [https://github.com/fuckyourheroes/CVE-2025-53691](https://github.com/fuckyourheroes/CVE-2025-53691) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-53691.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-53691.svg)
- [https://github.com/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691](https://github.com/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-53694-to-CVE-2025-53691.svg)


## CVE-2025-49132
 Pterodactyl is a free, open-source game server management panel. Prior to version 1.11.11, using the /locales/locale.json with the locale and namespace query parameters, a malicious actor is able to execute arbitrary code without being authenticated. With the ability to execute arbitrary code it could be used to gain access to the Panel's server, read credentials from the Panel's config, extract sensitive information from the database, access files of servers managed by the panel, etc. This issue has been patched in version 1.11.11. There are no software workarounds for this vulnerability, but use of an external Web Application Firewall (WAF) could help mitigate this attack.

- [https://github.com/unixskid/CVE-2025-49132-Pterodactyl-RCE](https://github.com/unixskid/CVE-2025-49132-Pterodactyl-RCE) :  ![starts](https://img.shields.io/github/stars/unixskid/CVE-2025-49132-Pterodactyl-RCE.svg) ![forks](https://img.shields.io/github/forks/unixskid/CVE-2025-49132-Pterodactyl-RCE.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/hujiaozhuzhu/CVE-2025-29927__Next.js](https://github.com/hujiaozhuzhu/CVE-2025-29927__Next.js) :  ![starts](https://img.shields.io/github/stars/hujiaozhuzhu/CVE-2025-29927__Next.js.svg) ![forks](https://img.shields.io/github/forks/hujiaozhuzhu/CVE-2025-29927__Next.js.svg)
- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-24367
 Cacti is an open source performance and fault management framework. An authenticated Cacti user can abuse graph creation and graph template functionality to create arbitrary PHP scripts in the web root of the application, leading to remote code execution on the server. This vulnerability is fixed in 1.2.29.

- [https://github.com/dantedansh/CVE-2025-24367-Cacti-Exploit](https://github.com/dantedansh/CVE-2025-24367-Cacti-Exploit) :  ![starts](https://img.shields.io/github/stars/dantedansh/CVE-2025-24367-Cacti-Exploit.svg) ![forks](https://img.shields.io/github/forks/dantedansh/CVE-2025-24367-Cacti-Exploit.svg)


## CVE-2025-3515
 The Drag and Drop Multiple File Upload for Contact Form 7 plugin for WordPress is vulnerable to arbitrary file uploads due to insufficient file type validation in all versions up to, and including, 1.3.8.9. This makes it possible for unauthenticated attackers to bypass the plugin's blacklist and upload .phar or other dangerous file types on the affected site's server, which may make remote code execution possible on the servers that are configured to handle .phar files as executable PHP scripts, particularly in default Apache+mod_php configurations where the file extension is not strictly validated before being passed to the PHP interpreter.

- [https://github.com/fuckyourheroes/CVE-2025-3515](https://github.com/fuckyourheroes/CVE-2025-3515) :  ![starts](https://img.shields.io/github/stars/fuckyourheroes/CVE-2025-3515.svg) ![forks](https://img.shields.io/github/forks/fuckyourheroes/CVE-2025-3515.svg)


## CVE-2024-53677
You can find more details in  https://cwiki.apache.org/confluence/display/WW/S2-067

- [https://github.com/ctfsec/CVE-2024-53677](https://github.com/ctfsec/CVE-2024-53677) :  ![starts](https://img.shields.io/github/stars/ctfsec/CVE-2024-53677.svg) ![forks](https://img.shields.io/github/forks/ctfsec/CVE-2024-53677.svg)


## CVE-2024-36039
 PyMySQL through 1.1.0 allows SQL injection if used with untrusted JSON input because keys are not escaped by escape_dict.

- [https://github.com/zenniskayy2k4/CVE-2024-36039_PoC](https://github.com/zenniskayy2k4/CVE-2024-36039_PoC) :  ![starts](https://img.shields.io/github/stars/zenniskayy2k4/CVE-2024-36039_PoC.svg) ![forks](https://img.shields.io/github/forks/zenniskayy2k4/CVE-2024-36039_PoC.svg)


## CVE-2024-3094
Through a series of complex obfuscations, the liblzma build process extracts a prebuilt object file from a disguised test file existing in the source code, which is then used to modify specific functions in the liblzma code. This results in a modified liblzma library that can be used by any software linked against this library, intercepting and modifying the data interaction with this library.

- [https://github.com/jbnetwork-git/CVE-2024-3094-XZ-Utils-Check](https://github.com/jbnetwork-git/CVE-2024-3094-XZ-Utils-Check) :  ![starts](https://img.shields.io/github/stars/jbnetwork-git/CVE-2024-3094-XZ-Utils-Check.svg) ![forks](https://img.shields.io/github/forks/jbnetwork-git/CVE-2024-3094-XZ-Utils-Check.svg)


## CVE-2023-46604
which fixes this issue.

- [https://github.com/trnguyen03/activemq-ids-ips-lab](https://github.com/trnguyen03/activemq-ids-ips-lab) :  ![starts](https://img.shields.io/github/stars/trnguyen03/activemq-ids-ips-lab.svg) ![forks](https://img.shields.io/github/forks/trnguyen03/activemq-ids-ips-lab.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/Taldrid1/cve-2021-41773](https://github.com/Taldrid1/cve-2021-41773) :  ![starts](https://img.shields.io/github/stars/Taldrid1/cve-2021-41773.svg) ![forks](https://img.shields.io/github/forks/Taldrid1/cve-2021-41773.svg)


## CVE-2020-11022
 In jQuery starting with 1.12.0 and before 3.5.0, passing HTML from untrusted sources - even after sanitizing it - to one of jQuery's DOM manipulation methods (i.e. .html(), .append(), and others) may execute untrusted code. This problem is patched in jQuery 3.5.0.

- [https://github.com/ibnurusdianto/CVE-2020-11022](https://github.com/ibnurusdianto/CVE-2020-11022) :  ![starts](https://img.shields.io/github/stars/ibnurusdianto/CVE-2020-11022.svg) ![forks](https://img.shields.io/github/forks/ibnurusdianto/CVE-2020-11022.svg)


## CVE-2019-6250
 A pointer overflow, with code execution, was discovered in ZeroMQ libzmq (aka 0MQ) 4.2.x and 4.3.x before 4.3.1. A v2_decoder.cpp zmq::v2_decoder_t::size_ready integer overflow allows an authenticated attacker to overwrite an arbitrary amount of bytes beyond the bounds of a buffer, which can be leveraged to run arbitrary code on the target system. The memory layout allows the attacker to inject OS commands into a data structure located immediately after the problematic buffer (i.e., it is not necessary to use a typical buffer-overflow exploitation technique that changes the flow of control).

- [https://github.com/dinosn/cve-2019-6250-lab](https://github.com/dinosn/cve-2019-6250-lab) :  ![starts](https://img.shields.io/github/stars/dinosn/cve-2019-6250-lab.svg) ![forks](https://img.shields.io/github/forks/dinosn/cve-2019-6250-lab.svg)

