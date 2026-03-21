# Update 2026-03-21
## CVE-2026-32746
 telnetd in GNU inetutils through 2.7 allows an out-of-bounds write in the LINEMODE SLC (Set Local Characters) suboption handler because add_slc does not check whether the buffer is full.

- [https://github.com/watchtowrlabs/watchtowr-vs-telnetd-CVE-2026-32746](https://github.com/watchtowrlabs/watchtowr-vs-telnetd-CVE-2026-32746) :  ![starts](https://img.shields.io/github/stars/watchtowrlabs/watchtowr-vs-telnetd-CVE-2026-32746.svg) ![forks](https://img.shields.io/github/forks/watchtowrlabs/watchtowr-vs-telnetd-CVE-2026-32746.svg)


## CVE-2026-32731
The `extract()` function in `gzip.js` constructs file-write paths using `fs.createWriteStream(path.join(exportPath, header.name))`. `path.join()` does not resolve or sanitise traversal segments such as `../`. It concatenates them as-is, meaning a tar entry named `../../evil.js` resolves to a path outside the intended extraction directory. No canonical-path check is performed before the write stream is opened. This is a textbook Zip Slip vulnerability. Any user who has been granted the Global Content Modify permission — a role routinely assigned to content editors and site managers — can upload a crafted `.tar.gz` file through the standard CMS import UI and write attacker-controlled content to any path the Node.js process can reach on the host filesystem. Version 3.5.3 of `@apostrophecms/import-export` fixes the issue.

- [https://github.com/0xEr3n/CVE-2026-32731](https://github.com/0xEr3n/CVE-2026-32731) :  ![starts](https://img.shields.io/github/stars/0xEr3n/CVE-2026-32731.svg) ![forks](https://img.shields.io/github/forks/0xEr3n/CVE-2026-32731.svg)


## CVE-2026-32255
 Kan is an open-source project management tool. In versions 0.5.4 and below, the /api/download/attatchment endpoint has no authentication and no URL validation. The Attachment Download endpoint accepts a user-supplied URL query parameter and passes it directly to fetch() server-side, and returns the full response body. An unauthenticated attacker can use this to make HTTP requests from the server to internal services, cloud metadata endpoints, or private network resources. This issue has been fixed in version 0.5.5. To workaround this issue, block or restrict access to /api/download/attatchment at the reverse proxy level (nginx, Cloudflare, etc.).

- [https://github.com/kOaDT/poc-cve-2026-32255](https://github.com/kOaDT/poc-cve-2026-32255) :  ![starts](https://img.shields.io/github/stars/kOaDT/poc-cve-2026-32255.svg) ![forks](https://img.shields.io/github/forks/kOaDT/poc-cve-2026-32255.svg)


## CVE-2026-32238
 OpenEMR is a free and open source electronic health records and medical practice management application. Versions prior to 8.0.0.2 contain a Command injection vulnerability in the backup functionality that can be exploited by authenticated attackers. The vulnerability exists due to insufficient input validation in the backup functionality. Version 8.0.0.2 fixes the issue.

- [https://github.com/ChrisSub08/CVE-2026-32238_RemoteCodeExecutionOpenEMR8.0.0](https://github.com/ChrisSub08/CVE-2026-32238_RemoteCodeExecutionOpenEMR8.0.0) :  ![starts](https://img.shields.io/github/stars/ChrisSub08/CVE-2026-32238_RemoteCodeExecutionOpenEMR8.0.0.svg) ![forks](https://img.shields.io/github/forks/ChrisSub08/CVE-2026-32238_RemoteCodeExecutionOpenEMR8.0.0.svg)


## CVE-2026-31891
 Cockpit is a headless content management system. Any Cockpit CMS instance running version 2.13.4 or earlier with API access enabled is potentially affected by a a SQL Injection vulnerability in the MongoLite Aggregation Optimizer. Any deployment where the `/api/content/aggregate/{model}` endpoint is publicly accessible or reachable by untrusted users may be vulnerable, and attackers in possession of a valid read-only API key (the lowest privilege level) can exploit this vulnerability — no admin access is required. An attacker can inject arbitrary SQL via unsanitized field names in aggregation queries, bypass the `_state=1` published-content filter to access unpublished or restricted content, and extract unauthorized data from the underlying SQLite content database. This vulnerability has been patched in version 2.13.5. The fix applies the same field-name sanitization introduced in v2.13.3 for `toJsonPath()` to the `toJsonExtractRaw()` method in `lib/MongoLite/Aggregation/Optimizer.php`, closing the injection vector in the Aggregation Optimizer.

- [https://github.com/ffasterss/CVE-2026-31891](https://github.com/ffasterss/CVE-2026-31891) :  ![starts](https://img.shields.io/github/stars/ffasterss/CVE-2026-31891.svg) ![forks](https://img.shields.io/github/forks/ffasterss/CVE-2026-31891.svg)


## CVE-2026-29041
 Chamilo is a learning management system. Prior to version 1.11.34, Chamilo LMS is affected by an authenticated remote code execution vulnerability caused by improper validation of uploaded files. The application relies solely on MIME-type verification when handling file uploads and does not adequately validate file extensions or enforce safe server-side storage restrictions. As a result, an authenticated low-privileged user can upload a crafted file containing executable code and subsequently execute arbitrary commands on the server. This issue has been patched in version 1.11.34.

- [https://github.com/kx00007/CVE-2026-29041](https://github.com/kx00007/CVE-2026-29041) :  ![starts](https://img.shields.io/github/stars/kx00007/CVE-2026-29041.svg) ![forks](https://img.shields.io/github/forks/kx00007/CVE-2026-29041.svg)


## CVE-2026-27541
 Incorrect Privilege Assignment vulnerability in Josh Kohlbach Wholesale Suite woocommerce-wholesale-prices allows Privilege Escalation.This issue affects Wholesale Suite: from n/a through = 2.2.6.

- [https://github.com/rootdirective-sec/CVE-2026-27541-Analysis-Lab](https://github.com/rootdirective-sec/CVE-2026-27541-Analysis-Lab) :  ![starts](https://img.shields.io/github/stars/rootdirective-sec/CVE-2026-27541-Analysis-Lab.svg) ![forks](https://img.shields.io/github/forks/rootdirective-sec/CVE-2026-27541-Analysis-Lab.svg)


## CVE-2026-27540
 Unrestricted Upload of File with Dangerous Type vulnerability in Rymera Web Co Pty Ltd. Woocommerce Wholesale Lead Capture allows Using Malicious Files.This issue affects Woocommerce Wholesale Lead Capture: from n/a through 2.0.3.1.

- [https://github.com/DeadExpl0it/CVE-2026-27540-WordPress-Exploit-PoC](https://github.com/DeadExpl0it/CVE-2026-27540-WordPress-Exploit-PoC) :  ![starts](https://img.shields.io/github/stars/DeadExpl0it/CVE-2026-27540-WordPress-Exploit-PoC.svg) ![forks](https://img.shields.io/github/forks/DeadExpl0it/CVE-2026-27540-WordPress-Exploit-PoC.svg)


## CVE-2026-24291
 Incorrect permission assignment for critical resource in Windows Accessibility Infrastructure (ATBroker.exe) allows an authorized attacker to elevate privileges locally.

- [https://github.com/lennertdefauw/CVE-2026-24291](https://github.com/lennertdefauw/CVE-2026-24291) :  ![starts](https://img.shields.io/github/stars/lennertdefauw/CVE-2026-24291.svg) ![forks](https://img.shields.io/github/forks/lennertdefauw/CVE-2026-24291.svg)


## CVE-2026-3888
 Local privilege escalation in snapd on Linux allows local attackers to get root privilege by re-creating snap's private /tmp directory when systemd-tmpfiles is configured to automatically clean up this directory. This issue affects Ubuntu 16.04 LTS, 18.04 LTS, 20.04 LTS, 22.04 LTS, and 24.04 LTS.

- [https://github.com/Many-Hat-Group/Ubuntu-CVE-2026-3888-patcher](https://github.com/Many-Hat-Group/Ubuntu-CVE-2026-3888-patcher) :  ![starts](https://img.shields.io/github/stars/Many-Hat-Group/Ubuntu-CVE-2026-3888-patcher.svg) ![forks](https://img.shields.io/github/forks/Many-Hat-Group/Ubuntu-CVE-2026-3888-patcher.svg)


## CVE-2025-71260
 BMC FootPrints ITSM versions 20.20.02 through 20.24.01.001 contain a deserialization of untrusted data vulnerability in the ASP.NET servlet's VIEWSTATE handling that allows authenticated attackers to execute arbitrary code. Attackers can supply crafted serialized objects to the VIEWSTATE parameter to achieve remote code execution and fully compromise the application. The following hotfixes remediate the vulnerability: 20.20.02, 20.20.03.002, 20.21.01.001, 20.21.02.002, 20.22.01, 20.22.01.001, 20.23.01, 20.23.01.002, and 20.24.01.

- [https://github.com/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260](https://github.com/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260) :  ![starts](https://img.shields.io/github/stars/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260.svg) ![forks](https://img.shields.io/github/forks/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260.svg)


## CVE-2025-71257
 BMC FootPrints ITSM versions 20.20.02 through 20.24.01.001 contain an authentication bypass vulnerability due to improper enforcement of security filters on restricted REST API endpoints and servlets. Unauthenticated remote attackers can bypass access controls to invoke restricted functionality and gain unauthorized access to application data and modify system resources. The following hotfixes remediate the vulnerability: 20.20.02, 20.20.03.002, 20.21.01.001, 20.21.02.002, 20.22.01, 20.22.01.001, 20.23.01, 20.23.01.002, and 20.24.01.

- [https://github.com/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260](https://github.com/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260) :  ![starts](https://img.shields.io/github/stars/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260.svg) ![forks](https://img.shields.io/github/forks/watchtowrlabs/watchTowr-vs-BMC-Footprints-RCE-CVE-2025-71257-CVE-2025-71260.svg)


## CVE-2025-69720
 ncurses v6.5 and v6.4 are vulnerable to Buffer Overflow in progs/infocmp.c, function analyze_string().

- [https://github.com/Cao-Wuhui/CVE-2025-69720](https://github.com/Cao-Wuhui/CVE-2025-69720) :  ![starts](https://img.shields.io/github/stars/Cao-Wuhui/CVE-2025-69720.svg) ![forks](https://img.shields.io/github/forks/Cao-Wuhui/CVE-2025-69720.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg)


## CVE-2025-54236
 Adobe Commerce versions 2.4.9-alpha2, 2.4.8-p2, 2.4.7-p7, 2.4.6-p12, 2.4.5-p14, 2.4.4-p15 and earlier are affected by an Improper Input Validation vulnerability. A successful attacker can abuse this to achieve session takeover, increasing the confidentiality, and integrity impact to high. Exploitation of this issue does not require user interaction.

- [https://github.com/alexb616/SessionReaper-CVE-2025-54236](https://github.com/alexb616/SessionReaper-CVE-2025-54236) :  ![starts](https://img.shields.io/github/stars/alexb616/SessionReaper-CVE-2025-54236.svg) ![forks](https://img.shields.io/github/forks/alexb616/SessionReaper-CVE-2025-54236.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/maronnjapan/claude-create-CVE-2025-29927](https://github.com/maronnjapan/claude-create-CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/maronnjapan/claude-create-CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/maronnjapan/claude-create-CVE-2025-29927.svg)


## CVE-2025-21420
 Windows Disk Cleanup Tool Elevation of Privilege Vulnerability

- [https://github.com/Dmitri131313/CVE-2025-21420-PoC](https://github.com/Dmitri131313/CVE-2025-21420-PoC) :  ![starts](https://img.shields.io/github/stars/Dmitri131313/CVE-2025-21420-PoC.svg) ![forks](https://img.shields.io/github/forks/Dmitri131313/CVE-2025-21420-PoC.svg)


## CVE-2025-10147
 The Podlove Podcast Publisher plugin for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the 'move_as_original_file' function in all versions up to, and including, 4.2.6. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/ghostpel-sec/CVE-2025-10147](https://github.com/ghostpel-sec/CVE-2025-10147) :  ![starts](https://img.shields.io/github/stars/ghostpel-sec/CVE-2025-10147.svg) ![forks](https://img.shields.io/github/forks/ghostpel-sec/CVE-2025-10147.svg)


## CVE-2025-2026
An authenticated remote attacker with web read-only privileges can exploit the vulnerable API to inject malicious input. Successful exploitation may cause the device to reboot, disrupting normal operations and causing a temporary denial of service.

- [https://github.com/magercode/List-CVE-2025-2026](https://github.com/magercode/List-CVE-2025-2026) :  ![starts](https://img.shields.io/github/stars/magercode/List-CVE-2025-2026.svg) ![forks](https://img.shields.io/github/forks/magercode/List-CVE-2025-2026.svg)


## CVE-2025-1304
 The NewsBlogger theme for WordPress is vulnerable to arbitrary file uploads due to a missing capability check on the newsblogger_install_and_activate_plugin() function in all versions up to, and including, 0.2.5.1. This makes it possible for authenticated attackers, with subscriber-level access and above, to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/Nxploited/CVE-2025-1304](https://github.com/Nxploited/CVE-2025-1304) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-1304.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-1304.svg)


## CVE-2024-51482
 ZoneMinder is a free, open source closed-circuit television software application. ZoneMinder v1.37.* = 1.37.64 is vulnerable to boolean-based SQL Injection in function of web/ajax/event.php. This is fixed in 1.37.65.

- [https://github.com/Erhui-Li/CVE-2024-51482-ZoneMinder-CCTV-HTB-Reliable-EXP](https://github.com/Erhui-Li/CVE-2024-51482-ZoneMinder-CCTV-HTB-Reliable-EXP) :  ![starts](https://img.shields.io/github/stars/Erhui-Li/CVE-2024-51482-ZoneMinder-CCTV-HTB-Reliable-EXP.svg) ![forks](https://img.shields.io/github/forks/Erhui-Li/CVE-2024-51482-ZoneMinder-CCTV-HTB-Reliable-EXP.svg)


## CVE-2024-48510
 Directory Traversal vulnerability in DotNetZip v.1.16.0 and before allows a remote attacker to execute arbitrary code via the src/Zip.Shared/ZipEntry.Extract.cs component NOTE: This vulnerability only affects products that are no longer supported by the maintainer.

- [https://github.com/havertz2110/CVE-2024-48510-PoC](https://github.com/havertz2110/CVE-2024-48510-PoC) :  ![starts](https://img.shields.io/github/stars/havertz2110/CVE-2024-48510-PoC.svg) ![forks](https://img.shields.io/github/forks/havertz2110/CVE-2024-48510-PoC.svg)


## CVE-2024-27304
 pgx is a PostgreSQL driver and toolkit for Go. SQL injection can occur if an attacker can cause a single query or bind message to exceed 4 GB in size. An integer overflow in the calculated message size can cause the one large message to be sent as multiple messages under the attacker's control. The problem is resolved in v4.18.2 and v5.5.4. As a workaround, reject user input large enough to cause a single query or bind message to exceed 4 GB in size.

- [https://github.com/flying-owl/Go-PGX-Vulnerability-POC-Public-Mirror](https://github.com/flying-owl/Go-PGX-Vulnerability-POC-Public-Mirror) :  ![starts](https://img.shields.io/github/stars/flying-owl/Go-PGX-Vulnerability-POC-Public-Mirror.svg) ![forks](https://img.shields.io/github/forks/flying-owl/Go-PGX-Vulnerability-POC-Public-Mirror.svg)


## CVE-2024-25081
 Splinefont in FontForge through 20230101 allows command injection via crafted filenames.

- [https://github.com/InzegoSec/CVE-2024-25081_2025-47273](https://github.com/InzegoSec/CVE-2024-25081_2025-47273) :  ![starts](https://img.shields.io/github/stars/InzegoSec/CVE-2024-25081_2025-47273.svg) ![forks](https://img.shields.io/github/forks/InzegoSec/CVE-2024-25081_2025-47273.svg)


## CVE-2024-8504
 An attacker with authenticated access to VICIdial as an "agent" can execute arbitrary shell commands as the "root" user. This attack can be chained with CVE-2024-8503 to execute arbitrary shell commands starting from an unauthenticated perspective.

- [https://github.com/Chocapikk/CVE-2024-8504](https://github.com/Chocapikk/CVE-2024-8504) :  ![starts](https://img.shields.io/github/stars/Chocapikk/CVE-2024-8504.svg) ![forks](https://img.shields.io/github/forks/Chocapikk/CVE-2024-8504.svg)
- [https://github.com/havokzero/ViciDial](https://github.com/havokzero/ViciDial) :  ![starts](https://img.shields.io/github/stars/havokzero/ViciDial.svg) ![forks](https://img.shields.io/github/forks/havokzero/ViciDial.svg)


## CVE-2022-39299
 Passport-SAML is a SAML 2.0 authentication provider for Passport, the Node.js authentication library. A remote attacker may be able to bypass SAML authentication on a website using passport-saml. A successful attack requires that the attacker is in possession of an arbitrary IDP signed XML element. Depending on the IDP used, fully unauthenticated attacks (e.g without access to a valid user) might also be feasible if generation of a signed message can be triggered. Users should upgrade to passport-saml version 3.2.2 or newer. The issue was also present in the beta releases of `node-saml` before version 4.0.0-beta.5. If you cannot upgrade, disabling SAML authentication may be done as a workaround.

- [https://github.com/KaztoRay/CVE-2022-39299-Research](https://github.com/KaztoRay/CVE-2022-39299-Research) :  ![starts](https://img.shields.io/github/stars/KaztoRay/CVE-2022-39299-Research.svg) ![forks](https://img.shields.io/github/forks/KaztoRay/CVE-2022-39299-Research.svg)


## CVE-2022-31798
 Nortek Linear eMerge E3-Series 0.32-07p devices are vulnerable to /card_scan.php?CardFormatNo= XSS with session fixation (via PHPSESSID) when they are chained together. This would allow an attacker to take over an admin account or a user account.

- [https://github.com/omarhashem123/CVE-2022-31798](https://github.com/omarhashem123/CVE-2022-31798) :  ![starts](https://img.shields.io/github/stars/omarhashem123/CVE-2022-31798.svg) ![forks](https://img.shields.io/github/forks/omarhashem123/CVE-2022-31798.svg)


## CVE-2019-1003000
 A sandbox bypass vulnerability exists in Script Security Plugin 1.49 and earlier in src/main/java/org/jenkinsci/plugins/scriptsecurity/sandbox/groovy/GroovySandbox.java that allows attackers with the ability to provide sandboxed scripts to execute arbitrary code on the Jenkins master JVM.

- [https://github.com/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins](https://github.com/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins) :  ![starts](https://img.shields.io/github/stars/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins.svg) ![forks](https://img.shields.io/github/forks/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins.svg)


## CVE-2019-17570
 An untrusted deserialization was found in the org.apache.xmlrpc.parser.XmlRpcResponseParser:addResult method of Apache XML-RPC (aka ws-xmlrpc) library. A malicious XML-RPC server could target a XML-RPC client causing it to execute arbitrary code. Apache XML-RPC is no longer maintained and this issue will not be fixed.

- [https://github.com/im23pds/xmlrpc-common-deserialization](https://github.com/im23pds/xmlrpc-common-deserialization) :  ![starts](https://img.shields.io/github/stars/im23pds/xmlrpc-common-deserialization.svg) ![forks](https://img.shields.io/github/forks/im23pds/xmlrpc-common-deserialization.svg)


## CVE-2019-0232
 When running on Windows with enableCmdLineArguments enabled, the CGI Servlet in Apache Tomcat 9.0.0.M1 to 9.0.17, 8.5.0 to 8.5.39 and 7.0.0 to 7.0.93 is vulnerable to Remote Code Execution due to a bug in the way the JRE passes command line arguments to Windows. The CGI Servlet is disabled by default. The CGI option enableCmdLineArguments is disable by default in Tomcat 9.0.x (and will be disabled by default in all versions in response to this vulnerability). For a detailed explanation of the JRE behaviour, see Markus Wulftange's blog (https://codewhitesec.blogspot.com/2016/02/java-and-command-line-injections-in-windows.html) and this archived MSDN blog (https://web.archive.org/web/20161228144344/https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/).

- [https://github.com/r4vl1t0/CVE-2019-0232](https://github.com/r4vl1t0/CVE-2019-0232) :  ![starts](https://img.shields.io/github/stars/r4vl1t0/CVE-2019-0232.svg) ![forks](https://img.shields.io/github/forks/r4vl1t0/CVE-2019-0232.svg)


## CVE-2018-1999002
 A arbitrary file read vulnerability exists in Jenkins 2.132 and earlier, 2.121.1 and earlier in the Stapler web framework's org/kohsuke/stapler/Stapler.java that allows attackers to send crafted HTTP requests returning the contents of any file on the Jenkins master file system that the Jenkins master has access to.

- [https://github.com/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins](https://github.com/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins) :  ![starts](https://img.shields.io/github/stars/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins.svg) ![forks](https://img.shields.io/github/forks/im23pds/CVE-2019-1003000-and-CVE-2018-1999002-Pre-Auth-RCE-Jenkins.svg)


## CVE-2018-7843
 A CWE-248: Uncaught Exception vulnerability exists in all versions of the Modicon M580, Modicon M340, Modicon Quantum, and Modicon Premium which could cause denial of service when reading memory blocks with an invalid data size or with an invalid data offset in the controller over Modbus.

- [https://github.com/yanissec/CVE-2018-7843](https://github.com/yanissec/CVE-2018-7843) :  ![starts](https://img.shields.io/github/stars/yanissec/CVE-2018-7843.svg) ![forks](https://img.shields.io/github/forks/yanissec/CVE-2018-7843.svg)

