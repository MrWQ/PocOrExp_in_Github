# Update 2026-04-11
## CVE-2026-39912
 V2Board 1.6.1 through 1.7.4 and Xboard through 0.1.9 expose authentication tokens in HTTP response bodies of the loginWithMailLink endpoint when the login_with_mail_link_enable feature is active. Unauthenticated attackers can POST to the loginWithMailLink endpoint with a known email address to receive the full authentication URL in the response, then exchange the token at the token2Login endpoint to obtain a valid bearer token with complete account access including admin privileges.

- [https://github.com/Chocapikk/CVE-2026-39912](https://github.com/Chocapikk/CVE-2026-39912) :  ![starts](https://img.shields.io/github/stars/Chocapikk/CVE-2026-39912.svg) ![forks](https://img.shields.io/github/forks/Chocapikk/CVE-2026-39912.svg)


## CVE-2026-34724
 Zammad is a web based open source helpdesk/customer support system. Prior to 7.0.1, a server-side template injection vulnerability  which leads to RCE via AI Agent exists. Impact is limited to environments where an attacker can control or influence type_enrichment_data (typically high-privilege administrative configuration). This vulnerability is fixed in 7.0.1.

- [https://github.com/0xBlackash/CVE-2026-34724](https://github.com/0xBlackash/CVE-2026-34724) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-34724.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-34724.svg)


## CVE-2026-34197
Users are recommended to upgrade to version 5.19.4 or 6.2.3, which fixes the issue

- [https://github.com/AtoposX-J/CVE-2026-34197-Apache-ActiveMQ-RCE](https://github.com/AtoposX-J/CVE-2026-34197-Apache-ActiveMQ-RCE) :  ![starts](https://img.shields.io/github/stars/AtoposX-J/CVE-2026-34197-Apache-ActiveMQ-RCE.svg) ![forks](https://img.shields.io/github/forks/AtoposX-J/CVE-2026-34197-Apache-ActiveMQ-RCE.svg)
- [https://github.com/KONDORDEVSECURITYCORP/CVE-2026-34197](https://github.com/KONDORDEVSECURITYCORP/CVE-2026-34197) :  ![starts](https://img.shields.io/github/stars/KONDORDEVSECURITYCORP/CVE-2026-34197.svg) ![forks](https://img.shields.io/github/forks/KONDORDEVSECURITYCORP/CVE-2026-34197.svg)


## CVE-2026-31402
correct response on the original request.

- [https://github.com/0xBlackash/CVE-2026-31402](https://github.com/0xBlackash/CVE-2026-31402) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-31402.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-31402.svg)


## CVE-2026-29923
 The pstrip64.sys driver in EnTech Taiwan PowerStrip =3.90.736 allows local users to escalate privileges to SYSTEM via a crafted IOCTL request enabling unprivileged users to map arbitrary physical memory into their address space and modify critical kernel structures.

- [https://github.com/Smarttfoxx/CVE-2026-29923](https://github.com/Smarttfoxx/CVE-2026-29923) :  ![starts](https://img.shields.io/github/stars/Smarttfoxx/CVE-2026-29923.svg) ![forks](https://img.shields.io/github/forks/Smarttfoxx/CVE-2026-29923.svg)


## CVE-2026-21876
 The OWASP core rule set (CRS) is a set of generic attack detection rules for use with compatible web application firewalls. Prior to versions 4.22.0 and 3.3.8, the current rule 922110 has a bug when processing multipart requests with multiple parts. When the first rule in a chain iterates over a collection (like `MULTIPART_PART_HEADERS`), the capture variables (`TX:0`, `TX:1`) get overwritten with each iteration. Only the last captured value is available to the chained rule, which means malicious charsets in earlier parts can be missed if a later part has a legitimate charset. Versions 4.22.0 and 3.3.8 patch the issue.

- [https://github.com/Mefhika120/CVE-2026-21876](https://github.com/Mefhika120/CVE-2026-21876) :  ![starts](https://img.shields.io/github/stars/Mefhika120/CVE-2026-21876.svg) ![forks](https://img.shields.io/github/forks/Mefhika120/CVE-2026-21876.svg)


## CVE-2026-21858
 n8n is an open source workflow automation platform. Versions starting with 1.65.0 and below 1.121.0 enable an attacker to access files on the underlying server through execution of certain form-based workflows. A vulnerable workflow could grant access to an unauthenticated remote attacker, resulting in exposure of sensitive information stored on the system and may enable further compromise depending on deployment configuration and workflow usage. This issue is fixed in version 1.121.0.

- [https://github.com/kaleth4/CVE-2026-21858](https://github.com/kaleth4/CVE-2026-21858) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-21858.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-21858.svg)


## CVE-2026-5173
 GitLab has remediated an issue in GitLab CE/EE affecting all versions from 16.9.6 before 18.8.9, 18.9 before 18.9.5, and 18.10 before 18.10.3 that could have allowed an authenticated user to invoke unintended server-side methods through websocket connections due to improper access control.

- [https://github.com/0xBlackash/CVE-2026-5173](https://github.com/0xBlackash/CVE-2026-5173) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-5173.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-5173.svg)


## CVE-2026-4747
In userspace, applications which have librpcgss_sec loaded and run an RPC server are vulnerable to remote code execution from any client able to send it packets.  We are not aware of any such applications in the FreeBSD base system.

- [https://github.com/kaleth4/CVE-2026-4747](https://github.com/kaleth4/CVE-2026-4747) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-4747.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-4747.svg)


## CVE-2026-4257
 The Contact Form by Supsystic plugin for WordPress is vulnerable to Server-Side Template Injection (SSTI) leading to Remote Code Execution (RCE) in all versions up to, and including, 1.7.36. This is due to the plugin using the Twig `Twig_Loader_String` template engine without sandboxing, combined with the `cfsPreFill` prefill functionality that allows unauthenticated users to inject arbitrary Twig expressions into form field values via GET parameters. This makes it possible for unauthenticated attackers to execute arbitrary PHP functions and OS commands on the server by leveraging Twig's `registerUndefinedFilterCallback()` method to register arbitrary PHP callbacks.

- [https://github.com/bootstrapbool/cve-2026-4257](https://github.com/bootstrapbool/cve-2026-4257) :  ![starts](https://img.shields.io/github/stars/bootstrapbool/cve-2026-4257.svg) ![forks](https://img.shields.io/github/forks/bootstrapbool/cve-2026-4257.svg)


## CVE-2026-4112
 Improper neutralization of special elements used in an SQL command (“SQL Injection”) in SonicWall SMA1000 series appliances allows a remote authenticated attacker with read-only administrator privileges to escalate privileges to primary administrator.

- [https://github.com/Hann1bl3L3ct3r/CVE-2026-4112](https://github.com/Hann1bl3L3ct3r/CVE-2026-4112) :  ![starts](https://img.shields.io/github/stars/Hann1bl3L3ct3r/CVE-2026-4112.svg) ![forks](https://img.shields.io/github/forks/Hann1bl3L3ct3r/CVE-2026-4112.svg)


## CVE-2026-3516
 The Contact List plugin for WordPress is vulnerable to Stored Cross-Site Scripting via the '_cl_map_iframe' parameter in all versions up to, and including, 3.0.18. This is due to insufficient input sanitization and output escaping when handling the Google Maps iframe custom field. The saveCustomFields() function in class-contact-list-custom-fields.php uses a regex to extract iframe tags from user input but does not validate or sanitize the iframe's attributes, allowing event handlers like 'onload' to be included. The extracted iframe HTML is stored via update_post_meta() and later rendered on the front-end in class-cl-public-card.php without any escaping or wp_kses filtering. This makes it possible for authenticated attackers, with Contributor-level access and above, to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page.

- [https://github.com/d3kc4rt1/CVE-2026-3516](https://github.com/d3kc4rt1/CVE-2026-3516) :  ![starts](https://img.shields.io/github/stars/d3kc4rt1/CVE-2026-3516.svg) ![forks](https://img.shields.io/github/forks/d3kc4rt1/CVE-2026-3516.svg)


## CVE-2026-2796
 JIT miscompilation in the JavaScript: WebAssembly component. This vulnerability affects Firefox  148 and Thunderbird  148.

- [https://github.com/WostGit/CVE-2026-2796](https://github.com/WostGit/CVE-2026-2796) :  ![starts](https://img.shields.io/github/stars/WostGit/CVE-2026-2796.svg) ![forks](https://img.shields.io/github/forks/WostGit/CVE-2026-2796.svg)
- [https://github.com/WostGit/cve-2026-2796-repro](https://github.com/WostGit/cve-2026-2796-repro) :  ![starts](https://img.shields.io/github/stars/WostGit/cve-2026-2796-repro.svg) ![forks](https://img.shields.io/github/forks/WostGit/cve-2026-2796-repro.svg)


## CVE-2026-1657
 The EventPrime plugin for WordPress is vulnerable to unauthorized image file upload in all versions up to, and including, 4.2.8.4. This is due to the plugin registering the upload_file_media AJAX action as publicly accessible (nopriv-enabled) without implementing any authentication, authorization, or nonce verification despite a nonce being created. This makes it possible for unauthenticated attackers to upload image files to the WordPress uploads directory and create Media Library attachments via the ep_upload_file_media endpoint.

- [https://github.com/d3kc4rt1/CVE-2026-1657](https://github.com/d3kc4rt1/CVE-2026-1657) :  ![starts](https://img.shields.io/github/stars/d3kc4rt1/CVE-2026-1657.svg) ![forks](https://img.shields.io/github/forks/d3kc4rt1/CVE-2026-1657.svg)


## CVE-2026-1375
 The Tutor LMS – eLearning and online course solution plugin for WordPress is vulnerable to Insecure Direct Object References (IDOR) in all versions up to, and including, 3.9.5. This is due to missing object-level authorization checks in the `course_list_bulk_action()`, `bulk_delete_course()`, and `update_course_status()` functions. This makes it possible for authenticated attackers, with Tutor Instructor-level access and above, to modify or delete arbitrary courses they do not own by manipulating course IDs in bulk action requests.

- [https://github.com/d3kc4rt1/CVE-2026-1375](https://github.com/d3kc4rt1/CVE-2026-1375) :  ![starts](https://img.shields.io/github/stars/d3kc4rt1/CVE-2026-1375.svg) ![forks](https://img.shields.io/github/forks/d3kc4rt1/CVE-2026-1375.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-63353
 A vulnerability in FiberHome GPON ONU HG6145F1 RP4423 allows the device's factory default Wi-Fi password (WPA/WPA2 pre-shared key) to be predicted from the SSID. The device generates default passwords using a deterministic algorithm that derives the router passphrase from the SSID, enabling an attacker who can observe the SSID to predict the default password without authentication or user interaction.

- [https://github.com/r0otk3r/CVE-2025-63353](https://github.com/r0otk3r/CVE-2025-63353) :  ![starts](https://img.shields.io/github/stars/r0otk3r/CVE-2025-63353.svg) ![forks](https://img.shields.io/github/forks/r0otk3r/CVE-2025-63353.svg)


## CVE-2025-60709
 Out-of-bounds read in Windows Common Log File System Driver allows an authorized attacker to elevate privileges locally.

- [https://github.com/KONDORDEVSECURITYCORP/CVE-2025-60709](https://github.com/KONDORDEVSECURITYCORP/CVE-2025-60709) :  ![starts](https://img.shields.io/github/stars/KONDORDEVSECURITYCORP/CVE-2025-60709.svg) ![forks](https://img.shields.io/github/forks/KONDORDEVSECURITYCORP/CVE-2025-60709.svg)


## CVE-2025-54236
 Adobe Commerce versions 2.4.9-alpha2, 2.4.8-p2, 2.4.7-p7, 2.4.6-p12, 2.4.5-p14, 2.4.4-p15 and earlier are affected by an Improper Input Validation vulnerability. A successful attacker can abuse this to achieve session takeover, increasing the confidentiality, and integrity impact to high. Exploitation of this issue does not require user interaction.

- [https://github.com/nocerainfosec/polyshellv2.0](https://github.com/nocerainfosec/polyshellv2.0) :  ![starts](https://img.shields.io/github/stars/nocerainfosec/polyshellv2.0.svg) ![forks](https://img.shields.io/github/forks/nocerainfosec/polyshellv2.0.svg)


## CVE-2025-49596
 The MCP inspector is a developer tool for testing and debugging MCP servers. Versions of MCP Inspector below 0.14.1 are vulnerable to remote code execution due to lack of authentication between the Inspector client and proxy, allowing unauthenticated requests to launch MCP commands over stdio. Users should immediately upgrade to version 0.14.1 or later to address these vulnerabilities.

- [https://github.com/acseguin21/trust-boundary-ctf](https://github.com/acseguin21/trust-boundary-ctf) :  ![starts](https://img.shields.io/github/stars/acseguin21/trust-boundary-ctf.svg) ![forks](https://img.shields.io/github/forks/acseguin21/trust-boundary-ctf.svg)


## CVE-2025-49132
 Pterodactyl is a free, open-source game server management panel. Prior to version 1.11.11, using the /locales/locale.json with the locale and namespace query parameters, a malicious actor is able to execute arbitrary code without being authenticated. With the ability to execute arbitrary code it could be used to gain access to the Panel's server, read credentials from the Panel's config, extract sensitive information from the database, access files of servers managed by the panel, etc. This issue has been patched in version 1.11.11. There are no software workarounds for this vulnerability, but use of an external Web Application Firewall (WAF) could help mitigate this attack.

- [https://github.com/unixskid/CVE-2025-49132](https://github.com/unixskid/CVE-2025-49132) :  ![starts](https://img.shields.io/github/stars/unixskid/CVE-2025-49132.svg) ![forks](https://img.shields.io/github/forks/unixskid/CVE-2025-49132.svg)


## CVE-2025-47812
 In Wing FTP Server before 7.4.4. the user and admin web interfaces mishandle '\0' bytes, ultimately allowing injection of arbitrary Lua code into user session files. This can be used to execute arbitrary system commands with the privileges of the FTP service (root or SYSTEM by default). This is thus a remote code execution vulnerability that guarantees a total server compromise. This is also exploitable via anonymous FTP accounts.

- [https://github.com/Majdae/CVE-2025-47812-Research](https://github.com/Majdae/CVE-2025-47812-Research) :  ![starts](https://img.shields.io/github/stars/Majdae/CVE-2025-47812-Research.svg) ![forks](https://img.shields.io/github/forks/Majdae/CVE-2025-47812-Research.svg)


## CVE-2025-47273
 setuptools is a package that allows users to download, build, install, upgrade, and uninstall Python packages. A path traversal vulnerability in `PackageIndex` is present in setuptools prior to version 78.1.1. An attacker would be allowed to write files to arbitrary locations on the filesystem with the permissions of the process running the Python code, which could escalate to remote code execution depending on the context. Version 78.1.1 fixes the issue.

- [https://github.com/V0idW1re/HTB-VariaType-Writeup](https://github.com/V0idW1re/HTB-VariaType-Writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/HTB-VariaType-Writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/HTB-VariaType-Writeup.svg)


## CVE-2025-43990
 Dell Command Monitor (DCM), versions prior to 10.12.3.28, contains an Execution with Unnecessary Privileges vulnerability. A low privileged attacker with local access could potentially exploit this vulnerability, leading to Elevation of Privileges.

- [https://github.com/AMkkk221/CVE-2025-43990-Magento-RCE](https://github.com/AMkkk221/CVE-2025-43990-Magento-RCE) :  ![starts](https://img.shields.io/github/stars/AMkkk221/CVE-2025-43990-Magento-RCE.svg) ![forks](https://img.shields.io/github/forks/AMkkk221/CVE-2025-43990-Magento-RCE.svg)


## CVE-2025-34077
 An authentication bypass vulnerability exists in the WordPress Pie Register plugin ≤ 3.7.1.4 that allows unauthenticated attackers to impersonate arbitrary users by submitting a crafted POST request to the login endpoint. By setting social_site=true and manipulating the user_id_social_site parameter, an attacker can generate a valid WordPress session cookie for any user ID, including administrators. Once authenticated, the attacker may exploit plugin upload functionality to install a malicious plugin containing arbitrary PHP code, resulting in remote code execution on the underlying server.

- [https://github.com/salimelh94/Web-Penetration-Test](https://github.com/salimelh94/Web-Penetration-Test) :  ![starts](https://img.shields.io/github/stars/salimelh94/Web-Penetration-Test.svg) ![forks](https://img.shields.io/github/forks/salimelh94/Web-Penetration-Test.svg)


## CVE-2025-34037
 An OS command injection vulnerability exists in various models of E-Series Linksys routers via the /tmUnblock.cgi and /hndUnblock.cgi endpoints over HTTP on port 8080. The CGI scripts improperly process user-supplied input passed to the ttcp_ip parameter without sanitization, allowing unauthenticated attackers to inject shell commands. This vulnerability was reported to be exploited in the wild by the "TheMoon" worm  in 2014 to deploy a MIPS ELF payload, enabling arbitrary code execution on the router. Additionally, this vulnerability may affect other Linksys products to include, but not limited to, WAG/WAP/WES/WET/WRT-series router models and Wireless-N access points and routers. Exploitation evidence was observed by the Shadowserver Foundation on 2025-02-06 UTC.

- [https://github.com/Taxanehh/CVE-2025-34037](https://github.com/Taxanehh/CVE-2025-34037) :  ![starts](https://img.shields.io/github/stars/Taxanehh/CVE-2025-34037.svg) ![forks](https://img.shields.io/github/forks/Taxanehh/CVE-2025-34037.svg)


## CVE-2025-32433
 Erlang/OTP is a set of libraries for the Erlang programming language. Prior to versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20, a SSH server may allow an attacker to perform unauthenticated remote code execution (RCE). By exploiting a flaw in SSH protocol message handling, a malicious actor could gain unauthorized access to affected systems and execute arbitrary commands without valid credentials. This issue is patched in versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20. A temporary workaround involves disabling the SSH server or to prevent access via firewall rules.

- [https://github.com/0xBlackash/CVE-2025-32433](https://github.com/0xBlackash/CVE-2025-32433) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-32433.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-32433.svg)


## CVE-2025-31722
 In Jenkins Templating Engine Plugin 2.5.3 and earlier, libraries defined in folders are not subject to sandbox protection, allowing attackers with Item/Configure permission to execute arbitrary code in the context of the Jenkins controller JVM.

- [https://github.com/h3raklez/CVE-2025-31722](https://github.com/h3raklez/CVE-2025-31722) :  ![starts](https://img.shields.io/github/stars/h3raklez/CVE-2025-31722.svg) ![forks](https://img.shields.io/github/forks/h3raklez/CVE-2025-31722.svg)
- [https://github.com/Nick6371/CVE-2025-31722](https://github.com/Nick6371/CVE-2025-31722) :  ![starts](https://img.shields.io/github/stars/Nick6371/CVE-2025-31722.svg) ![forks](https://img.shields.io/github/forks/Nick6371/CVE-2025-31722.svg)


## CVE-2025-15260
 The MyRewards – Loyalty Points and Rewards for WooCommerce plugin for WordPress is vulnerable to missing authorization in all versions up to, and including, 5.6.1. This is due to the plugin not properly verifying that a user is authorized to perform an action in the 'ajax' function. This makes it possible for authenticated attackers, with subscriber level access and above, to modify, add, or delete loyalty program earning rules, including manipulating point multipliers to arbitrary values.

- [https://github.com/d3kc4rt1/CVE-2025-15260](https://github.com/d3kc4rt1/CVE-2025-15260) :  ![starts](https://img.shields.io/github/stars/d3kc4rt1/CVE-2025-15260.svg) ![forks](https://img.shields.io/github/forks/d3kc4rt1/CVE-2025-15260.svg)


## CVE-2025-14893
 The IndieWeb plugin for WordPress is vulnerable to Stored Cross-Site Scripting via the 'Telephone' parameter in all versions up to, and including, 4.0.5 due to insufficient input sanitization and output escaping. This makes it possible for authenticated attackers, with author level access and above, to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page.

- [https://github.com/d3kc4rt1/CVE-2025-14893](https://github.com/d3kc4rt1/CVE-2025-14893) :  ![starts](https://img.shields.io/github/stars/d3kc4rt1/CVE-2025-14893.svg) ![forks](https://img.shields.io/github/forks/d3kc4rt1/CVE-2025-14893.svg)


## CVE-2025-14325
 JIT miscompilation in the JavaScript Engine: JIT component. This vulnerability affects Firefox  146, Firefox ESR  140.6, Thunderbird  146, and Thunderbird  140.6.

- [https://github.com/WostGit/cve-2025-14325-full-repro](https://github.com/WostGit/cve-2025-14325-full-repro) :  ![starts](https://img.shields.io/github/stars/WostGit/cve-2025-14325-full-repro.svg) ![forks](https://img.shields.io/github/forks/WostGit/cve-2025-14325-full-repro.svg)


## CVE-2025-11187
not support PBMAC1 in PKCS#12.

- [https://github.com/x-stp/cves-2025-11187_15467_69418](https://github.com/x-stp/cves-2025-11187_15467_69418) :  ![starts](https://img.shields.io/github/stars/x-stp/cves-2025-11187_15467_69418.svg) ![forks](https://img.shields.io/github/forks/x-stp/cves-2025-11187_15467_69418.svg)


## CVE-2024-27766
 An issue in MariaDB v.11.1 allows a remote attacker to execute arbitrary code via the lib_mysqludf_sys.so function. NOTE: this is disputed by the MariaDB Foundation because no privilege boundary is crossed.

- [https://github.com/y0un9eee/CVE-2024-27766](https://github.com/y0un9eee/CVE-2024-27766) :  ![starts](https://img.shields.io/github/stars/y0un9eee/CVE-2024-27766.svg) ![forks](https://img.shields.io/github/forks/y0un9eee/CVE-2024-27766.svg)


## CVE-2024-3094
Through a series of complex obfuscations, the liblzma build process extracts a prebuilt object file from a disguised test file existing in the source code, which is then used to modify specific functions in the liblzma code. This results in a modified liblzma library that can be used by any software linked against this library, intercepting and modifying the data interaction with this library.

- [https://github.com/h3raklez/CVE-2024-3094](https://github.com/h3raklez/CVE-2024-3094) :  ![starts](https://img.shields.io/github/stars/h3raklez/CVE-2024-3094.svg) ![forks](https://img.shields.io/github/forks/h3raklez/CVE-2024-3094.svg)


## CVE-2023-33177
 Xibo is a content management system (CMS). A path traversal vulnerability exists in the Xibo CMS whereby a specially crafted zip file can be uploaded to the CMS via the layout import function by an authenticated user which would allow creation of files outside of the CMS library directory as the webserver user. This can be used to upload a PHP webshell inside the web root directory and achieve remote code execution as the webserver user. Users should upgrade to version 2.3.17 or 3.3.5, which fix this issue. Customers who host their CMS with Xibo Signage have already received an upgrade or patch to resolve this issue regardless of the CMS version that they are running.

- [https://github.com/kaxm23/-CVE-2023-33177-](https://github.com/kaxm23/-CVE-2023-33177-) :  ![starts](https://img.shields.io/github/stars/kaxm23/-CVE-2023-33177-.svg) ![forks](https://img.shields.io/github/forks/kaxm23/-CVE-2023-33177-.svg)


## CVE-2023-20198
 Cisco is providing an update for the ongoing investigation into observed exploitation of the web UI feature in Cisco IOS XE Software. We are updating the list of fixed releases and adding the Software Checker. Our investigation has determined that the actors exploited two previously unknown issues. The attacker first exploited CVE-2023-20198 to gain initial access and issued a privilege 15 command to create a local user and password combination. This allowed the user to log in with normal user access. The attacker then exploited another component of the web UI feature, leveraging the new local user to elevate privilege to root and write the implant to the file system. Cisco has assigned CVE-2023-20273 to this issue. CVE-2023-20198 has been assigned a CVSS Score of 10.0. CVE-2023-20273 has been assigned a CVSS Score of 7.2. Both of these CVEs are being tracked by CSCwh87343.

- [https://github.com/telly251/forwardnetworksdemo](https://github.com/telly251/forwardnetworksdemo) :  ![starts](https://img.shields.io/github/stars/telly251/forwardnetworksdemo.svg) ![forks](https://img.shields.io/github/forks/telly251/forwardnetworksdemo.svg)


## CVE-2022-22963
 In Spring Cloud Function versions 3.1.6, 3.2.2 and older unsupported versions, when using routing functionality it is possible for a user to provide a specially crafted SpEL as a routing-expression that may result in remote code execution and access to local resources.

- [https://github.com/C4yberLan/SpringBoot-Exploit-Toolkit](https://github.com/C4yberLan/SpringBoot-Exploit-Toolkit) :  ![starts](https://img.shields.io/github/stars/C4yberLan/SpringBoot-Exploit-Toolkit.svg) ![forks](https://img.shields.io/github/forks/C4yberLan/SpringBoot-Exploit-Toolkit.svg)


## CVE-2022-22947
 In spring cloud gateway versions prior to 3.1.1+ and 3.0.7+ , applications are vulnerable to a code injection attack when the Gateway Actuator endpoint is enabled, exposed and unsecured. A remote attacker could make a maliciously crafted request that could allow arbitrary remote execution on the remote host.

- [https://github.com/C4yberLan/SpringBoot-Exploit-Toolkit](https://github.com/C4yberLan/SpringBoot-Exploit-Toolkit) :  ![starts](https://img.shields.io/github/stars/C4yberLan/SpringBoot-Exploit-Toolkit.svg) ![forks](https://img.shields.io/github/forks/C4yberLan/SpringBoot-Exploit-Toolkit.svg)


## CVE-2022-0847
 A flaw was found in the way the "flags" member of the new pipe buffer structure was lacking proper initialization in copy_page_to_iter_pipe and push_pipe functions in the Linux kernel and could thus contain stale values. An unprivileged local user could use this flaw to write to pages in the page cache backed by read only files and as such escalate their privileges on the system.

- [https://github.com/Scouserr/cve-2022-0847-poc-dockerimage](https://github.com/Scouserr/cve-2022-0847-poc-dockerimage) :  ![starts](https://img.shields.io/github/stars/Scouserr/cve-2022-0847-poc-dockerimage.svg) ![forks](https://img.shields.io/github/forks/Scouserr/cve-2022-0847-poc-dockerimage.svg)


## CVE-2021-22911
 A improper input sanitization vulnerability exists in Rocket.Chat server 3.11, 3.12 & 3.13 that could lead to unauthenticated NoSQL injection, resulting potentially in RCE.

- [https://github.com/roshanrajbanshi/rocketcat-cve-2021-22911-exploit](https://github.com/roshanrajbanshi/rocketcat-cve-2021-22911-exploit) :  ![starts](https://img.shields.io/github/stars/roshanrajbanshi/rocketcat-cve-2021-22911-exploit.svg) ![forks](https://img.shields.io/github/forks/roshanrajbanshi/rocketcat-cve-2021-22911-exploit.svg)


## CVE-2018-16763
 FUEL CMS 1.4.1 allows PHP Code Evaluation via the pages/select/ filter parameter or the preview/ data parameter. This can lead to Pre-Auth Remote Code Execution.

- [https://github.com/estebanzarate/CVE-2018-16763-Fuel-CMS-1.4.1-Remote-Code-Execution-PoC](https://github.com/estebanzarate/CVE-2018-16763-Fuel-CMS-1.4.1-Remote-Code-Execution-PoC) :  ![starts](https://img.shields.io/github/stars/estebanzarate/CVE-2018-16763-Fuel-CMS-1.4.1-Remote-Code-Execution-PoC.svg) ![forks](https://img.shields.io/github/forks/estebanzarate/CVE-2018-16763-Fuel-CMS-1.4.1-Remote-Code-Execution-PoC.svg)


## CVE-2014-6271
 GNU Bash through 4.3 processes trailing strings after function definitions in the values of environment variables, which allows remote attackers to execute arbitrary code via a crafted environment, as demonstrated by vectors involving the ForceCommand feature in OpenSSH sshd, the mod_cgi and mod_cgid modules in the Apache HTTP Server, scripts executed by unspecified DHCP clients, and other situations in which setting the environment occurs across a privilege boundary from Bash execution, aka "ShellShock."  NOTE: the original fix for this issue was incorrect; CVE-2014-7169 has been assigned to cover the vulnerability that is still present after the incorrect fix.

- [https://github.com/kaleth4/CVE-2014-6271](https://github.com/kaleth4/CVE-2014-6271) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2014-6271.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2014-6271.svg)
- [https://github.com/kaleth4/-CVE-2014-6271](https://github.com/kaleth4/-CVE-2014-6271) :  ![starts](https://img.shields.io/github/stars/kaleth4/-CVE-2014-6271.svg) ![forks](https://img.shields.io/github/forks/kaleth4/-CVE-2014-6271.svg)


## CVE-2011-2523
 vsftpd 2.3.4 downloaded between 20110630 and 20110703 contains a backdoor which opens a shell on port 6200/tcp.

- [https://github.com/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report](https://github.com/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report) :  ![starts](https://img.shields.io/github/stars/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report.svg) ![forks](https://img.shields.io/github/forks/Nyabayo/flatiron-pentest-nmap-enum4linux-smb-ftp-samba-metasploitable2-kali-healthcare-report.svg)

