# Update 2026-03-29
## CVE-2026-33868
 Mastodon is a free, open-source social network server based on ActivityPub. Prior to versions 4.5.8, 4.4.15, and 4.3.21, an unauthenticated Open Redirect vulnerability (CWE-601) exists in the `/web/*` route due to improper handling of URL-encoded path segments. An attacker can craft a specially encoded URL that causes the application to redirect users to an arbitrary external domain, enabling phishing attacks and potential OAuth credential theft. The issue occurs because URL-encoded slashes (`%2F`) bypass Rails path normalization and are interpreted as host-relative redirects. Versions 4.5.8, 4.4.15, and 4.3.21 patch the issue.

- [https://github.com/O99099O/By-Poloss..-..CVE-2026-33868](https://github.com/O99099O/By-Poloss..-..CVE-2026-33868) :  ![starts](https://img.shields.io/github/stars/O99099O/By-Poloss..-..CVE-2026-33868.svg) ![forks](https://img.shields.io/github/forks/O99099O/By-Poloss..-..CVE-2026-33868.svg)


## CVE-2026-33693
 Lemmy is a link aggregator and forum for the fediverse. Prior to version 0.7.0-beta.9, the `v4_is_invalid()` function in `activitypub-federation-rust` (`src/utils.rs`) does not check for `Ipv4Addr::UNSPECIFIED` (0.0.0.0). An unauthenticated attacker controlling a remote domain can point it to 0.0.0.0, bypass the SSRF protection introduced by the fix for CVE-2025-25194 (GHSA-7723-35v7-qcxw), and reach localhost services on the target server. Version 0.7.0-beta.9 patches the issue.

- [https://github.com/SnailSploit/CVE-2026-33693](https://github.com/SnailSploit/CVE-2026-33693) :  ![starts](https://img.shields.io/github/stars/SnailSploit/CVE-2026-33693.svg) ![forks](https://img.shields.io/github/forks/SnailSploit/CVE-2026-33693.svg)


## CVE-2026-33532
 `yaml` is a YAML parser and serialiser for JavaScript. Parsing a YAML document with a version of `yaml` on the 1.x branch prior to 1.10.3 or on the 2.x branch prior to 2.8.3 may throw a RangeError due to a stack overflow. The node resolution/composition phase uses recursive function calls without a depth bound. An attacker who can supply YAML for parsing can trigger a `RangeError: Maximum call stack size exceeded` with a small payload (~2–10 KB). The `RangeError` is not a `YAMLParseError`, so applications that only catch YAML-specific errors will encounter an unexpected exception type. Depending on the host application's exception handling, this can fail requests or terminate the Node.js process. Flow sequences allow deep nesting with minimal bytes (2 bytes per level: one `[` and one `]`). On the default Node.js stack, approximately 1,000–5,000 levels of nesting (2–10 KB input) exhaust the call stack. The exact threshold is environment-dependent (Node.js version, stack size, call stack depth at invocation). Note: the library's `Parser` (CST phase) uses a stack-based iterative approach and is not affected. Only the compose/resolve phase uses actual call-stack recursion. All three public parsing APIs are affected: `YAML.parse()`, `YAML.parseDocument()`, and `YAML.parseAllDocuments()`. Versions 1.10.3 and 2.8.3 contain a patch.

- [https://github.com/danwulff/astro_CVE-2026-33532](https://github.com/danwulff/astro_CVE-2026-33532) :  ![starts](https://img.shields.io/github/stars/danwulff/astro_CVE-2026-33532.svg) ![forks](https://img.shields.io/github/forks/danwulff/astro_CVE-2026-33532.svg)


## CVE-2026-33531
 InvenTree is an Open Source Inventory Management System. Prior to version 1.2.6, a path traversal vulnerability in the report template engine allows a staff-level user to read arbitrary files from the server filesystem via crafted template tags. Affected functions: `encode_svg_image()`, `asset()`, and `uploaded_image()` in `src/backend/InvenTree/report/templatetags/report.py`. This requires staff access (to upload / edit templates with maliciously crafted tags). If the InvenTree installation is configured with high access privileges on the host system, this path traversal may allow file access outside of the InvenTree source directory. This issue is patched in version 1.2.6, and 1.3.0 (or above). Users should update to the patched versions. No known workarounds are available.

- [https://github.com/alonaki/InvenTree-Path-Traversal-CVE-2026-33531](https://github.com/alonaki/InvenTree-Path-Traversal-CVE-2026-33531) :  ![starts](https://img.shields.io/github/stars/alonaki/InvenTree-Path-Traversal-CVE-2026-33531.svg) ![forks](https://img.shields.io/github/forks/alonaki/InvenTree-Path-Traversal-CVE-2026-33531.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/z4yd3/PoC-CVE-2026-33017](https://github.com/z4yd3/PoC-CVE-2026-33017) :  ![starts](https://img.shields.io/github/stars/z4yd3/PoC-CVE-2026-33017.svg) ![forks](https://img.shields.io/github/forks/z4yd3/PoC-CVE-2026-33017.svg)


## CVE-2026-28289
 FreeScout is a free help desk and shared inbox built with PHP's Laravel framework. A patch bypass vulnerability for CVE-2026-27636 in FreeScout 1.8.206 and earlier allows any authenticated user with file upload permissions to achieve Remote Code Execution (RCE) on the server by uploading a malicious .htaccess file using a zero-width space character prefix to bypass the security check. The vulnerability exists in the sanitizeUploadedFileName() function in app/Http/Helper.php. The function contains a Time-of-Check to Time-of-Use (TOCTOU) flaw where the dot-prefix check occurs before sanitization removes invisible characters. This vulnerability is fixed in 1.8.207.

- [https://github.com/0xBlackash/CVE-2026-28289](https://github.com/0xBlackash/CVE-2026-28289) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-28289.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-28289.svg)


## CVE-2026-24061
 telnetd in GNU Inetutils through 2.7 allows remote authentication bypass via a "-f root" value for the USER environment variable.

- [https://github.com/0xBlackash/CVE-2026-24061](https://github.com/0xBlackash/CVE-2026-24061) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-24061.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-24061.svg)
- [https://github.com/franckferman/CVE_2026_24061](https://github.com/franckferman/CVE_2026_24061) :  ![starts](https://img.shields.io/github/stars/franckferman/CVE_2026_24061.svg) ![forks](https://img.shields.io/github/forks/franckferman/CVE_2026_24061.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/AhmadF77/CVE-2026-23744](https://github.com/AhmadF77/CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/AhmadF77/CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/AhmadF77/CVE-2026-23744.svg)
- [https://github.com/0xg00se/CVE-2026-23744-script](https://github.com/0xg00se/CVE-2026-23744-script) :  ![starts](https://img.shields.io/github/stars/0xg00se/CVE-2026-23744-script.svg) ![forks](https://img.shields.io/github/forks/0xg00se/CVE-2026-23744-script.svg)
- [https://github.com/fcjaviergarcia/CVE-2026-23744-POC](https://github.com/fcjaviergarcia/CVE-2026-23744-POC) :  ![starts](https://img.shields.io/github/stars/fcjaviergarcia/CVE-2026-23744-POC.svg) ![forks](https://img.shields.io/github/forks/fcjaviergarcia/CVE-2026-23744-POC.svg)


## CVE-2026-21858
 n8n is an open source workflow automation platform. Versions starting with 1.65.0 and below 1.121.0 enable an attacker to access files on the underlying server through execution of certain form-based workflows. A vulnerable workflow could grant access to an unauthenticated remote attacker, resulting in exposure of sensitive information stored on the system and may enable further compromise depending on deployment configuration and workflow usage. This issue is fixed in version 1.121.0.

- [https://github.com/0xBlackash/CVE-2026-21858](https://github.com/0xBlackash/CVE-2026-21858) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-21858.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-21858.svg)


## CVE-2026-21643
 An improper neutralization of special elements used in an sql command ('sql injection') vulnerability in Fortinet FortiClientEMS 7.4.4 may allow an unauthenticated attacker to execute unauthorized code or commands via specifically crafted HTTP requests.

- [https://github.com/alirezac0/CVE-2026-21643](https://github.com/alirezac0/CVE-2026-21643) :  ![starts](https://img.shields.io/github/stars/alirezac0/CVE-2026-21643.svg) ![forks](https://img.shields.io/github/forks/alirezac0/CVE-2026-21643.svg)


## CVE-2026-20963
 Deserialization of untrusted data in Microsoft Office SharePoint allows an authorized attacker to execute code over a network.

- [https://github.com/jenniferreire26/CVE-2026-20963](https://github.com/jenniferreire26/CVE-2026-20963) :  ![starts](https://img.shields.io/github/stars/jenniferreire26/CVE-2026-20963.svg) ![forks](https://img.shields.io/github/forks/jenniferreire26/CVE-2026-20963.svg)


## CVE-2026-4447
 Inappropriate implementation in V8 in Google Chrome prior to 146.0.7680.153 allowed a remote attacker to execute arbitrary code inside a sandbox via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/blackhatlegend/CVE-2026-4447](https://github.com/blackhatlegend/CVE-2026-4447) :  ![starts](https://img.shields.io/github/stars/blackhatlegend/CVE-2026-4447.svg) ![forks](https://img.shields.io/github/forks/blackhatlegend/CVE-2026-4447.svg)


## CVE-2026-3891
 The Pix for WooCommerce plugin for WordPress is vulnerable to arbitrary file uploads due to missing capability check and missing file type validation in the 'lkn_pix_for_woocommerce_c6_save_settings' function in all versions up to, and including, 1.5.0. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/Nxploited/CVE-2026-3891](https://github.com/Nxploited/CVE-2026-3891) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-3891.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-3891.svg)


## CVE-2026-3422
 U-Office Force developed by e-Excellence has a Insecure Deserialization vulnerability, allowing unauthenticated remote attackers to execute arbitrary code on the server by sending maliciously crafted serialized content.

- [https://github.com/skoveit/CVE-2026-34227](https://github.com/skoveit/CVE-2026-34227) :  ![starts](https://img.shields.io/github/stars/skoveit/CVE-2026-34227.svg) ![forks](https://img.shields.io/github/forks/skoveit/CVE-2026-34227.svg)


## CVE-2026-3098
 The Smart Slider 3 plugin for WordPress is vulnerable to Arbitrary File Read in all versions up to, and including, 3.5.1.33 via the 'actionExportAll' function. This makes it possible for authenticated attackers, with Subscriber-level access and above, to read the contents of arbitrary files on the server, which can contain sensitive information.

- [https://github.com/George0Papasotiriou/LLM-Jailbreak-via-Chain-of-Logic-Injection-CVE-2026-3098](https://github.com/George0Papasotiriou/LLM-Jailbreak-via-Chain-of-Logic-Injection-CVE-2026-3098) :  ![starts](https://img.shields.io/github/stars/George0Papasotiriou/LLM-Jailbreak-via-Chain-of-Logic-Injection-CVE-2026-3098.svg) ![forks](https://img.shields.io/github/forks/George0Papasotiriou/LLM-Jailbreak-via-Chain-of-Logic-Injection-CVE-2026-3098.svg)


## CVE-2026-3055
 Insufficient input validation in NetScaler ADC and NetScaler Gateway when configured as a SAML IDP leading to memory overread

- [https://github.com/RootAid/CVE-2026-3055](https://github.com/RootAid/CVE-2026-3055) :  ![starts](https://img.shields.io/github/stars/RootAid/CVE-2026-3055.svg) ![forks](https://img.shields.io/github/forks/RootAid/CVE-2026-3055.svg)


## CVE-2026-2995
 GitLab has remediated an issue in GitLab EE affecting all versions from 15.4 before 18.8.7, 18.9 before 18.9.3, and 18.10 before 18.10.1 that could have allowed an authenticated user to add email addresses to targeted user accounts due to improper sanitization of HTML content.

- [https://github.com/b0b0haha/CVE-2026-29955](https://github.com/b0b0haha/CVE-2026-29955) :  ![starts](https://img.shields.io/github/stars/b0b0haha/CVE-2026-29955.svg) ![forks](https://img.shields.io/github/forks/b0b0haha/CVE-2026-29955.svg)
- [https://github.com/b0b0haha/CVE-2026-29954](https://github.com/b0b0haha/CVE-2026-29954) :  ![starts](https://img.shields.io/github/stars/b0b0haha/CVE-2026-29954.svg) ![forks](https://img.shields.io/github/forks/b0b0haha/CVE-2026-29954.svg)


## CVE-2026-1357
 The Migration, Backup, Staging – WPvivid Backup & Migration plugin for WordPress is vulnerable to Unauthenticated Arbitrary File Upload in versions up to and including 0.9.123. This is due to improper error handling in the RSA decryption process combined with a lack of path sanitization when writing uploaded files. When the plugin fails to decrypt a session key using openssl_private_decrypt(), it does not terminate execution and instead passes the boolean false value to the phpseclib library's AES cipher initialization. The library treats this false value as a string of null bytes, allowing an attacker to encrypt a malicious payload using a predictable null-byte key. Additionally, the plugin accepts filenames from the decrypted payload without sanitization, enabling directory traversal to escape the protected backup directory. This makes it possible for unauthenticated attackers to upload arbitrary PHP files to publicly accessible directories and achieve Remote Code Execution via the wpvivid_action=send_to_site parameter.

- [https://github.com/0xBlackash/CVE-2026-1357](https://github.com/0xBlackash/CVE-2026-1357) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-1357.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-1357.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)


## CVE-2025-64446
 A relative path traversal vulnerability in Fortinet FortiWeb 8.0.0 through 8.0.1, FortiWeb 7.6.0 through 7.6.4, FortiWeb 7.4.0 through 7.4.9, FortiWeb 7.2.0 through 7.2.11, FortiWeb 7.0.0 through 7.0.11 may allow an attacker to execute administrative commands on the system via crafted HTTP or HTTPS requests.

- [https://github.com/0xBlackash/CVE-2025-64446](https://github.com/0xBlackash/CVE-2025-64446) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-64446.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-64446.svg)


## CVE-2025-49844
 Redis is an open source, in-memory database that persists on disk. Versions 8.2.1 and below allow an authenticated user to use a specially crafted Lua script to manipulate the garbage collector, trigger a use-after-free and potentially lead to remote code execution. The problem exists in all versions of Redis with Lua scripting. This issue is fixed in version 8.2.2. To workaround this issue without patching the redis-server executable is to prevent users from executing Lua scripts. This can be done using ACL to restrict EVAL and EVALSHA commands.

- [https://github.com/0xBlackash/CVE-2025-49844](https://github.com/0xBlackash/CVE-2025-49844) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-49844.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-49844.svg)


## CVE-2025-43529
 A use-after-free issue was addressed with improved memory management. This issue is fixed in watchOS 26.2, Safari 26.2, iOS 18.7.3 and iPadOS 18.7.3, iOS 26.2 and iPadOS 26.2, macOS Tahoe 26.2, visionOS 26.2, tvOS 26.2. Processing maliciously crafted web content may lead to arbitrary code execution. Apple is aware of a report that this issue may have been exploited in an extremely sophisticated attack against specific targeted individuals on versions of iOS before iOS 26. CVE-2025-14174 was also issued in response to this report.

- [https://github.com/stationedK-06/DarkSword_analysis](https://github.com/stationedK-06/DarkSword_analysis) :  ![starts](https://img.shields.io/github/stars/stationedK-06/DarkSword_analysis.svg) ![forks](https://img.shields.io/github/forks/stationedK-06/DarkSword_analysis.svg)


## CVE-2025-32463
 Sudo before 1.9.17p1 allows local users to obtain root access because /etc/nsswitch.conf from a user-controlled directory is used with the --chroot option.

- [https://github.com/0xBlackash/CVE-2025-32463](https://github.com/0xBlackash/CVE-2025-32463) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-32463.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-32463.svg)


## CVE-2025-31277
 The issue was addressed with improved memory handling. This issue is fixed in Safari 18.6, watchOS 11.6, visionOS 2.6, iOS 18.6 and iPadOS 18.6, macOS Sequoia 15.6, tvOS 18.6. Processing maliciously crafted web content may lead to memory corruption.

- [https://github.com/stationedK-06/DarkSword_analysis](https://github.com/stationedK-06/DarkSword_analysis) :  ![starts](https://img.shields.io/github/stars/stationedK-06/DarkSword_analysis.svg) ![forks](https://img.shields.io/github/forks/stationedK-06/DarkSword_analysis.svg)


## CVE-2025-14847
 Mismatched length fields in Zlib compressed protocol headers may allow a read of uninitialized heap memory by an unauthenticated client. This issue affects all MongoDB Server v7.0 prior to 7.0.28 versions, MongoDB Server v8.0 versions prior to 8.0.17, MongoDB Server v8.2 versions prior to 8.2.3, MongoDB Server v6.0 versions prior to 6.0.27, MongoDB Server v5.0 versions prior to 5.0.32, MongoDB Server v4.4 versions prior to 4.4.30, MongoDB Server v4.2 versions greater than or equal to 4.2.0, MongoDB Server v4.0 versions greater than or equal to 4.0.0, and MongoDB Server v3.6 versions greater than or equal to 3.6.0.

- [https://github.com/0xBlackash/CVE-2025-14847](https://github.com/0xBlackash/CVE-2025-14847) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-14847.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-14847.svg)


## CVE-2025-6440
 The WooCommerce Designer Pro plugin for WordPress, used by the Pricom - Printing Company & Design Services WordPress theme, is vulnerable to arbitrary file uploads due to missing file type validation in the 'wcdp_save_canvas_design_ajax' function in all versions up to, and including, 1.9.26. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/BastianXploited/CVE-2025-6440](https://github.com/BastianXploited/CVE-2025-6440) :  ![starts](https://img.shields.io/github/stars/BastianXploited/CVE-2025-6440.svg) ![forks](https://img.shields.io/github/forks/BastianXploited/CVE-2025-6440.svg)


## CVE-2025-5777
 Insufficient input validation leading to memory overread when the NetScaler is configured as a Gateway (VPN virtual server, ICA Proxy, CVPN, RDP Proxy) OR AAA virtual server

- [https://github.com/0xBlackash/CVE-2025-5777](https://github.com/0xBlackash/CVE-2025-5777) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-5777.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-5777.svg)


## CVE-2025-1383
 The Podlove Podcast Publisher plugin for WordPress is vulnerable to Cross-Site Request Forgery in all versions up to, and including, 4.2.2. This is due to missing or incorrect nonce validation on the ajax_transcript_delete() function. This makes it possible for unauthenticated attackers to delete arbitrary episode transcripts via a forged request granted they can trick a site administrator into performing an action such as clicking on a link.

- [https://github.com/sastraadiwiguna-purpleeliteteaming/CVE-2025-13834-A-Bluetooth-RFCOMM-Out-of-Bounds-Read-Vulnerability-in-Modern-Wireless-Devices](https://github.com/sastraadiwiguna-purpleeliteteaming/CVE-2025-13834-A-Bluetooth-RFCOMM-Out-of-Bounds-Read-Vulnerability-in-Modern-Wireless-Devices) :  ![starts](https://img.shields.io/github/stars/sastraadiwiguna-purpleeliteteaming/CVE-2025-13834-A-Bluetooth-RFCOMM-Out-of-Bounds-Read-Vulnerability-in-Modern-Wireless-Devices.svg) ![forks](https://img.shields.io/github/forks/sastraadiwiguna-purpleeliteteaming/CVE-2025-13834-A-Bluetooth-RFCOMM-Out-of-Bounds-Read-Vulnerability-in-Modern-Wireless-Devices.svg)


## CVE-2025-1304
 The NewsBlogger theme for WordPress is vulnerable to arbitrary file uploads due to a missing capability check on the newsblogger_install_and_activate_plugin() function in all versions up to, and including, 0.2.5.1. This makes it possible for authenticated attackers, with subscriber-level access and above, to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/Nxploited/CVE-2025-1304](https://github.com/Nxploited/CVE-2025-1304) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-1304.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-1304.svg)


## CVE-2024-38828
 Spring MVC controller methods with an @RequestBody byte[] method parameter are vulnerable to a DoS attack.

- [https://github.com/topilov/axiom-jdk-test-task](https://github.com/topilov/axiom-jdk-test-task) :  ![starts](https://img.shields.io/github/stars/topilov/axiom-jdk-test-task.svg) ![forks](https://img.shields.io/github/forks/topilov/axiom-jdk-test-task.svg)


## CVE-2024-26229
 Windows CSC Service Elevation of Privilege Vulnerability

- [https://github.com/vettrivel007/CVE-2024-26229](https://github.com/vettrivel007/CVE-2024-26229) :  ![starts](https://img.shields.io/github/stars/vettrivel007/CVE-2024-26229.svg) ![forks](https://img.shields.io/github/forks/vettrivel007/CVE-2024-26229.svg)


## CVE-2024-25600
 Improper Control of Generation of Code ('Code Injection') vulnerability in Codeer Limited Bricks Builder allows Code Injection.This issue affects Bricks Builder: from n/a through 1.9.6.

- [https://github.com/Anjai7/TryHack3M-Bricks-Heist](https://github.com/Anjai7/TryHack3M-Bricks-Heist) :  ![starts](https://img.shields.io/github/stars/Anjai7/TryHack3M-Bricks-Heist.svg) ![forks](https://img.shields.io/github/forks/Anjai7/TryHack3M-Bricks-Heist.svg)


## CVE-2024-21410
 Microsoft Exchange Server Elevation of Privilege Vulnerability

- [https://github.com/Piyush20004/SentinelStream-AI](https://github.com/Piyush20004/SentinelStream-AI) :  ![starts](https://img.shields.io/github/stars/Piyush20004/SentinelStream-AI.svg) ![forks](https://img.shields.io/github/forks/Piyush20004/SentinelStream-AI.svg)


## CVE-2022-22965
 A Spring MVC or Spring WebFlux application running on JDK 9+ may be vulnerable to remote code execution (RCE) via data binding. The specific exploit requires the application to run on Tomcat as a WAR deployment. If the application is deployed as a Spring Boot executable jar, i.e. the default, it is not vulnerable to the exploit. However, the nature of the vulnerability is more general, and there may be other ways to exploit it.

- [https://github.com/0xBlackash/CVE-2022-22965](https://github.com/0xBlackash/CVE-2022-22965) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2022-22965.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2022-22965.svg)
- [https://github.com/shoucheng3/spring-projects__spring-framework_CVE-2022-22965_5-2-19-RELEASE](https://github.com/shoucheng3/spring-projects__spring-framework_CVE-2022-22965_5-2-19-RELEASE) :  ![starts](https://img.shields.io/github/stars/shoucheng3/spring-projects__spring-framework_CVE-2022-22965_5-2-19-RELEASE.svg) ![forks](https://img.shields.io/github/forks/shoucheng3/spring-projects__spring-framework_CVE-2022-22965_5-2-19-RELEASE.svg)


## CVE-2021-20294
 A flaw was found in binutils readelf 2.35 program. An attacker who is able to convince a victim using readelf to read a crafted file could trigger a stack buffer overflow, out-of-bounds write of arbitrary data supplied by the attacker. The highest impact of this flaw is to confidentiality, integrity, and availability.

- [https://github.com/tin-z/CVE-2021-20294-POC](https://github.com/tin-z/CVE-2021-20294-POC) :  ![starts](https://img.shields.io/github/stars/tin-z/CVE-2021-20294-POC.svg) ![forks](https://img.shields.io/github/forks/tin-z/CVE-2021-20294-POC.svg)


## CVE-2020-5902
 In BIG-IP versions 15.0.0-15.1.0.3, 14.1.0-14.1.2.5, 13.1.0-13.1.3.3, 12.1.0-12.1.5.1, and 11.6.1-11.6.5.1, the Traffic Management User Interface (TMUI), also referred to as the Configuration utility, has a Remote Code Execution (RCE) vulnerability in undisclosed pages.

- [https://github.com/0xBlackash/CVE-2020-5902](https://github.com/0xBlackash/CVE-2020-5902) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2020-5902.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2020-5902.svg)


## CVE-2016-1611
 Novell Filr 1.2 before Hot Patch 6 and 2.0 before Hot Patch 2 uses world-writable permissions for /etc/profile.d/vainit.sh, which allows local users to gain privileges by replacing this file's content with arbitrary shell commands.

- [https://github.com/d3vn0mi/CVE-2016-16113-POC](https://github.com/d3vn0mi/CVE-2016-16113-POC) :  ![starts](https://img.shields.io/github/stars/d3vn0mi/CVE-2016-16113-POC.svg) ![forks](https://img.shields.io/github/forks/d3vn0mi/CVE-2016-16113-POC.svg)


## CVE-2007-1567
 Stack-based buffer overflow in War FTP Daemon 1.65, and possibly earlier, allows remote attackers to cause a denial of service or execute arbitrary code via unspecified vectors, as demonstrated by warftp_165.tar by Immunity.  NOTE: this might be the same issue as CVE-1999-0256, CVE-2000-0131, or CVE-2006-2171, but due to Immunity's lack of details, this cannot be certain.

- [https://github.com/TheMalwareGuardian/CVE-2007-1567](https://github.com/TheMalwareGuardian/CVE-2007-1567) :  ![starts](https://img.shields.io/github/stars/TheMalwareGuardian/CVE-2007-1567.svg) ![forks](https://img.shields.io/github/forks/TheMalwareGuardian/CVE-2007-1567.svg)

