# Update 2026-03-22
## CVE-2026-32941
 Sliver is a command and control framework that uses a custom Wireguard netstack. Versions 1.7.3 and below contain a Remote OOM (Out-of-Memory) vulnerability in the Sliver C2 server's mTLS and WireGuard C2 transport layer. The socketReadEnvelope and socketWGReadEnvelope functions trust an attacker-controlled 4-byte length prefix to allocate memory, with ServerMaxMessageSize allowing single allocations of up to ~2 GiB. A compromised implant or an attacker with valid credentials can exploit this by sending fabricated length prefixes over concurrent yamux streams (up to 128 per connection), forcing the server to attempt allocating ~256 GiB of memory and triggering an OS OOM kill. This crashes the Sliver server, disrupts all active implant sessions, and may degrade or kill other processes sharing the same host. The same pattern also affects all implant-side readers, which have no upper-bound check at all. The issue was not fixed at the the time of publication.

- [https://github.com/skoveit/CVE-2026-32941](https://github.com/skoveit/CVE-2026-32941) :  ![starts](https://img.shields.io/github/stars/skoveit/CVE-2026-32941.svg) ![forks](https://img.shields.io/github/forks/skoveit/CVE-2026-32941.svg)


## CVE-2026-32746
 telnetd in GNU inetutils through 2.7 allows an out-of-bounds write in the LINEMODE SLC (Set Local Characters) suboption handler because add_slc does not check whether the buffer is full.

- [https://github.com/chosenonehacks/CVE-2026-32746](https://github.com/chosenonehacks/CVE-2026-32746) :  ![starts](https://img.shields.io/github/stars/chosenonehacks/CVE-2026-32746.svg) ![forks](https://img.shields.io/github/forks/chosenonehacks/CVE-2026-32746.svg)
- [https://github.com/danindiana/cve-2026-32746-mitigation](https://github.com/danindiana/cve-2026-32746-mitigation) :  ![starts](https://img.shields.io/github/stars/danindiana/cve-2026-32746-mitigation.svg) ![forks](https://img.shields.io/github/forks/danindiana/cve-2026-32746-mitigation.svg)


## CVE-2026-22730
The vulnerability exists due to missing input sanitization.

- [https://github.com/NULL200OK/CVE-2026-22730-Scanner](https://github.com/NULL200OK/CVE-2026-22730-Scanner) :  ![starts](https://img.shields.io/github/stars/NULL200OK/CVE-2026-22730-Scanner.svg) ![forks](https://img.shields.io/github/forks/NULL200OK/CVE-2026-22730-Scanner.svg)


## CVE-2026-21992
 Vulnerability in the Oracle Identity Manager product of Oracle Fusion Middleware (component: REST WebServices) and Oracle Web Services Manager product of Oracle Fusion Middleware (component: Web Services Security).  Supported versions that are affected are 12.2.1.4.0 and  14.1.2.1.0. Easily exploitable vulnerability allows unauthenticated attacker with network access via HTTP to compromise Oracle Identity Manager and Oracle Web Services Manager.  Successful attacks of this vulnerability can result in takeover of Oracle Identity Manager and Oracle Web Services Manager. Note: Oracle Web Services Manager is installed with an Oracle Fusion Middleware Infrastructure. CVSS 3.1 Base Score 9.8 (Confidentiality, Integrity and Availability impacts).  CVSS Vector: (CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H).

- [https://github.com/TEXploited/CVE-2026-21992](https://github.com/TEXploited/CVE-2026-21992) :  ![starts](https://img.shields.io/github/stars/TEXploited/CVE-2026-21992.svg) ![forks](https://img.shields.io/github/forks/TEXploited/CVE-2026-21992.svg)


## CVE-2026-20643
 A cross-origin issue in the Navigation API was addressed with improved input validation. This issue is fixed in Background Security Improvements for iOS 26.3.1, iPadOS 26.3.1, macOS 26.3.1, and macOS 26.3.2. Processing maliciously crafted web content may bypass Same Origin Policy.

- [https://github.com/Fliv/CVE-2026-20643](https://github.com/Fliv/CVE-2026-20643) :  ![starts](https://img.shields.io/github/stars/Fliv/CVE-2026-20643.svg) ![forks](https://img.shields.io/github/forks/Fliv/CVE-2026-20643.svg)


## CVE-2026-4342
 A security issue was discovered in ingress-nginx where a combination of Ingress annotations can be used to inject configuration into nginx. This can lead to arbitrary code execution in the context of the ingress-nginx controller, and disclosure of Secrets accessible to the controller. (Note that in the default installation, the controller can access all Secrets cluster-wide.)

- [https://github.com/stuartMoorhouse/CVE-2026-4342](https://github.com/stuartMoorhouse/CVE-2026-4342) :  ![starts](https://img.shields.io/github/stars/stuartMoorhouse/CVE-2026-4342.svg) ![forks](https://img.shields.io/github/forks/stuartMoorhouse/CVE-2026-4342.svg)


## CVE-2026-3888
 Local privilege escalation in snapd on Linux allows local attackers to get root privilege by re-creating snap's private /tmp directory when systemd-tmpfiles is configured to automatically clean up this directory. This issue affects Ubuntu 16.04 LTS, 18.04 LTS, 20.04 LTS, 22.04 LTS, and 24.04 LTS.

- [https://github.com/netw0rk7/CVE-2026-3888-PoC](https://github.com/netw0rk7/CVE-2026-3888-PoC) :  ![starts](https://img.shields.io/github/stars/netw0rk7/CVE-2026-3888-PoC.svg) ![forks](https://img.shields.io/github/forks/netw0rk7/CVE-2026-3888-PoC.svg)


## CVE-2026-2964
 A vulnerability was identified in higuma web-audio-recorder-js 0.1/0.1.1. Impacted is the function extend in the library lib/WebAudioRecorder.js of the component Dynamic Config Handling. Such manipulation leads to improperly controlled modification of object prototype attributes. It is possible to launch the attack remotely. Attacks of this nature are highly complex. The exploitability is considered difficult. The exploit is publicly available and might be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/thegenetic/CVE-2026-2964-Lab](https://github.com/thegenetic/CVE-2026-2964-Lab) :  ![starts](https://img.shields.io/github/stars/thegenetic/CVE-2026-2964-Lab.svg) ![forks](https://img.shields.io/github/forks/thegenetic/CVE-2026-2964-Lab.svg)


## CVE-2026-2631
 The Datalogics Ecommerce Delivery  WordPress plugin before 2.6.60 exposes an unauthenticated REST endpoint that allows any remote user to modify the option `datalogics_token` without verification. This token is subsequently used for authentication in a protected endpoint that allows users to perform arbitrary WordPress `update_option()` operations. Attackers can use this to enable registartion and to set the default role as Administrator.

- [https://github.com/Nxploited/CVE-2026-2631](https://github.com/Nxploited/CVE-2026-2631) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-2631.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-2631.svg)


## CVE-2026-1731
 BeyondTrust Remote Support (RS) and certain older versions of Privileged Remote Access (PRA) contain a critical pre-authentication remote code execution vulnerability. By sending specially crafted requests, an unauthenticated remote attacker may be able to execute operating system commands in the context of the site user.

- [https://github.com/LutfifakeeXone/CVE-2026-1731](https://github.com/LutfifakeeXone/CVE-2026-1731) :  ![starts](https://img.shields.io/github/stars/LutfifakeeXone/CVE-2026-1731.svg) ![forks](https://img.shields.io/github/forks/LutfifakeeXone/CVE-2026-1731.svg)


## CVE-2026-1492
 The User Registration & Membership – Custom Registration Form Builder, Custom Login Form, User Profile, Content Restriction & Membership Plugin plugin for WordPress is vulnerable to improper privilege management in all versions up to, and including, 5.1.2. This is due to the plugin accepting a user-supplied role during membership registration without properly enforcing a server-side allowlist. This makes it possible for unauthenticated attackers to create administrator accounts by supplying a role value during membership registration.

- [https://github.com/the8frust/CVE-2026-1492](https://github.com/the8frust/CVE-2026-1492) :  ![starts](https://img.shields.io/github/stars/the8frust/CVE-2026-1492.svg) ![forks](https://img.shields.io/github/forks/the8frust/CVE-2026-1492.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)


## CVE-2025-49144
 Notepad++ is a free and open-source source code editor. In versions 8.8.1 and prior, a privilege escalation vulnerability exists in the Notepad++ v8.8.1 installer that allows unprivileged users to gain SYSTEM-level privileges through insecure executable search paths. An attacker could use social engineering or clickjacking to trick users into downloading both the legitimate installer and a malicious executable to the same directory (typically Downloads folder - which is known as Vulnerable directory). Upon running the installer, the attack executes automatically with SYSTEM privileges. This issue has been fixed and will be released in version 8.8.2.

- [https://github.com/havertz2110/CVE-2025-49144-PoC](https://github.com/havertz2110/CVE-2025-49144-PoC) :  ![starts](https://img.shields.io/github/stars/havertz2110/CVE-2025-49144-PoC.svg) ![forks](https://img.shields.io/github/forks/havertz2110/CVE-2025-49144-PoC.svg)


## CVE-2025-48784
 A missing authorization vulnerability in Soar Cloud HRD Human Resource Management System through version 7.3.2025.0408 allows remote attackers to modify system settings without prior authorization.

- [https://github.com/h3raklez/CVE-2025-48784](https://github.com/h3raklez/CVE-2025-48784) :  ![starts](https://img.shields.io/github/stars/h3raklez/CVE-2025-48784.svg) ![forks](https://img.shields.io/github/forks/h3raklez/CVE-2025-48784.svg)


## CVE-2025-48734
 2.x are recommended to upgrade to version 2.0.0-M2, which fixes the issue.

- [https://github.com/h3raklez/CVE-2025-48784](https://github.com/h3raklez/CVE-2025-48784) :  ![starts](https://img.shields.io/github/stars/h3raklez/CVE-2025-48784.svg) ![forks](https://img.shields.io/github/forks/h3raklez/CVE-2025-48784.svg)


## CVE-2025-48384
 Git is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals. When reading a config value, Git strips any trailing carriage return and line feed (CRLF). When writing a config entry, values with a trailing CR are not quoted, causing the CR to be lost when the config is later read. When initializing a submodule, if the submodule path contains a trailing CR, the altered path is read resulting in the submodule being checked out to an incorrect location. If a symlink exists that points the altered path to the submodule hooks directory, and the submodule contains an executable post-checkout hook, the script may be unintentionally executed after checkout. This vulnerability is fixed in v2.43.7, v2.44.4, v2.45.4, v2.46.4, v2.47.3, v2.48.2, v2.49.1, and v2.50.1.

- [https://github.com/anthonyc53/cve-2025-48384](https://github.com/anthonyc53/cve-2025-48384) :  ![starts](https://img.shields.io/github/stars/anthonyc53/cve-2025-48384.svg) ![forks](https://img.shields.io/github/forks/anthonyc53/cve-2025-48384.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/KaztoRay/CVE-2025-29927-Research](https://github.com/KaztoRay/CVE-2025-29927-Research) :  ![starts](https://img.shields.io/github/stars/KaztoRay/CVE-2025-29927-Research.svg) ![forks](https://img.shields.io/github/forks/KaztoRay/CVE-2025-29927-Research.svg)


## CVE-2025-11926
 The Related Posts Lite plugin for WordPress is vulnerable to Stored Cross-Site Scripting via admin settings in all versions up to, and including, 1.12 due to insufficient input sanitization and output escaping. This makes it possible for authenticated attackers, with administrator-level permissions and above, to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page. This only affects multi-site installations and installations where unfiltered_html has been disabled.

- [https://github.com/prabhatverma47/CVE-2025-11926](https://github.com/prabhatverma47/CVE-2025-11926) :  ![starts](https://img.shields.io/github/stars/prabhatverma47/CVE-2025-11926.svg) ![forks](https://img.shields.io/github/forks/prabhatverma47/CVE-2025-11926.svg)


## CVE-2025-6934
 The Opal Estate Pro – Property Management and Submission plugin for WordPress, used by the FullHouse - Real Estate Responsive WordPress Theme, is vulnerable to privilege escalation via in all versions up to, and including, 1.7.5. This is due to a lack of role restriction during registration in the 'on_regiser_user' function. This makes it possible for unauthenticated attackers to arbitrarily choose the role, including the Administrator role, assigned when registering.

- [https://github.com/MejbanKadir/CVE-2025-6934-PoC](https://github.com/MejbanKadir/CVE-2025-6934-PoC) :  ![starts](https://img.shields.io/github/stars/MejbanKadir/CVE-2025-6934-PoC.svg) ![forks](https://img.shields.io/github/forks/MejbanKadir/CVE-2025-6934-PoC.svg)


## CVE-2025-3248
code.

- [https://github.com/nebari-playground/langflow-cve-2025-3248](https://github.com/nebari-playground/langflow-cve-2025-3248) :  ![starts](https://img.shields.io/github/stars/nebari-playground/langflow-cve-2025-3248.svg) ![forks](https://img.shields.io/github/forks/nebari-playground/langflow-cve-2025-3248.svg)


## CVE-2025-1489
 The WP-Appbox plugin for WordPress is vulnerable to Stored Cross-Site Scripting via the plugin's appbox shortcode in all versions up to, and including, 4.5.4 due to insufficient input sanitization and output escaping on user supplied attributes. This makes it possible for authenticated attackers, with contributor-level access and above, to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page.

- [https://github.com/khaifunglee/reproducing-CVE-2025-1489](https://github.com/khaifunglee/reproducing-CVE-2025-1489) :  ![starts](https://img.shields.io/github/stars/khaifunglee/reproducing-CVE-2025-1489.svg) ![forks](https://img.shields.io/github/forks/khaifunglee/reproducing-CVE-2025-1489.svg)


## CVE-2024-36991
 In Splunk Enterprise on Windows versions below 9.2.2, 9.1.5, and 9.0.10, an attacker could perform a path traversal on the /modules/messaging/ endpoint in Splunk Enterprise on Windows. This vulnerability should only affect Splunk Enterprise on Windows.

- [https://github.com/jhurtadomi/CVE-2024-36991-Splunk](https://github.com/jhurtadomi/CVE-2024-36991-Splunk) :  ![starts](https://img.shields.io/github/stars/jhurtadomi/CVE-2024-36991-Splunk.svg) ![forks](https://img.shields.io/github/forks/jhurtadomi/CVE-2024-36991-Splunk.svg)


## CVE-2021-42574
 An issue was discovered in the Bidirectional Algorithm in the Unicode Specification through 14.0. It permits the visual reordering of characters via control sequences, which can be used to craft source code that renders different logic than the logical ordering of tokens ingested by compilers and interpreters. Adversaries can leverage this to encode source code for compilers accepting Unicode such that targeted vulnerabilities are introduced invisibly to human reviewers. NOTE: the Unicode Consortium offers the following alternative approach to presenting this concern. An issue is noted in the nature of international text that can affect applications that implement support for The Unicode Standard and the Unicode Bidirectional Algorithm (all versions). Due to text display behavior when text includes left-to-right and right-to-left characters, the visual order of tokens may be different from their logical order. Additionally, control characters needed to fully support the requirements of bidirectional text can further obfuscate the logical order of tokens. Unless mitigated, an adversary could craft source code such that the ordering of tokens perceived by human reviewers does not match what will be processed by a compiler/interpreter/etc. The Unicode Consortium has documented this class of vulnerability in its document, Unicode Technical Report #36, Unicode Security Considerations. The Unicode Consortium also provides guidance on mitigations for this class of issues in Unicode Technical Standard #39, Unicode Security Mechanisms, and in Unicode Standard Annex #31, Unicode Identifier and Pattern Syntax. Also, the BIDI specification allows applications to tailor the implementation in ways that can mitigate misleading visual reordering in program text; see HL4 in Unicode Standard Annex #9, Unicode Bidirectional Algorithm.

- [https://github.com/Moshe-ship/bidi-guard](https://github.com/Moshe-ship/bidi-guard) :  ![starts](https://img.shields.io/github/stars/Moshe-ship/bidi-guard.svg) ![forks](https://img.shields.io/github/forks/Moshe-ship/bidi-guard.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/Taldrid1/cve-2021-41773](https://github.com/Taldrid1/cve-2021-41773) :  ![starts](https://img.shields.io/github/stars/Taldrid1/cve-2021-41773.svg) ![forks](https://img.shields.io/github/forks/Taldrid1/cve-2021-41773.svg)


## CVE-2021-38163
 SAP NetWeaver (Visual Composer 7.0 RT) versions - 7.30, 7.31, 7.40, 7.50, without restriction, an attacker authenticated as a non-administrative user can upload a malicious file over a network and trigger its processing, which is capable of running operating system commands with the privilege of the Java Server process. These commands can be used to read or modify any information on the server or shut the server down making it unavailable.

- [https://github.com/core1impact/CVE-2021-38163](https://github.com/core1impact/CVE-2021-38163) :  ![starts](https://img.shields.io/github/stars/core1impact/CVE-2021-38163.svg) ![forks](https://img.shields.io/github/forks/core1impact/CVE-2021-38163.svg)
- [https://github.com/purpleteam-ru/CVE-2021-38163](https://github.com/purpleteam-ru/CVE-2021-38163) :  ![starts](https://img.shields.io/github/stars/purpleteam-ru/CVE-2021-38163.svg) ![forks](https://img.shields.io/github/forks/purpleteam-ru/CVE-2021-38163.svg)


## CVE-2021-38149
 index.php/admin/add_user in Chikitsa Patient Management System 2.0.0 allows XSS.

- [https://github.com/jboogie15/CVE-2021-38149](https://github.com/jboogie15/CVE-2021-38149) :  ![starts](https://img.shields.io/github/stars/jboogie15/CVE-2021-38149.svg) ![forks](https://img.shields.io/github/forks/jboogie15/CVE-2021-38149.svg)


## CVE-2021-29447
 Wordpress is an open source CMS. A user with the ability to upload files (like an Author) can exploit an XML parsing issue in the Media Library leading to XXE attacks. This requires WordPress installation to be using PHP 8. Access to internal files is possible in a successful XXE attack. This has been patched in WordPress version 5.7.1, along with the older affected versions via a minor release. We strongly recommend you keep auto-updates enabled.

- [https://github.com/danilo1992-sys/CVE-2021-29447](https://github.com/danilo1992-sys/CVE-2021-29447) :  ![starts](https://img.shields.io/github/stars/danilo1992-sys/CVE-2021-29447.svg) ![forks](https://img.shields.io/github/forks/danilo1992-sys/CVE-2021-29447.svg)


## CVE-2021-26904
 LMA ISIDA Retriever 5.2 allows SQL Injection.

- [https://github.com/Security-AVS/-CVE-2021-26904](https://github.com/Security-AVS/-CVE-2021-26904) :  ![starts](https://img.shields.io/github/stars/Security-AVS/-CVE-2021-26904.svg) ![forks](https://img.shields.io/github/forks/Security-AVS/-CVE-2021-26904.svg)


## CVE-2021-26882
 Remote Access API Elevation of Privilege Vulnerability

- [https://github.com/taiji-xo/CVE-2021-26882](https://github.com/taiji-xo/CVE-2021-26882) :  ![starts](https://img.shields.io/github/stars/taiji-xo/CVE-2021-26882.svg) ![forks](https://img.shields.io/github/forks/taiji-xo/CVE-2021-26882.svg)


## CVE-2021-26868
 Windows Graphics Component Elevation of Privilege Vulnerability

- [https://github.com/Ascotbe/Kernelhub](https://github.com/Ascotbe/Kernelhub) :  ![starts](https://img.shields.io/github/stars/Ascotbe/Kernelhub.svg) ![forks](https://img.shields.io/github/forks/Ascotbe/Kernelhub.svg)
- [https://github.com/KangD1W2/CVE-2021-26868](https://github.com/KangD1W2/CVE-2021-26868) :  ![starts](https://img.shields.io/github/stars/KangD1W2/CVE-2021-26868.svg) ![forks](https://img.shields.io/github/forks/KangD1W2/CVE-2021-26868.svg)


## CVE-2021-26865
 Windows Container Execution Agent Elevation of Privilege Vulnerability

- [https://github.com/soteria-security/HAFNIUM-IOC](https://github.com/soteria-security/HAFNIUM-IOC) :  ![starts](https://img.shields.io/github/stars/soteria-security/HAFNIUM-IOC.svg) ![forks](https://img.shields.io/github/forks/soteria-security/HAFNIUM-IOC.svg)
- [https://github.com/Yt1g3r/CVE-2021-26855_SSRF](https://github.com/Yt1g3r/CVE-2021-26855_SSRF) :  ![starts](https://img.shields.io/github/stars/Yt1g3r/CVE-2021-26855_SSRF.svg) ![forks](https://img.shields.io/github/forks/Yt1g3r/CVE-2021-26855_SSRF.svg)
- [https://github.com/34zY/APT-Backpack](https://github.com/34zY/APT-Backpack) :  ![starts](https://img.shields.io/github/stars/34zY/APT-Backpack.svg) ![forks](https://img.shields.io/github/forks/34zY/APT-Backpack.svg)


## CVE-2021-26714
 The Enterprise License Manager portal in Mitel MiContact Center Enterprise before 9.4 could allow a user to access restricted files and folders due to insufficient access control. A successful exploit could allow an attacker to view and modify application data via Directory Traversal.

- [https://github.com/PwCNO-CTO/CVE-2021-26714](https://github.com/PwCNO-CTO/CVE-2021-26714) :  ![starts](https://img.shields.io/github/stars/PwCNO-CTO/CVE-2021-26714.svg) ![forks](https://img.shields.io/github/forks/PwCNO-CTO/CVE-2021-26714.svg)


## CVE-2021-26415
 Windows Installer Elevation of Privilege Vulnerability

- [https://github.com/adenkiewicz/CVE-2021-26415](https://github.com/adenkiewicz/CVE-2021-26415) :  ![starts](https://img.shields.io/github/stars/adenkiewicz/CVE-2021-26415.svg) ![forks](https://img.shields.io/github/forks/adenkiewicz/CVE-2021-26415.svg)


## CVE-2021-26411
 Internet Explorer Memory Corruption Vulnerability

- [https://github.com/CrackerCat/CVE-2021-26411](https://github.com/CrackerCat/CVE-2021-26411) :  ![starts](https://img.shields.io/github/stars/CrackerCat/CVE-2021-26411.svg) ![forks](https://img.shields.io/github/forks/CrackerCat/CVE-2021-26411.svg)


## CVE-2021-26295
 Apache OFBiz has unsafe deserialization prior to 17.12.06. An unauthenticated attacker can use this vulnerability to successfully take over Apache OFBiz.

- [https://github.com/yumusb/CVE-2021-26295](https://github.com/yumusb/CVE-2021-26295) :  ![starts](https://img.shields.io/github/stars/yumusb/CVE-2021-26295.svg) ![forks](https://img.shields.io/github/forks/yumusb/CVE-2021-26295.svg)
- [https://github.com/yuaneuro/ofbiz-poc](https://github.com/yuaneuro/ofbiz-poc) :  ![starts](https://img.shields.io/github/stars/yuaneuro/ofbiz-poc.svg) ![forks](https://img.shields.io/github/forks/yuaneuro/ofbiz-poc.svg)
- [https://github.com/rakjong/CVE-2021-26295-Apache-OFBiz](https://github.com/rakjong/CVE-2021-26295-Apache-OFBiz) :  ![starts](https://img.shields.io/github/stars/rakjong/CVE-2021-26295-Apache-OFBiz.svg) ![forks](https://img.shields.io/github/forks/rakjong/CVE-2021-26295-Apache-OFBiz.svg)
- [https://github.com/dskho/CVE-2021-26295](https://github.com/dskho/CVE-2021-26295) :  ![starts](https://img.shields.io/github/stars/dskho/CVE-2021-26295.svg) ![forks](https://img.shields.io/github/forks/dskho/CVE-2021-26295.svg)
- [https://github.com/DarkFunct/exp_hub](https://github.com/DarkFunct/exp_hub) :  ![starts](https://img.shields.io/github/stars/DarkFunct/exp_hub.svg) ![forks](https://img.shields.io/github/forks/DarkFunct/exp_hub.svg)
- [https://github.com/coolyin001/CVE-2021-26295--](https://github.com/coolyin001/CVE-2021-26295--) :  ![starts](https://img.shields.io/github/stars/coolyin001/CVE-2021-26295--.svg) ![forks](https://img.shields.io/github/forks/coolyin001/CVE-2021-26295--.svg)


## CVE-2021-3492
 Shiftfs, an out-of-tree stacking file system included in Ubuntu Linux kernels, did not properly handle faults occurring during copy_from_user() correctly. These could lead to either a double-free situation or memory not being freed at all. An attacker could use this to cause a denial of service (kernel memory exhaustion) or gain privileges via executing arbitrary code. AKA ZDI-CAN-13562.

- [https://github.com/synacktiv/CVE-2021-3492](https://github.com/synacktiv/CVE-2021-3492) :  ![starts](https://img.shields.io/github/stars/synacktiv/CVE-2021-3492.svg) ![forks](https://img.shields.io/github/forks/synacktiv/CVE-2021-3492.svg)


## CVE-2019-9511
 Some HTTP/2 implementations are vulnerable to window size manipulation and stream prioritization manipulation, potentially leading to a denial of service. The attacker requests a large amount of data from a specified resource over multiple streams. They manipulate window size and stream priority to force the server to queue the data in 1-byte chunks. Depending on how efficiently this data is queued, this can consume excess CPU, memory, or both.

- [https://github.com/flyniu666/ingress-nginx-0.21-1.19.5](https://github.com/flyniu666/ingress-nginx-0.21-1.19.5) :  ![starts](https://img.shields.io/github/stars/flyniu666/ingress-nginx-0.21-1.19.5.svg) ![forks](https://img.shields.io/github/forks/flyniu666/ingress-nginx-0.21-1.19.5.svg)


## CVE-2019-7609
 Kibana versions before 5.6.15 and 6.6.1 contain an arbitrary code execution flaw in the Timelion visualizer. An attacker with access to the Timelion application could send a request that will attempt to execute javascript code. This could possibly lead to an attacker executing arbitrary commands with permissions of the Kibana process on the host system.

- [https://github.com/d0x-awrqxavc/CVE-2019-7609-KibanaRCE](https://github.com/d0x-awrqxavc/CVE-2019-7609-KibanaRCE) :  ![starts](https://img.shields.io/github/stars/d0x-awrqxavc/CVE-2019-7609-KibanaRCE.svg) ![forks](https://img.shields.io/github/forks/d0x-awrqxavc/CVE-2019-7609-KibanaRCE.svg)


## CVE-2018-8033
 In Apache OFBiz 16.11.01 to 16.11.04, the OFBiz HTTP engine (org.apache.ofbiz.service.engine.HttpEngine.java) handles requests for HTTP services via the /webtools/control/httpService endpoint. Both POST and GET requests to the httpService endpoint may contain three parameters: serviceName, serviceMode, and serviceContext. The exploitation occurs by having DOCTYPEs pointing to external references that trigger a payload that returns secret information from the host.

- [https://github.com/jamieparfet/Apache-OFBiz-XXE](https://github.com/jamieparfet/Apache-OFBiz-XXE) :  ![starts](https://img.shields.io/github/stars/jamieparfet/Apache-OFBiz-XXE.svg) ![forks](https://img.shields.io/github/forks/jamieparfet/Apache-OFBiz-XXE.svg)
- [https://github.com/Cappricio-Securities/CVE-2018-8033](https://github.com/Cappricio-Securities/CVE-2018-8033) :  ![starts](https://img.shields.io/github/stars/Cappricio-Securities/CVE-2018-8033.svg) ![forks](https://img.shields.io/github/forks/Cappricio-Securities/CVE-2018-8033.svg)

