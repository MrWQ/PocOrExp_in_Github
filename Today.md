# Update 2026-03-27
## CVE-2026-33179
 libfuse is the reference implementation of the Linux FUSE. From version 3.18.0 to before version 3.18.2, a NULL pointer dereference and memory leak in fuse_uring_init_queue allows a local user to crash the FUSE daemon or cause resource exhaustion. When numa_alloc_local fails during io_uring queue entry setup, the code proceeds with NULL pointers. When fuse_uring_register_queue fails, NUMA allocations are leaked and the function incorrectly returns success. Only the io_uring transport is affected; the traditional /dev/fuse path is not affected. PoC confirmed with AddressSanitizer/LeakSanitizer. This issue has been patched in version 3.18.2.

- [https://github.com/abhinavagarwal07/abhinavagarwal07.github.io](https://github.com/abhinavagarwal07/abhinavagarwal07.github.io) :  ![starts](https://img.shields.io/github/stars/abhinavagarwal07/abhinavagarwal07.github.io.svg) ![forks](https://img.shields.io/github/forks/abhinavagarwal07/abhinavagarwal07.github.io.svg)


## CVE-2026-33150
 libfuse is the reference implementation of the Linux FUSE. From version 3.18.0 to before version 3.18.2, a use-after-free vulnerability in the io_uring subsystem of libfuse allows a local attacker to crash FUSE filesystem processes and potentially execute arbitrary code. When io_uring thread creation fails due to resource exhaustion (e.g., cgroup pids.max), fuse_uring_start() frees the ring pool structure but stores the dangling pointer in the session state, leading to a use-after-free when the session shuts down. The trigger is reliable in containerized environments where cgroup pids.max limits naturally constrain thread creation. This issue has been patched in version 3.18.2.

- [https://github.com/abhinavagarwal07/abhinavagarwal07.github.io](https://github.com/abhinavagarwal07/abhinavagarwal07.github.io) :  ![starts](https://img.shields.io/github/stars/abhinavagarwal07/abhinavagarwal07.github.io.svg) ![forks](https://img.shields.io/github/forks/abhinavagarwal07/abhinavagarwal07.github.io.svg)


## CVE-2026-26833
 thumbler through 1.1.2 allows OS command injection via the input, output, time, or size parameter in the thumbnail() function because user input is concatenated into a shell command string passed to child_process.exec() without proper sanitization or escaping.

- [https://github.com/zebbernCVE/npm-cve-2026-26830-26833](https://github.com/zebbernCVE/npm-cve-2026-26830-26833) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/npm-cve-2026-26830-26833.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/npm-cve-2026-26830-26833.svg)
- [https://github.com/zebbernCVE/CVE-2026-26833](https://github.com/zebbernCVE/CVE-2026-26833) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26833.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26833.svg)


## CVE-2026-26832
 node-tesseract-ocr is an npm package that provides a Node.js wrapper for Tesseract OCR. In all versions through 2.2.1, the recognize() function in src/index.js is vulnerable to OS Command Injection. The file path parameter is concatenated into a shell command string and passed to child_process.exec() without proper sanitization

- [https://github.com/zebbernCVE/CVE-2026-26832](https://github.com/zebbernCVE/CVE-2026-26832) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26832.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26832.svg)


## CVE-2026-26831
 textract through 2.5.0 is vulnerable to OS Command Injection via the file path parameter in multiple extractors. When processing files with malicious filenames, the filePath is passed directly to child_process.exec() in lib/extractors/doc.js, rtf.js, dxf.js, images.js, and lib/util.js with inadequate sanitization

- [https://github.com/zebbernCVE/CVE-2026-26831](https://github.com/zebbernCVE/CVE-2026-26831) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26831.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26831.svg)


## CVE-2026-26830
 pdf-image (npm package) through version 2.0.0 allows OS command injection via the pdfFilePath parameter. The constructGetInfoCommand and constructConvertCommandForPage functions use util.format() to interpolate user-controlled file paths into shell command strings that are executed via child_process.exec()

- [https://github.com/zebbernCVE/npm-cve-2026-26830-26833](https://github.com/zebbernCVE/npm-cve-2026-26830-26833) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/npm-cve-2026-26830-26833.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/npm-cve-2026-26830-26833.svg)
- [https://github.com/zebbernCVE/CVE-2026-26830](https://github.com/zebbernCVE/CVE-2026-26830) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26830.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26830.svg)


## CVE-2026-26198
 Ormar is a async mini ORM for Python. In versions 0.9.9 through 0.22.0, when performing aggregate queries, Ormar ORM constructs SQL expressions by passing user-supplied column names directly into `sqlalchemy.text()` without any validation or sanitization. The `min()` and `max()` methods in the `QuerySet` class accept arbitrary string input as the column parameter. While `sum()` and `avg()` are partially protected by an `is_numeric` type check that rejects non-existent fields, `min()` and `max()` skip this validation entirely. As a result, an attacker-controlled string is embedded as raw SQL inside the aggregate function call. Any unauthorized user can exploit this vulnerability to read the entire database contents, including tables unrelated to the queried model, by injecting a subquery as the column parameter. Version 0.23.0 contains a patch.

- [https://github.com/sergicortesabadia/CVE-2026-26198-analysis](https://github.com/sergicortesabadia/CVE-2026-26198-analysis) :  ![starts](https://img.shields.io/github/stars/sergicortesabadia/CVE-2026-26198-analysis.svg) ![forks](https://img.shields.io/github/forks/sergicortesabadia/CVE-2026-26198-analysis.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/z4yd3/PoC-CVE-2026-23744](https://github.com/z4yd3/PoC-CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/z4yd3/PoC-CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/z4yd3/PoC-CVE-2026-23744.svg)
- [https://github.com/yassertioursi/htb-kobold-writeup](https://github.com/yassertioursi/htb-kobold-writeup) :  ![starts](https://img.shields.io/github/stars/yassertioursi/htb-kobold-writeup.svg) ![forks](https://img.shields.io/github/forks/yassertioursi/htb-kobold-writeup.svg)


## CVE-2026-23520
 Arcane provides modern docker management. Prior to 1.13.0, Arcane has a command injection in the updater service. Arcane’s updater service supported lifecycle labels com.getarcaneapp.arcane.lifecycle.pre-update and com.getarcaneapp.arcane.lifecycle.post-update that allowed defining a command to run before or after a container update. The label value is passed directly to /bin/sh -c without sanitization or validation. Because any authenticated user (not limited to administrators) can create projects through the API, an attacker can create a project that specifies one of these lifecycle labels with a malicious command. When an administrator later triggers a container update (either manually or via scheduled update checks), Arcane reads the lifecycle label and executes its value as a shell command inside the container. This vulnerability is fixed in 1.13.0.

- [https://github.com/0xzap/CVE-2026-23520](https://github.com/0xzap/CVE-2026-23520) :  ![starts](https://img.shields.io/github/stars/0xzap/CVE-2026-23520.svg) ![forks](https://img.shields.io/github/forks/0xzap/CVE-2026-23520.svg)


## CVE-2026-20687
 A use after free issue was addressed with improved memory management. This issue is fixed in iOS 18.7.7 and iPadOS 18.7.7, iOS 26.4 and iPadOS 26.4, macOS Sequoia 15.7.5, macOS Tahoe 26.4, tvOS 26.4, watchOS 26.4. An app may be able to cause unexpected system termination or write kernel memory.

- [https://github.com/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF](https://github.com/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF) :  ![starts](https://img.shields.io/github/stars/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF.svg) ![forks](https://img.shields.io/github/forks/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF.svg)


## CVE-2026-3584
 The Kali Forms plugin for WordPress is vulnerable to Remote Code Execution in all versions up to, and including, 2.4.9 via the 'form_process' function. This is due to the 'prepare_post_data' function mapping user-supplied keys directly into internal placeholder storage, combined with the use of 'call_user_func' on these placeholder values. This makes it possible for unauthenticated attackers to execute code on the server.

- [https://github.com/Yucaerin/CVE-2026-3584](https://github.com/Yucaerin/CVE-2026-3584) :  ![starts](https://img.shields.io/github/stars/Yucaerin/CVE-2026-3584.svg) ![forks](https://img.shields.io/github/forks/Yucaerin/CVE-2026-3584.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg)


## CVE-2025-52204
 A Cross-Site Scripting (XSS) vulnerability exists in Znuny::ITSM 6.5.x in the customer.pl endpoint via the OTRSCustomerInterface parameter

- [https://github.com/j0qq3r/CVE-2025-52204](https://github.com/j0qq3r/CVE-2025-52204) :  ![starts](https://img.shields.io/github/stars/j0qq3r/CVE-2025-52204.svg) ![forks](https://img.shields.io/github/forks/j0qq3r/CVE-2025-52204.svg)


## CVE-2025-32463
 Sudo before 1.9.17p1 allows local users to obtain root access because /etc/nsswitch.conf from a user-controlled directory is used with the --chroot option.

- [https://github.com/0xzap/CVE-2025-32463](https://github.com/0xzap/CVE-2025-32463) :  ![starts](https://img.shields.io/github/stars/0xzap/CVE-2025-32463.svg) ![forks](https://img.shields.io/github/forks/0xzap/CVE-2025-32463.svg)


## CVE-2025-8088
     from ESET.

- [https://github.com/lennertdefauw/CVE-2025-8088](https://github.com/lennertdefauw/CVE-2025-8088) :  ![starts](https://img.shields.io/github/stars/lennertdefauw/CVE-2025-8088.svg) ![forks](https://img.shields.io/github/forks/lennertdefauw/CVE-2025-8088.svg)


## CVE-2024-52302
 common-user-management is a robust Spring Boot application featuring user management services designed to control user access dynamically. There is a critical security vulnerability in the application endpoint /api/v1/customer/profile-picture. This endpoint allows file uploads without proper validation or restrictions, enabling attackers to upload malicious files that can lead to Remote Code Execution (RCE).

- [https://github.com/pream-totaram/CVE-2024-52302-reproduction](https://github.com/pream-totaram/CVE-2024-52302-reproduction) :  ![starts](https://img.shields.io/github/stars/pream-totaram/CVE-2024-52302-reproduction.svg) ![forks](https://img.shields.io/github/forks/pream-totaram/CVE-2024-52302-reproduction.svg)


## CVE-2024-21413
 Microsoft Outlook Remote Code Execution Vulnerability

- [https://github.com/TheMursalin/HTB-Mailing-A-Complete-Walkthrough](https://github.com/TheMursalin/HTB-Mailing-A-Complete-Walkthrough) :  ![starts](https://img.shields.io/github/stars/TheMursalin/HTB-Mailing-A-Complete-Walkthrough.svg) ![forks](https://img.shields.io/github/forks/TheMursalin/HTB-Mailing-A-Complete-Walkthrough.svg)


## CVE-2024-4577
 In PHP versions 8.1.* before 8.1.29, 8.2.* before 8.2.20, 8.3.* before 8.3.8, when using Apache and PHP-CGI on Windows, if the system is set up to use certain code pages, Windows may use "Best-Fit" behavior to replace characters in command line given to Win32 API functions. PHP CGI module may misinterpret those characters as PHP options, which may allow a malicious user to pass options to PHP binary being run, and thus reveal the source code of scripts, run arbitrary PHP code on the server, etc.

- [https://github.com/aavamin/cve-2024-4577](https://github.com/aavamin/cve-2024-4577) :  ![starts](https://img.shields.io/github/stars/aavamin/cve-2024-4577.svg) ![forks](https://img.shields.io/github/forks/aavamin/cve-2024-4577.svg)


## CVE-2024-3094
Through a series of complex obfuscations, the liblzma build process extracts a prebuilt object file from a disguised test file existing in the source code, which is then used to modify specific functions in the liblzma code. This results in a modified liblzma library that can be used by any software linked against this library, intercepting and modifying the data interaction with this library.

- [https://github.com/greydoubt/xz](https://github.com/greydoubt/xz) :  ![starts](https://img.shields.io/github/stars/greydoubt/xz.svg) ![forks](https://img.shields.io/github/forks/greydoubt/xz.svg)


## CVE-2023-20198
 Cisco is providing an update for the ongoing investigation into observed exploitation of the web UI feature in Cisco IOS XE Software. We are updating the list of fixed releases and adding the Software Checker. Our investigation has determined that the actors exploited two previously unknown issues. The attacker first exploited CVE-2023-20198 to gain initial access and issued a privilege 15 command to create a local user and password combination. This allowed the user to log in with normal user access. The attacker then exploited another component of the web UI feature, leveraging the new local user to elevate privilege to root and write the implant to the file system. Cisco has assigned CVE-2023-20273 to this issue. CVE-2023-20198 has been assigned a CVSS Score of 10.0. CVE-2023-20273 has been assigned a CVSS Score of 7.2. Both of these CVEs are being tracked by CSCwh87343.

- [https://github.com/Gill-Singh-A/CVE-2023-20198-Exploit](https://github.com/Gill-Singh-A/CVE-2023-20198-Exploit) :  ![starts](https://img.shields.io/github/stars/Gill-Singh-A/CVE-2023-20198-Exploit.svg) ![forks](https://img.shields.io/github/forks/Gill-Singh-A/CVE-2023-20198-Exploit.svg)


## CVE-2022-36883
 A missing permission check in Jenkins Git Plugin 4.11.3 and earlier allows unauthenticated attackers to trigger builds of jobs configured to use an attacker-specified Git repository and to cause them to check out an attacker-specified commit.

- [https://github.com/superjimmygou/CVE-2022-36883](https://github.com/superjimmygou/CVE-2022-36883) :  ![starts](https://img.shields.io/github/stars/superjimmygou/CVE-2022-36883.svg) ![forks](https://img.shields.io/github/forks/superjimmygou/CVE-2022-36883.svg)
- [https://github.com/qoo7972365/CVE-2022-36883-Poc](https://github.com/qoo7972365/CVE-2022-36883-Poc) :  ![starts](https://img.shields.io/github/stars/qoo7972365/CVE-2022-36883-Poc.svg) ![forks](https://img.shields.io/github/forks/qoo7972365/CVE-2022-36883-Poc.svg)


## CVE-2022-32250
 net/netfilter/nf_tables_api.c in the Linux kernel through 5.18.1 allows a local user (able to create user/net namespaces) to escalate privileges to root because an incorrect NFT_STATEFUL_EXPR check leads to a use-after-free.

- [https://github.com/Noidolosity/CVE-2022-32250](https://github.com/Noidolosity/CVE-2022-32250) :  ![starts](https://img.shields.io/github/stars/Noidolosity/CVE-2022-32250.svg) ![forks](https://img.shields.io/github/forks/Noidolosity/CVE-2022-32250.svg)


## CVE-2022-29455
 DOM-based Reflected Cross-Site Scripting (XSS) vulnerability in Elementor's Elementor Website Builder plugin = 3.5.5 versions.

- [https://github.com/abdipranata/CVE-2022-29455](https://github.com/abdipranata/CVE-2022-29455) :  ![starts](https://img.shields.io/github/stars/abdipranata/CVE-2022-29455.svg) ![forks](https://img.shields.io/github/forks/abdipranata/CVE-2022-29455.svg)


## CVE-2022-1271
 An arbitrary file write vulnerability was found in GNU gzip's zgrep utility. When zgrep is applied on the attacker's chosen file name (for example, a crafted file name), this can overwrite an attacker's content to an arbitrary attacker-selected file. This flaw occurs due to insufficient validation when processing filenames with two or more newlines where selected content and the target file names are embedded in crafted multi-line file names. This flaw allows a remote, low privileged attacker to force zgrep to write arbitrary files on the system.

- [https://github.com/greydoubt/xz](https://github.com/greydoubt/xz) :  ![starts](https://img.shields.io/github/stars/greydoubt/xz.svg) ![forks](https://img.shields.io/github/forks/greydoubt/xz.svg)


## CVE-2021-39156
 Istio is an open source platform for providing a uniform way to integrate microservices, manage traffic flow across microservices, enforce policies and aggregate telemetry data. Istio 1.11.0, 1.10.3 and below, and 1.9.7 and below contain a remotely exploitable vulnerability where an HTTP request with `#fragment` in the path may bypass Istio’s URI path based authorization policies. Patches are available in Istio 1.11.1, Istio 1.10.4 and Istio 1.9.8. As a work around a Lua filter may be written to normalize the path.

- [https://github.com/anonymousAIware2026/MicroserviceCVE-2021-39156](https://github.com/anonymousAIware2026/MicroserviceCVE-2021-39156) :  ![starts](https://img.shields.io/github/stars/anonymousAIware2026/MicroserviceCVE-2021-39156.svg) ![forks](https://img.shields.io/github/forks/anonymousAIware2026/MicroserviceCVE-2021-39156.svg)


## CVE-2020-22916
 An issue discovered in XZ 5.2.5 allows attackers to cause a denial of service via decompression of a crafted file. NOTE: the vendor disputes the claims of "endless output" and "denial of service" because decompression of the 17,486 bytes always results in 114,881,179 bytes, which is often a reasonable size increase.

- [https://github.com/greydoubt/xz](https://github.com/greydoubt/xz) :  ![starts](https://img.shields.io/github/stars/greydoubt/xz.svg) ![forks](https://img.shields.io/github/forks/greydoubt/xz.svg)


## CVE-2020-10567
 An issue was discovered in Responsive Filemanager through 9.14.0. In the ajax_calls.php file in the save_img action in the name parameter, there is no validation of what kind of extension is sent. This makes it possible to execute PHP code if a legitimate JPEG image contains this code in the EXIF data, and the .php extension is used in the name parameter. (A potential fast patch is to disable the save_img action in the config file.)

- [https://github.com/PierreAdams/POC-CVE-2020-10567](https://github.com/PierreAdams/POC-CVE-2020-10567) :  ![starts](https://img.shields.io/github/stars/PierreAdams/POC-CVE-2020-10567.svg) ![forks](https://img.shields.io/github/forks/PierreAdams/POC-CVE-2020-10567.svg)


## CVE-2019-25065
 A vulnerability was found in OpenNetAdmin 18.1.1. It has been rated as critical. Affected by this issue is some unknown functionality. The manipulation leads to privilege escalation. The attack may be launched remotely. The exploit has been disclosed to the public and may be used.

- [https://github.com/HexRazor/CVE-2019-25065-poc](https://github.com/HexRazor/CVE-2019-25065-poc) :  ![starts](https://img.shields.io/github/stars/HexRazor/CVE-2019-25065-poc.svg) ![forks](https://img.shields.io/github/forks/HexRazor/CVE-2019-25065-poc.svg)


## CVE-2017-12542
 A authentication bypass and execution of code vulnerability in HPE Integrated Lights-out 4 (iLO 4) version prior to 2.53 was found.

- [https://github.com/Gill-Singh-A/CVE-2017-12542-Exploit](https://github.com/Gill-Singh-A/CVE-2017-12542-Exploit) :  ![starts](https://img.shields.io/github/stars/Gill-Singh-A/CVE-2017-12542-Exploit.svg) ![forks](https://img.shields.io/github/forks/Gill-Singh-A/CVE-2017-12542-Exploit.svg)

