# Update 2026-03-28
## CVE-2026-33917
 OpenEMR is a free and open source electronic health records and medical practice management application. Versions prior to 8.0.0.3 contais a SQL injection vulnerability in the ajax_save CAMOS form that can be exploited by authenticated attackers. The vulnerability exists due to insufficient input validation in the ajax_save page in the CAMOS form. Version 8.0.0.3 patches the issue.

- [https://github.com/ChrisSub08/CVE-2026-33917_SqlInjectionVulnerabilityOpenEMR8.0.0](https://github.com/ChrisSub08/CVE-2026-33917_SqlInjectionVulnerabilityOpenEMR8.0.0) :  ![starts](https://img.shields.io/github/stars/ChrisSub08/CVE-2026-33917_SqlInjectionVulnerabilityOpenEMR8.0.0.svg) ![forks](https://img.shields.io/github/forks/ChrisSub08/CVE-2026-33917_SqlInjectionVulnerabilityOpenEMR8.0.0.svg)


## CVE-2026-33910
 OpenEMR is a free and open source electronic health records and medical practice management application. Versions up to and including 8.0.0.2 contain a SQL injection vulnerability in the patient selection feature that can be exploited by authenticated attackers. The vulnerability exists due to insufficient input validation in the patient selection feature. Version 8.0.0.3 contains a patch.

- [https://github.com/ChrisSub08/CVE-2026-33910_SqlInjectionVulnerabilityOpenEMR8.0.0.2](https://github.com/ChrisSub08/CVE-2026-33910_SqlInjectionVulnerabilityOpenEMR8.0.0.2) :  ![starts](https://img.shields.io/github/stars/ChrisSub08/CVE-2026-33910_SqlInjectionVulnerabilityOpenEMR8.0.0.2.svg) ![forks](https://img.shields.io/github/forks/ChrisSub08/CVE-2026-33910_SqlInjectionVulnerabilityOpenEMR8.0.0.2.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/rootdirective-sec/CVE-2026-33017-Lab](https://github.com/rootdirective-sec/CVE-2026-33017-Lab) :  ![starts](https://img.shields.io/github/stars/rootdirective-sec/CVE-2026-33017-Lab.svg) ![forks](https://img.shields.io/github/forks/rootdirective-sec/CVE-2026-33017-Lab.svg)


## CVE-2026-32746
 telnetd in GNU inetutils through 2.7 allows an out-of-bounds write in the LINEMODE SLC (Set Local Characters) suboption handler because add_slc does not check whether the buffer is full.

- [https://github.com/ekomsSavior/telnet_scan](https://github.com/ekomsSavior/telnet_scan) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/telnet_scan.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/telnet_scan.svg)


## CVE-2026-29905
 Kirby CMS through 5.1.4 allows an authenticated user with 'Editor' permissions to cause a persistent Denial of Service (DoS) via a malformed image upload. The application fails to properly validate the return value of the PHP getimagesize() function. When the system attempts to process this file for metadata or thumbnail generation, it triggers a fatal TypeError.

- [https://github.com/Stalin-143/CVE-2026-29905](https://github.com/Stalin-143/CVE-2026-29905) :  ![starts](https://img.shields.io/github/stars/Stalin-143/CVE-2026-29905.svg) ![forks](https://img.shields.io/github/forks/Stalin-143/CVE-2026-29905.svg)


## CVE-2026-29187
 OpenEMR is a free and open source electronic health records and medical practice management application. Prior to version 8.0.0.3, a Blind SQL Injection vulnerability exists in the Patient Search functionality (/interface/new/new_search_popup.php). The vulnerability allows an authenticated attacker to execute arbitrary SQL commands by manipulating the HTTP parameter keys rather than the values. Version 8.0.0.3 contains a patch.

- [https://github.com/ChrisSub08/CVE-2026-29187_SqlInjectionVulnerabilityOpenEMR7.0.4](https://github.com/ChrisSub08/CVE-2026-29187_SqlInjectionVulnerabilityOpenEMR7.0.4) :  ![starts](https://img.shields.io/github/stars/ChrisSub08/CVE-2026-29187_SqlInjectionVulnerabilityOpenEMR7.0.4.svg) ![forks](https://img.shields.io/github/forks/ChrisSub08/CVE-2026-29187_SqlInjectionVulnerabilityOpenEMR7.0.4.svg)


## CVE-2026-27940
 llama.cpp is an inference of several LLM models in C/C++. Prior to b8146, the gguf_init_from_file_impl() in gguf.cpp is vulnerable to an Integer overflow, leading to an undersized heap allocation. Using the subsequent fread() writes 528+ bytes of attacker-controlled data past the buffer boundary. This is a bypass of a similar bug in the same file - CVE-2025-53630, but the fix overlooked some areas. This vulnerability is fixed in b8146.

- [https://github.com/ngtuonghung/CVE-2026-27940](https://github.com/ngtuonghung/CVE-2026-27940) :  ![starts](https://img.shields.io/github/stars/ngtuonghung/CVE-2026-27940.svg) ![forks](https://img.shields.io/github/forks/ngtuonghung/CVE-2026-27940.svg)


## CVE-2026-25075
 strongSwan versions 4.5.0 prior to 6.0.5 contain an integer underflow vulnerability in the EAP-TTLS AVP parser that allows unauthenticated remote attackers to cause a denial of service by sending crafted AVP data with invalid length fields during IKEv2 authentication. Attackers can exploit the failure to validate AVP length fields before subtraction to trigger excessive memory allocation or NULL pointer dereference, crashing the charon IKE daemon.

- [https://github.com/BishopFox/CVE-2026-25075-check](https://github.com/BishopFox/CVE-2026-25075-check) :  ![starts](https://img.shields.io/github/stars/BishopFox/CVE-2026-25075-check.svg) ![forks](https://img.shields.io/github/forks/BishopFox/CVE-2026-25075-check.svg)


## CVE-2026-24423
 SmarterTools SmarterMail versions prior to build 9511 contain an unauthenticated remote code execution vulnerability in the ConnectToHub API method. The attacker could point the SmarterMail to the malicious HTTP server, which serves the malicious OS command. This command will be executed by the vulnerable application.

- [https://github.com/aavamin/CVE-2026-24423](https://github.com/aavamin/CVE-2026-24423) :  ![starts](https://img.shields.io/github/stars/aavamin/CVE-2026-24423.svg) ![forks](https://img.shields.io/github/forks/aavamin/CVE-2026-24423.svg)


## CVE-2026-24291
 Incorrect permission assignment for critical resource in Windows Accessibility Infrastructure (ATBroker.exe) allows an authorized attacker to elevate privileges locally.

- [https://github.com/uname1able/CVE-2026-24291](https://github.com/uname1able/CVE-2026-24291) :  ![starts](https://img.shields.io/github/stars/uname1able/CVE-2026-24291.svg) ![forks](https://img.shields.io/github/forks/uname1able/CVE-2026-24291.svg)
- [https://github.com/tracyliving606/RegPwn](https://github.com/tracyliving606/RegPwn) :  ![starts](https://img.shields.io/github/stars/tracyliving606/RegPwn.svg) ![forks](https://img.shields.io/github/forks/tracyliving606/RegPwn.svg)


## CVE-2026-24126
 Weblate is a web based localization tool. Prior to 5.16.0, the SSH management console did not validate the passed input while adding the SSH host key, which could lead to an argument injection to `ssh-add`. Version 5.16.0 fixes the issue. As a workaround, properly limit access to the management console.

- [https://github.com/alexb616/Weblate-CVE-2026-24126](https://github.com/alexb616/Weblate-CVE-2026-24126) :  ![starts](https://img.shields.io/github/stars/alexb616/Weblate-CVE-2026-24126.svg) ![forks](https://img.shields.io/github/forks/alexb616/Weblate-CVE-2026-24126.svg)


## CVE-2026-24061
 telnetd in GNU Inetutils through 2.7 allows remote authentication bypass via a "-f root" value for the USER environment variable.

- [https://github.com/ekomsSavior/telnet_scan](https://github.com/ekomsSavior/telnet_scan) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/telnet_scan.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/telnet_scan.svg)


## CVE-2026-24018
 A UNIX symbolic link (Symlink) following vulnerability in Fortinet FortiClientLinux 7.4.0 through 7.4.4, FortiClientLinux 7.2.2 through 7.2.12 may allow a local and unprivileged user to escalate their privileges to root.

- [https://github.com/febin0x10/Fortinet_FortiClient_Exploit_CVE-2026-24018](https://github.com/febin0x10/Fortinet_FortiClient_Exploit_CVE-2026-24018) :  ![starts](https://img.shields.io/github/stars/febin0x10/Fortinet_FortiClient_Exploit_CVE-2026-24018.svg) ![forks](https://img.shields.io/github/forks/febin0x10/Fortinet_FortiClient_Exploit_CVE-2026-24018.svg)


## CVE-2026-23745
 node-tar is a Tar for Node.js. The node-tar library (= 7.5.2) fails to sanitize the linkpath of Link (hardlink) and SymbolicLink entries when preservePaths is false (the default secure behavior). This allows malicious archives to bypass the extraction root restriction, leading to Arbitrary File Overwrite via hardlinks and Symlink Poisoning via absolute symlink targets. This vulnerability is fixed in 7.5.3.

- [https://github.com/Novem13th/CVE-2026-23745-via-graphql-DEMO](https://github.com/Novem13th/CVE-2026-23745-via-graphql-DEMO) :  ![starts](https://img.shields.io/github/stars/Novem13th/CVE-2026-23745-via-graphql-DEMO.svg) ![forks](https://img.shields.io/github/forks/Novem13th/CVE-2026-23745-via-graphql-DEMO.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/ctzisme/CVE-2026-23744](https://github.com/ctzisme/CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/ctzisme/CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/ctzisme/CVE-2026-23744.svg)


## CVE-2026-3891
 The Pix for WooCommerce plugin for WordPress is vulnerable to arbitrary file uploads due to missing capability check and missing file type validation in the 'lkn_pix_for_woocommerce_c6_save_settings' function in all versions up to, and including, 1.5.0. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/vladimirmanylobed451/CVE-2026-3891](https://github.com/vladimirmanylobed451/CVE-2026-3891) :  ![starts](https://img.shields.io/github/stars/vladimirmanylobed451/CVE-2026-3891.svg) ![forks](https://img.shields.io/github/forks/vladimirmanylobed451/CVE-2026-3891.svg)


## CVE-2026-3407
 A vulnerability was determined in YosysHQ yosys up to 0.62. This affects the function Yosys::RTLIL::Const::set of the file kernel/rtlil.h of the component BLIF File Parser. This manipulation causes heap-based buffer overflow. It is possible to launch the attack on the local host. The exploit has been publicly disclosed and may be utilized. Applying a patch is the recommended action to fix this issue. It appears that the issue is not reproducible all the time.

- [https://github.com/Rickidevs/CVE-2026-34070](https://github.com/Rickidevs/CVE-2026-34070) :  ![starts](https://img.shields.io/github/stars/Rickidevs/CVE-2026-34070.svg) ![forks](https://img.shields.io/github/forks/Rickidevs/CVE-2026-34070.svg)


## CVE-2026-3400
 A security flaw has been discovered in Tenda AC15 up to 15.13.07.13. Affected by this issue is some unknown functionality of the file /goform/TextEditingConversion. The manipulation of the argument wpapsk_crypto2_4g results in stack-based buffer overflow. The attack may be launched remotely. The exploit has been released to the public and may be used for attacks.

- [https://github.com/uky007/CVE-2026-34005](https://github.com/uky007/CVE-2026-34005) :  ![starts](https://img.shields.io/github/stars/uky007/CVE-2026-34005.svg) ![forks](https://img.shields.io/github/forks/uky007/CVE-2026-34005.svg)


## CVE-2026-3003
 The Vagaro Booking Widget plugin for WordPress is vulnerable to Stored Cross-Site Scripting via the ‘vagaro_code’ parameter in all versions up to, and including, 0.3 due to insufficient input sanitization and output escaping. This makes it possible for unauthenticated attackers to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page.

- [https://github.com/bx33661/CVE-2026-30039](https://github.com/bx33661/CVE-2026-30039) :  ![starts](https://img.shields.io/github/stars/bx33661/CVE-2026-30039.svg) ![forks](https://img.shields.io/github/forks/bx33661/CVE-2026-30039.svg)


## CVE-2026-2997
 Tronclass developed by WisdomGarden has a Insecure Direct Object Reference vulnerability. After obtaining a course ID, authenticated remote attackers to modify a specific parameter to obtain a course invitation code, thereby joining any course.

- [https://github.com/Tharooon/CVE-2026-29971](https://github.com/Tharooon/CVE-2026-29971) :  ![starts](https://img.shields.io/github/stars/Tharooon/CVE-2026-29971.svg) ![forks](https://img.shields.io/github/forks/Tharooon/CVE-2026-29971.svg)
- [https://github.com/tharunchidurala-cyber/BACkupCVE-2026-29971](https://github.com/tharunchidurala-cyber/BACkupCVE-2026-29971) :  ![starts](https://img.shields.io/github/stars/tharunchidurala-cyber/BACkupCVE-2026-29971.svg) ![forks](https://img.shields.io/github/forks/tharunchidurala-cyber/BACkupCVE-2026-29971.svg)


## CVE-2026-2576
 The Business Directory Plugin – Easy Listing Directories for WordPress plugin for WordPress is vulnerable to time-based SQL Injection via the 'payment' parameter in all versions up to, and including, 6.4.2 due to insufficient escaping on the user supplied parameter and lack of sufficient preparation on the existing SQL query. This makes it possible for unauthenticated attackers to append additional SQL queries into already existing queries that can be used to extract sensitive information from the database.

- [https://github.com/SowatKheang/CVE_2026_2576_PoC](https://github.com/SowatKheang/CVE_2026_2576_PoC) :  ![starts](https://img.shields.io/github/stars/SowatKheang/CVE_2026_2576_PoC.svg) ![forks](https://img.shields.io/github/forks/SowatKheang/CVE_2026_2576_PoC.svg)


## CVE-2025-64446
 A relative path traversal vulnerability in Fortinet FortiWeb 8.0.0 through 8.0.1, FortiWeb 7.6.0 through 7.6.4, FortiWeb 7.4.0 through 7.4.9, FortiWeb 7.2.0 through 7.2.11, FortiWeb 7.0.0 through 7.0.11 may allow an attacker to execute administrative commands on the system via crafted HTTP or HTTPS requests.

- [https://github.com/0xAshwesker/CVE-2025-64446](https://github.com/0xAshwesker/CVE-2025-64446) :  ![starts](https://img.shields.io/github/stars/0xAshwesker/CVE-2025-64446.svg) ![forks](https://img.shields.io/github/forks/0xAshwesker/CVE-2025-64446.svg)


## CVE-2025-52913
 A vulnerability in the NuPoint Unified Messaging (NPM) component of Mitel MiCollab through 9.8 SP2 (9.8.2.12) could allow an unauthenticated attacker to conduct a path traversal attack due to insufficient input validation. A successful exploit could allow unauthorized access, enabling the attacker to view, corrupt, or delete users' data and system configurations.

- [https://github.com/pgaSUS99/PoC-CVE-2025-52913](https://github.com/pgaSUS99/PoC-CVE-2025-52913) :  ![starts](https://img.shields.io/github/stars/pgaSUS99/PoC-CVE-2025-52913.svg) ![forks](https://img.shields.io/github/forks/pgaSUS99/PoC-CVE-2025-52913.svg)


## CVE-2025-49844
 Redis is an open source, in-memory database that persists on disk. Versions 8.2.1 and below allow an authenticated user to use a specially crafted Lua script to manipulate the garbage collector, trigger a use-after-free and potentially lead to remote code execution. The problem exists in all versions of Redis with Lua scripting. This issue is fixed in version 8.2.2. To workaround this issue without patching the redis-server executable is to prevent users from executing Lua scripts. This can be done using ACL to restrict EVAL and EVALSHA commands.

- [https://github.com/zbyszkok/CVE-2025-49844-RediShell-AI-made-Revshell](https://github.com/zbyszkok/CVE-2025-49844-RediShell-AI-made-Revshell) :  ![starts](https://img.shields.io/github/stars/zbyszkok/CVE-2025-49844-RediShell-AI-made-Revshell.svg) ![forks](https://img.shields.io/github/forks/zbyszkok/CVE-2025-49844-RediShell-AI-made-Revshell.svg)


## CVE-2025-49132
 Pterodactyl is a free, open-source game server management panel. Prior to version 1.11.11, using the /locales/locale.json with the locale and namespace query parameters, a malicious actor is able to execute arbitrary code without being authenticated. With the ability to execute arbitrary code it could be used to gain access to the Panel's server, read credentials from the Panel's config, extract sensitive information from the database, access files of servers managed by the panel, etc. This issue has been patched in version 1.11.11. There are no software workarounds for this vulnerability, but use of an external Web Application Firewall (WAF) could help mitigate this attack.

- [https://github.com/Ahmedf000/CVE-2025-49132_HTB_SEASON10](https://github.com/Ahmedf000/CVE-2025-49132_HTB_SEASON10) :  ![starts](https://img.shields.io/github/stars/Ahmedf000/CVE-2025-49132_HTB_SEASON10.svg) ![forks](https://img.shields.io/github/forks/Ahmedf000/CVE-2025-49132_HTB_SEASON10.svg)


## CVE-2025-39459
 Incorrect Privilege Assignment vulnerability in Contempo Themes Real Estate 7 allows Privilege Escalation.This issue affects Real Estate 7: from n/a through 3.5.2.

- [https://github.com/qalesyaSN/CVE-2025-39459](https://github.com/qalesyaSN/CVE-2025-39459) :  ![starts](https://img.shields.io/github/stars/qalesyaSN/CVE-2025-39459.svg) ![forks](https://img.shields.io/github/forks/qalesyaSN/CVE-2025-39459.svg)


## CVE-2025-34282
 ThingsBoard versions  4.2.1 contain a server-side request forgery (SSRF) vulnerability in the dashboard's Image Upload Gallery feature. An attacker can upload a malicious SVG file that references a remote URL. If the server processes the SVG file in a way that parses external references, it may initiate unintended outbound requests. This can be used to access internal services or resources.

- [https://github.com/mathitam/thingsboard-ssrf-cve-2025-34282](https://github.com/mathitam/thingsboard-ssrf-cve-2025-34282) :  ![starts](https://img.shields.io/github/stars/mathitam/thingsboard-ssrf-cve-2025-34282.svg) ![forks](https://img.shields.io/github/forks/mathitam/thingsboard-ssrf-cve-2025-34282.svg)


## CVE-2025-34037
 An OS command injection vulnerability exists in various models of E-Series Linksys routers via the /tmUnblock.cgi and /hndUnblock.cgi endpoints over HTTP on port 8080. The CGI scripts improperly process user-supplied input passed to the ttcp_ip parameter without sanitization, allowing unauthenticated attackers to inject shell commands. This vulnerability was reported to be exploited in the wild by the "TheMoon" worm  in 2014 to deploy a MIPS ELF payload, enabling arbitrary code execution on the router. Additionally, this vulnerability may affect other Linksys products to include, but not limited to, WAG/WAP/WES/WET/WRT-series router models and Wireless-N access points and routers. Exploitation evidence was observed by the Shadowserver Foundation on 2025-02-06 UTC.

- [https://github.com/Taxanehh/CVE-2025-34037](https://github.com/Taxanehh/CVE-2025-34037) :  ![starts](https://img.shields.io/github/stars/Taxanehh/CVE-2025-34037.svg) ![forks](https://img.shields.io/github/forks/Taxanehh/CVE-2025-34037.svg)


## CVE-2025-31115
 XZ Utils provide a general-purpose data-compression library plus command-line tools. In XZ Utils 5.3.3alpha to 5.8.0, the multithreaded .xz decoder in liblzma has a bug where invalid input can at least result in a crash. The effects include heap use after free and writing to an address based on the null pointer plus an offset. Applications and libraries that use the lzma_stream_decoder_mt function are affected. The bug has been fixed in XZ Utils 5.8.1, and the fix has been committed to the v5.4, v5.6, v5.8, and master branches in the xz Git repository. No new release packages will be made from the old stable branches, but a standalone patch is available that applies to all affected releases.

- [https://github.com/greydoubt/xz](https://github.com/greydoubt/xz) :  ![starts](https://img.shields.io/github/stars/greydoubt/xz.svg) ![forks](https://img.shields.io/github/forks/greydoubt/xz.svg)


## CVE-2025-24813
Users are recommended to upgrade to version 11.0.3, 10.1.35 or 9.0.99, which fixes the issue.

- [https://github.com/EQSTLab/CVE-2025-24813](https://github.com/EQSTLab/CVE-2025-24813) :  ![starts](https://img.shields.io/github/stars/EQSTLab/CVE-2025-24813.svg) ![forks](https://img.shields.io/github/forks/EQSTLab/CVE-2025-24813.svg)


## CVE-2025-4615
Cloud NGFW and Prisma® Access are not affected by this vulnerability.

- [https://github.com/sh00bx/cve-2025-4615](https://github.com/sh00bx/cve-2025-4615) :  ![starts](https://img.shields.io/github/stars/sh00bx/cve-2025-4615.svg) ![forks](https://img.shields.io/github/forks/sh00bx/cve-2025-4615.svg)


## CVE-2024-47611
 XZ Utils provide a general-purpose data-compression library plus command-line tools. When built for native Windows (MinGW-w64 or MSVC), the command line tools from XZ Utils 5.6.2 and older have a command line argument injection vulnerability. If a command line contains Unicode characters (for example, filenames) that don't exist in the current legacy code page, the characters are converted to similar-looking characters with best-fit mapping. Some best-fit mappings result in ASCII characters that change the meaning of the command line, which can be exploited with malicious filenames to do argument injection or directory traversal attacks. This vulnerability is fixed in 5.6.3. Command line tools built for Cygwin or MSYS2 are unaffected. liblzma is unaffected.

- [https://github.com/greydoubt/xz](https://github.com/greydoubt/xz) :  ![starts](https://img.shields.io/github/stars/greydoubt/xz.svg) ![forks](https://img.shields.io/github/forks/greydoubt/xz.svg)


## CVE-2024-36039
 PyMySQL through 1.1.0 allows SQL injection if used with untrusted JSON input because keys are not escaped by escape_dict.

- [https://github.com/zenniskayy2k4/CVE-2024-36039_PoC](https://github.com/zenniskayy2k4/CVE-2024-36039_PoC) :  ![starts](https://img.shields.io/github/stars/zenniskayy2k4/CVE-2024-36039_PoC.svg) ![forks](https://img.shields.io/github/forks/zenniskayy2k4/CVE-2024-36039_PoC.svg)


## CVE-2022-2274
 The OpenSSL 3.0.4 release introduced a serious bug in the RSA implementation for X86_64 CPUs supporting the AVX512IFMA instructions. This issue makes the RSA implementation with 2048 bit private keys incorrect on such machines and memory corruption will happen during the computation. As a consequence of the memory corruption an attacker may be able to trigger a remote code execution on the machine performing the computation. SSL/TLS servers or other servers using 2048 bit RSA private keys running on machines supporting AVX512IFMA instructions of the X86_64 architecture are affected by this issue.

- [https://github.com/Malwareman007/CVE-2022-2274](https://github.com/Malwareman007/CVE-2022-2274) :  ![starts](https://img.shields.io/github/stars/Malwareman007/CVE-2022-2274.svg) ![forks](https://img.shields.io/github/forks/Malwareman007/CVE-2022-2274.svg)
- [https://github.com/DesmondSanctity/CVE-2022-2274](https://github.com/DesmondSanctity/CVE-2022-2274) :  ![starts](https://img.shields.io/github/stars/DesmondSanctity/CVE-2022-2274.svg) ![forks](https://img.shields.io/github/forks/DesmondSanctity/CVE-2022-2274.svg)
- [https://github.com/EkamSinghWalia/OpenSSL-Vulnerability-Detection-Script](https://github.com/EkamSinghWalia/OpenSSL-Vulnerability-Detection-Script) :  ![starts](https://img.shields.io/github/stars/EkamSinghWalia/OpenSSL-Vulnerability-Detection-Script.svg) ![forks](https://img.shields.io/github/forks/EkamSinghWalia/OpenSSL-Vulnerability-Detection-Script.svg)


## CVE-2022-2185
 A critical issue has been discovered in GitLab affecting all versions starting from 14.0 prior to 14.10.5, 15.0 prior to 15.0.4, and 15.1 prior to 15.1.1 where an authenticated user authorized to import projects could import a maliciously crafted project leading to remote code execution.

- [https://github.com/ESUAdmin/CVE-2022-2185](https://github.com/ESUAdmin/CVE-2022-2185) :  ![starts](https://img.shields.io/github/stars/ESUAdmin/CVE-2022-2185.svg) ![forks](https://img.shields.io/github/forks/ESUAdmin/CVE-2022-2185.svg)
- [https://github.com/safe3s/CVE-2022-2185-poc](https://github.com/safe3s/CVE-2022-2185-poc) :  ![starts](https://img.shields.io/github/stars/safe3s/CVE-2022-2185-poc.svg) ![forks](https://img.shields.io/github/forks/safe3s/CVE-2022-2185-poc.svg)


## CVE-2020-0601
 A spoofing vulnerability exists in the way Windows CryptoAPI (Crypt32.dll) validates Elliptic Curve Cryptography (ECC) certificates.An attacker could exploit the vulnerability by using a spoofed code-signing certificate to sign a malicious executable, making it appear the file was from a trusted, legitimate source, aka 'Windows CryptoAPI Spoofing Vulnerability'.

- [https://github.com/CrackerCat/CurveballCertTool](https://github.com/CrackerCat/CurveballCertTool) :  ![starts](https://img.shields.io/github/stars/CrackerCat/CurveballCertTool.svg) ![forks](https://img.shields.io/github/forks/CrackerCat/CurveballCertTool.svg)


## CVE-2018-13379
 An Improper Limitation of a Pathname to a Restricted Directory ("Path Traversal") in Fortinet FortiOS 6.0.0 to 6.0.4, 5.6.3 to 5.6.7 and 5.4.6 to 5.4.12 and FortiProxy 2.0.0, 1.2.0 to 1.2.8, 1.1.0 to 1.1.6, 1.0.0 to 1.0.7 under SSL VPN web portal allows an unauthenticated attacker to download system files via special crafted HTTP resource requests.

- [https://github.com/Justjeff211/conti-ransomware-writeup](https://github.com/Justjeff211/conti-ransomware-writeup) :  ![starts](https://img.shields.io/github/stars/Justjeff211/conti-ransomware-writeup.svg) ![forks](https://img.shields.io/github/forks/Justjeff211/conti-ransomware-writeup.svg)


## CVE-2018-13374
 A Improper Access Control in Fortinet FortiOS 6.0.2, 5.6.7 and before, FortiADC 6.1.0, 6.0.0 to 6.0.1, 5.4.0 to 5.4.4 allows attacker to obtain the LDAP server login credentials configured in FortiGate via pointing a LDAP server connectivity test request to a rogue LDAP server instead of the configured one.

- [https://github.com/Justjeff211/conti-ransomware-writeup](https://github.com/Justjeff211/conti-ransomware-writeup) :  ![starts](https://img.shields.io/github/stars/Justjeff211/conti-ransomware-writeup.svg) ![forks](https://img.shields.io/github/forks/Justjeff211/conti-ransomware-writeup.svg)


## CVE-2018-7600
 Drupal before 7.58, 8.x before 8.3.9, 8.4.x before 8.4.6, and 8.5.x before 8.5.1 allows remote attackers to execute arbitrary code because of an issue affecting multiple subsystems with default or common module configurations.

- [https://github.com/erman-bolukbasi/web-penetration-drupal](https://github.com/erman-bolukbasi/web-penetration-drupal) :  ![starts](https://img.shields.io/github/stars/erman-bolukbasi/web-penetration-drupal.svg) ![forks](https://img.shields.io/github/forks/erman-bolukbasi/web-penetration-drupal.svg)


## CVE-2014-6271
 GNU Bash through 4.3 processes trailing strings after function definitions in the values of environment variables, which allows remote attackers to execute arbitrary code via a crafted environment, as demonstrated by vectors involving the ForceCommand feature in OpenSSH sshd, the mod_cgi and mod_cgid modules in the Apache HTTP Server, scripts executed by unspecified DHCP clients, and other situations in which setting the environment occurs across a privilege boundary from Bash execution, aka "ShellShock."  NOTE: the original fix for this issue was incorrect; CVE-2014-7169 has been assigned to cover the vulnerability that is still present after the incorrect fix.

- [https://github.com/0xBlackash/CVE-2014-6271](https://github.com/0xBlackash/CVE-2014-6271) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2014-6271.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2014-6271.svg)


## CVE-2014-0160
 The (1) TLS and (2) DTLS implementations in OpenSSL 1.0.1 before 1.0.1g do not properly handle Heartbeat Extension packets, which allows remote attackers to obtain sensitive information from process memory via crafted packets that trigger a buffer over-read, as demonstrated by reading private keys, related to d1_both.c and t1_lib.c, aka the Heartbleed bug.

- [https://github.com/0xBlackash/CVE-2014-0160](https://github.com/0xBlackash/CVE-2014-0160) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2014-0160.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2014-0160.svg)


## CVE-2008-1657
 OpenSSH 4.4 up to versions before 4.9 allows remote authenticated users to bypass the sshd_config ForceCommand directive by modifying the .ssh/rc session file.

- [https://github.com/Faizan8232403/CVE-Exploit-Research-Development](https://github.com/Faizan8232403/CVE-Exploit-Research-Development) :  ![starts](https://img.shields.io/github/stars/Faizan8232403/CVE-Exploit-Research-Development.svg) ![forks](https://img.shields.io/github/forks/Faizan8232403/CVE-Exploit-Research-Development.svg)
- [https://github.com/QasimShahbaz21/CVE-Exploit-Research-Development](https://github.com/QasimShahbaz21/CVE-Exploit-Research-Development) :  ![starts](https://img.shields.io/github/stars/QasimShahbaz21/CVE-Exploit-Research-Development.svg) ![forks](https://img.shields.io/github/forks/QasimShahbaz21/CVE-Exploit-Research-Development.svg)


## CVE-2008-0166
 OpenSSL 0.9.8c-1 up to versions before 0.9.8g-9 on Debian-based operating systems uses a random number generator that generates predictable numbers, which makes it easier for remote attackers to conduct brute force guessing attacks against cryptographic keys.

- [https://github.com/Faizan8232403/CVE-Exploit-Research-Development](https://github.com/Faizan8232403/CVE-Exploit-Research-Development) :  ![starts](https://img.shields.io/github/stars/Faizan8232403/CVE-Exploit-Research-Development.svg) ![forks](https://img.shields.io/github/forks/Faizan8232403/CVE-Exploit-Research-Development.svg)
- [https://github.com/QasimShahbaz21/CVE-Exploit-Research-Development](https://github.com/QasimShahbaz21/CVE-Exploit-Research-Development) :  ![starts](https://img.shields.io/github/stars/QasimShahbaz21/CVE-Exploit-Research-Development.svg) ![forks](https://img.shields.io/github/forks/QasimShahbaz21/CVE-Exploit-Research-Development.svg)

