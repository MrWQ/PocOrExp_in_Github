# Update 2026-04-12
## CVE-2026-39983
 basic-ftp is an FTP client for Node.js. Prior to 5.2.1, basic-ftp allows FTP command injection via CRLF sequences (\r\n) in file path parameters passed to high-level path APIs such as cd(), remove(), rename(), uploadFrom(), downloadTo(), list(), and removeDir(). The library's protectWhitespace() helper only handles leading spaces and returns other paths unchanged, while FtpContext.send() writes the resulting command string directly to the control socket with \r\n appended. This lets attacker-controlled path strings split one intended FTP command into multiple commands. This vulnerability is fixed in 5.2.1.

- [https://github.com/zebbernCVE/CVE-2026-39983](https://github.com/zebbernCVE/CVE-2026-39983) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-39983.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-39983.svg)


## CVE-2026-39376
 FastFeedParser is a high performance RSS, Atom and RDF parser. Prior to 0.5.10, when parse() fetches a URL that returns an HTML page containing a meta http-equiv="refresh" tag, it recursively calls itself with the redirect URL — with no depth limit, no visited-URL deduplication, and no redirect count cap. An attacker-controlled server that returns an infinite chain of HTML meta-refresh responses causes unbounded recursion, exhausting the Python call stack and crashing the process. This vulnerability can also be chained with the companion SSRF issue to reach internal network targets after bypassing the initial URL check. This vulnerability is fixed in 0.5.10.

- [https://github.com/redyank/CVE-2026-39376](https://github.com/redyank/CVE-2026-39376) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-39376.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-39376.svg)


## CVE-2026-35584
 FreeScout is a free help desk and shared inbox built with PHP's Laravel framework. Prior to 1.8.212, the endpoint GET /thread/read/{conversation_id}/{thread_id} does not require authentication and does not validate whether the given thread_id belongs to the given conversation_id. This allows any unauthenticated attacker to mark any thread as read by passing arbitrary IDs, enumerate valid thread IDs via HTTP response codes (200 vs 404), and manipulate opened_at timestamps across conversations (IDOR). This vulnerability is fixed in 1.8.212.

- [https://github.com/LeonardoNovais7/CVE-2026-35584](https://github.com/LeonardoNovais7/CVE-2026-35584) :  ![starts](https://img.shields.io/github/stars/LeonardoNovais7/CVE-2026-35584.svg) ![forks](https://img.shields.io/github/forks/LeonardoNovais7/CVE-2026-35584.svg)


## CVE-2026-34197
Users are recommended to upgrade to version 5.19.4 or 6.2.3, which fixes the issue

- [https://github.com/hg0434hongzh0/CVE-2026-34197](https://github.com/hg0434hongzh0/CVE-2026-34197) :  ![starts](https://img.shields.io/github/stars/hg0434hongzh0/CVE-2026-34197.svg) ![forks](https://img.shields.io/github/forks/hg0434hongzh0/CVE-2026-34197.svg)


## CVE-2026-33033
Django would like to thank Seokchan Yoon for reporting this issue.

- [https://github.com/ch4n3-yoon/CVE-2026-33033-PoC](https://github.com/ch4n3-yoon/CVE-2026-33033-PoC) :  ![starts](https://img.shields.io/github/stars/ch4n3-yoon/CVE-2026-33033-PoC.svg) ![forks](https://img.shields.io/github/forks/ch4n3-yoon/CVE-2026-33033-PoC.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/masterwok/CVE-2026-33017-Langflow-PoC](https://github.com/masterwok/CVE-2026-33017-Langflow-PoC) :  ![starts](https://img.shields.io/github/stars/masterwok/CVE-2026-33017-Langflow-PoC.svg) ![forks](https://img.shields.io/github/forks/masterwok/CVE-2026-33017-Langflow-PoC.svg)


## CVE-2026-29923
 The pstrip64.sys driver in EnTech Taiwan PowerStrip =3.90.736 allows local users to escalate privileges to SYSTEM via a crafted IOCTL request enabling unprivileged users to map arbitrary physical memory into their address space and modify critical kernel structures.

- [https://github.com/athenasec16/CVE-2026-29923](https://github.com/athenasec16/CVE-2026-29923) :  ![starts](https://img.shields.io/github/stars/athenasec16/CVE-2026-29923.svg) ![forks](https://img.shields.io/github/forks/athenasec16/CVE-2026-29923.svg)


## CVE-2026-29861
 PHP-MYSQL-User-Login-System v1.0 was discovered to contain a SQL injection vulnerability via the username parameter at login.php.

- [https://github.com/amanyadav78/CVE-2026-29861](https://github.com/amanyadav78/CVE-2026-29861) :  ![starts](https://img.shields.io/github/stars/amanyadav78/CVE-2026-29861.svg) ![forks](https://img.shields.io/github/forks/amanyadav78/CVE-2026-29861.svg)


## CVE-2026-29000
 pac4j-jwt versions prior to 4.5.9, 5.7.9, and 6.3.3 contain an authentication bypass vulnerability in JwtAuthenticator when processing encrypted JWTs that allows remote attackers to forge authentication tokens. Attackers who possess the server's RSA public key can create a JWE-wrapped PlainJWT with arbitrary subject and role claims, bypassing signature verification to authenticate as any user including administrators.

- [https://github.com/Gajraj238/CVE-2026-29000](https://github.com/Gajraj238/CVE-2026-29000) :  ![starts](https://img.shields.io/github/stars/Gajraj238/CVE-2026-29000.svg) ![forks](https://img.shields.io/github/forks/Gajraj238/CVE-2026-29000.svg)


## CVE-2026-23869
 A denial of service vulnerability exists in React Server Components, affecting the following packages: react-server-dom-parcel, react-server-dom-turbopack and react-server-dom-webpack (versions 19.0.0 through 19.0.4, 19.1.0 through 19.1.5, and 19.2.0 through 19.2.4). The vulnerability is triggered by sending specially crafted HTTP requests to Server Function endpoints.The payload of the HTTP request causes excessive CPU usage for up to a minute ending in a thrown error that is catchable.

- [https://github.com/yohannslm/CVE-2026-23869](https://github.com/yohannslm/CVE-2026-23869) :  ![starts](https://img.shields.io/github/stars/yohannslm/CVE-2026-23869.svg) ![forks](https://img.shields.io/github/forks/yohannslm/CVE-2026-23869.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/luiskrnr/exploit-CVE-2026-23744](https://github.com/luiskrnr/exploit-CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/luiskrnr/exploit-CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/luiskrnr/exploit-CVE-2026-23744.svg)


## CVE-2026-5530
 A flaw has been found in Ollama up to 18.1. This issue affects some unknown processing of the file server/download.go of the component Model Pull API. Executing a manipulation can lead to server-side request forgery. The attack can be launched remotely. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/davidrxchester/CVE-2026-5530](https://github.com/davidrxchester/CVE-2026-5530) :  ![starts](https://img.shields.io/github/stars/davidrxchester/CVE-2026-5530.svg) ![forks](https://img.shields.io/github/forks/davidrxchester/CVE-2026-5530.svg)


## CVE-2026-4747
In userspace, applications which have librpcgss_sec loaded and run an RPC server are vulnerable to remote code execution from any client able to send it packets.  We are not aware of any such applications in the FreeBSD base system.

- [https://github.com/kaleth4/CVE-2026-4747-](https://github.com/kaleth4/CVE-2026-4747-) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-4747-.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-4747-.svg)


## CVE-2026-4660
 HashiCorp’s go-getter library up to v1.8.5 may allow arbitrary file reads on the file system during certain git operations through a maliciously crafted URL. This vulnerability, CVE-2026-4660, is fixed in go-getter v1.8.6. This vulnerability does not affect the go-getter/v2 branch and package.

- [https://github.com/gouldnicholas/CVE-2026-4660-PoC](https://github.com/gouldnicholas/CVE-2026-4660-PoC) :  ![starts](https://img.shields.io/github/stars/gouldnicholas/CVE-2026-4660-PoC.svg) ![forks](https://img.shields.io/github/forks/gouldnicholas/CVE-2026-4660-PoC.svg)


## CVE-2026-3909
 Out of bounds write in Skia in Google Chrome prior to 146.0.7680.75 allowed a remote attacker to perform out of bounds memory access via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/anansi2safe/CVE-2026-3909-PoC](https://github.com/anansi2safe/CVE-2026-3909-PoC) :  ![starts](https://img.shields.io/github/stars/anansi2safe/CVE-2026-3909-PoC.svg) ![forks](https://img.shields.io/github/forks/anansi2safe/CVE-2026-3909-PoC.svg)


## CVE-2026-1312
Django would like to thank Solomon Kebede for reporting this issue.

- [https://github.com/alpinine/CVE-2026-1312-Testing](https://github.com/alpinine/CVE-2026-1312-Testing) :  ![starts](https://img.shields.io/github/stars/alpinine/CVE-2026-1312-Testing.svg) ![forks](https://img.shields.io/github/forks/alpinine/CVE-2026-1312-Testing.svg)


## CVE-2026-0740
 The Ninja Forms - File Uploads plugin for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the 'NF_FU_AJAX_Controllers_Uploads::handle_upload' function in all versions up to, and including, 3.3.26. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible. Note: The vulnerability was partially patched in version 3.3.25 and fully patched in version 3.3.27.

- [https://github.com/whattheslime/CVE-2026-0740](https://github.com/whattheslime/CVE-2026-0740) :  ![starts](https://img.shields.io/github/stars/whattheslime/CVE-2026-0740.svg) ![forks](https://img.shields.io/github/forks/whattheslime/CVE-2026-0740.svg)


## CVE-2025-54328
 An issue was discovered in SMS in Samsung Mobile Processor, Wearable Processor, and Modem Exynos 980, 990, 850, 1080, 2100, 1280, 2200, 1330, 1380, 1480, 2400, 1580, 2500, 9110, W920, W930, W1000, Modem 5123, Modem 5300, and Modem 5400. A Stack-based Buffer Overflow occurs while parsing SMS RP-DATA messages.

- [https://github.com/Hunt-Benito/samsung-exynos-sms-stack-overflow-cve-2025-54328-critical-zero-click-baseband-rce](https://github.com/Hunt-Benito/samsung-exynos-sms-stack-overflow-cve-2025-54328-critical-zero-click-baseband-rce) :  ![starts](https://img.shields.io/github/stars/Hunt-Benito/samsung-exynos-sms-stack-overflow-cve-2025-54328-critical-zero-click-baseband-rce.svg) ![forks](https://img.shields.io/github/forks/Hunt-Benito/samsung-exynos-sms-stack-overflow-cve-2025-54328-critical-zero-click-baseband-rce.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-14018
 Unquoted Search Path or Element vulnerability in NetBT Consulting Services Inc. E-Fatura allows Leveraging/Manipulating Configuration File Search Paths, Redirect Access to Libraries.This issue affects e-Fatura: before 1.2.15.

- [https://github.com/kaleth4/CVE-2025-14018](https://github.com/kaleth4/CVE-2025-14018) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2025-14018.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2025-14018.svg)


## CVE-2025-5548
 A vulnerability, which was classified as critical, was found in FreeFloat FTP Server 1.0. Affected is an unknown function of the component NOOP Command Handler. The manipulation leads to buffer overflow. It is possible to launch the attack remotely. The exploit has been disclosed to the public and may be used.

- [https://github.com/CryptoMachio/CVE-2025-5548](https://github.com/CryptoMachio/CVE-2025-5548) :  ![starts](https://img.shields.io/github/stars/CryptoMachio/CVE-2025-5548.svg) ![forks](https://img.shields.io/github/forks/CryptoMachio/CVE-2025-5548.svg)


## CVE-2023-6553
 The Backup Migration plugin for WordPress is vulnerable to Remote Code Execution in all versions up to, and including, 1.3.7 via the /includes/backup-heart.php file. This is due to an attacker being able to control the values passed to an include, and subsequently leverage that to achieve remote code execution. This makes it possible for unauthenticated attackers to easily execute code on the server.

- [https://github.com/Aliyankhan-source/CVE-2023-6553-RCE-Fancy-Exploit](https://github.com/Aliyankhan-source/CVE-2023-6553-RCE-Fancy-Exploit) :  ![starts](https://img.shields.io/github/stars/Aliyankhan-source/CVE-2023-6553-RCE-Fancy-Exploit.svg) ![forks](https://img.shields.io/github/forks/Aliyankhan-source/CVE-2023-6553-RCE-Fancy-Exploit.svg)


## CVE-2022-41055
 Windows Human Interface Device Information Disclosure Vulnerability

- [https://github.com/TroyWarez/hid_pwn](https://github.com/TroyWarez/hid_pwn) :  ![starts](https://img.shields.io/github/stars/TroyWarez/hid_pwn.svg) ![forks](https://img.shields.io/github/forks/TroyWarez/hid_pwn.svg)


## CVE-2022-30190
Please see the MSRC Blog Entry for important information about steps you can take to protect your system from this vulnerability.

- [https://github.com/shndnth/CVE-2022-30190](https://github.com/shndnth/CVE-2022-30190) :  ![starts](https://img.shields.io/github/stars/shndnth/CVE-2022-30190.svg) ![forks](https://img.shields.io/github/forks/shndnth/CVE-2022-30190.svg)


## CVE-2022-0847
 A flaw was found in the way the "flags" member of the new pipe buffer structure was lacking proper initialization in copy_page_to_iter_pipe and push_pipe functions in the Linux kernel and could thus contain stale values. An unprivileged local user could use this flaw to write to pages in the page cache backed by read only files and as such escalate their privileges on the system.

- [https://github.com/AyoubNajim/cve-2022-0847dirtypipe-exploit](https://github.com/AyoubNajim/cve-2022-0847dirtypipe-exploit) :  ![starts](https://img.shields.io/github/stars/AyoubNajim/cve-2022-0847dirtypipe-exploit.svg) ![forks](https://img.shields.io/github/forks/AyoubNajim/cve-2022-0847dirtypipe-exploit.svg)


## CVE-2021-42574
 An issue was discovered in the Bidirectional Algorithm in the Unicode Specification through 14.0. It permits the visual reordering of characters via control sequences, which can be used to craft source code that renders different logic than the logical ordering of tokens ingested by compilers and interpreters. Adversaries can leverage this to encode source code for compilers accepting Unicode such that targeted vulnerabilities are introduced invisibly to human reviewers. NOTE: the Unicode Consortium offers the following alternative approach to presenting this concern. An issue is noted in the nature of international text that can affect applications that implement support for The Unicode Standard and the Unicode Bidirectional Algorithm (all versions). Due to text display behavior when text includes left-to-right and right-to-left characters, the visual order of tokens may be different from their logical order. Additionally, control characters needed to fully support the requirements of bidirectional text can further obfuscate the logical order of tokens. Unless mitigated, an adversary could craft source code such that the ordering of tokens perceived by human reviewers does not match what will be processed by a compiler/interpreter/etc. The Unicode Consortium has documented this class of vulnerability in its document, Unicode Technical Report #36, Unicode Security Considerations. The Unicode Consortium also provides guidance on mitigations for this class of issues in Unicode Technical Standard #39, Unicode Security Mechanisms, and in Unicode Standard Annex #31, Unicode Identifier and Pattern Syntax. Also, the BIDI specification allows applications to tailor the implementation in ways that can mitigate misleading visual reordering in program text; see HL4 in Unicode Standard Annex #9, Unicode Bidirectional Algorithm.

- [https://github.com/simplylu/CVE-2021-42574](https://github.com/simplylu/CVE-2021-42574) :  ![starts](https://img.shields.io/github/stars/simplylu/CVE-2021-42574.svg) ![forks](https://img.shields.io/github/forks/simplylu/CVE-2021-42574.svg)
- [https://github.com/maweil/bidi_char_detector](https://github.com/maweil/bidi_char_detector) :  ![starts](https://img.shields.io/github/stars/maweil/bidi_char_detector.svg) ![forks](https://img.shields.io/github/forks/maweil/bidi_char_detector.svg)
- [https://github.com/tin-z/solidity_CVE-2021-42574-POC](https://github.com/tin-z/solidity_CVE-2021-42574-POC) :  ![starts](https://img.shields.io/github/stars/tin-z/solidity_CVE-2021-42574-POC.svg) ![forks](https://img.shields.io/github/forks/tin-z/solidity_CVE-2021-42574-POC.svg)
- [https://github.com/Moshe-ship/bidi-guard](https://github.com/Moshe-ship/bidi-guard) :  ![starts](https://img.shields.io/github/stars/Moshe-ship/bidi-guard.svg) ![forks](https://img.shields.io/github/forks/Moshe-ship/bidi-guard.svg)
- [https://github.com/shiomiyan/CVE-2021-42574](https://github.com/shiomiyan/CVE-2021-42574) :  ![starts](https://img.shields.io/github/stars/shiomiyan/CVE-2021-42574.svg) ![forks](https://img.shields.io/github/forks/shiomiyan/CVE-2021-42574.svg)
- [https://github.com/waseeld/CVE-2021-42574](https://github.com/waseeld/CVE-2021-42574) :  ![starts](https://img.shields.io/github/stars/waseeld/CVE-2021-42574.svg) ![forks](https://img.shields.io/github/forks/waseeld/CVE-2021-42574.svg)
- [https://github.com/hffaust/CVE-2021-42574_and_CVE-2021-42694](https://github.com/hffaust/CVE-2021-42574_and_CVE-2021-42694) :  ![starts](https://img.shields.io/github/stars/hffaust/CVE-2021-42574_and_CVE-2021-42694.svg) ![forks](https://img.shields.io/github/forks/hffaust/CVE-2021-42574_and_CVE-2021-42694.svg)
- [https://github.com/pierDipi/unicode-control-characters-action](https://github.com/pierDipi/unicode-control-characters-action) :  ![starts](https://img.shields.io/github/stars/pierDipi/unicode-control-characters-action.svg) ![forks](https://img.shields.io/github/forks/pierDipi/unicode-control-characters-action.svg)


## CVE-2021-22986
 On BIG-IP versions 16.0.x before 16.0.1.1, 15.1.x before 15.1.2.1, 14.1.x before 14.1.4, 13.1.x before 13.1.3.6, and 12.1.x before 12.1.5.3 amd BIG-IQ 7.1.0.x before 7.1.0.3 and 7.0.0.x before 7.0.0.2, the iControl REST interface has an unauthenticated remote command execution vulnerability. Note: Software versions which have reached End of Software Development (EoSD) are not evaluated.

- [https://github.com/whatheheckisthis/bigip-icontrol-rce-research](https://github.com/whatheheckisthis/bigip-icontrol-rce-research) :  ![starts](https://img.shields.io/github/stars/whatheheckisthis/bigip-icontrol-rce-research.svg) ![forks](https://img.shields.io/github/forks/whatheheckisthis/bigip-icontrol-rce-research.svg)


## CVE-2020-1472
When the second phase of Windows updates become available in Q1 2021, customers will be notified via a revision to this security vulnerability. If you wish to be notified when these updates are released, we recommend that you register for the security notifications mailer to be alerted of content changes to this advisory. See Microsoft Technical Security Notifications.

- [https://github.com/noemvex/apex-predator](https://github.com/noemvex/apex-predator) :  ![starts](https://img.shields.io/github/stars/noemvex/apex-predator.svg) ![forks](https://img.shields.io/github/forks/noemvex/apex-predator.svg)


## CVE-2019-15107
 An issue was discovered in Webmin =1.920. The parameter old in password_change.cgi contains a command injection vulnerability.

- [https://github.com/adampawelczyk/cve-2019-15107](https://github.com/adampawelczyk/cve-2019-15107) :  ![starts](https://img.shields.io/github/stars/adampawelczyk/cve-2019-15107.svg) ![forks](https://img.shields.io/github/forks/adampawelczyk/cve-2019-15107.svg)


## CVE-2017-5638
 The Jakarta Multipart parser in Apache Struts 2 2.3.x before 2.3.32 and 2.5.x before 2.5.10.1 has incorrect exception handling and error-message generation during file-upload attempts, which allows remote attackers to execute arbitrary commands via a crafted Content-Type, Content-Disposition, or Content-Length HTTP header, as exploited in the wild in March 2017 with a Content-Type header containing a #cmd= string.

- [https://github.com/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper](https://github.com/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper) :  ![starts](https://img.shields.io/github/stars/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper.svg) ![forks](https://img.shields.io/github/forks/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper.svg)


## CVE-2010-2075
 UnrealIRCd 3.2.8.1, as distributed on certain mirror sites from November 2009 through June 2010, contains an externally introduced modification (Trojan Horse) in the DEBUG3_DOLOG_SYSTEM macro, which allows remote attackers to execute arbitrary commands.

- [https://github.com/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report](https://github.com/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report) :  ![starts](https://img.shields.io/github/stars/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report.svg) ![forks](https://img.shields.io/github/forks/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report.svg)


## CVE-2007-2447
 The MS-RPC functionality in smbd in Samba 3.0.0 through 3.0.25rc3 allows remote attackers to execute arbitrary commands via shell metacharacters involving the (1) SamrChangePassword function, when the "username map script" smb.conf option is enabled, and allows remote authenticated users to execute commands via shell metacharacters involving other MS-RPC functions in the (2) remote printer and (3) file share management.

- [https://github.com/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report](https://github.com/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report) :  ![starts](https://img.shields.io/github/stars/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report.svg) ![forks](https://img.shields.io/github/forks/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report.svg)

