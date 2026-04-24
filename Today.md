# Update 2026-04-24
## CVE-2026-34197
Users are recommended to upgrade to version 5.19.4 or 6.2.3, which fixes the issue

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2026-33937
 Handlebars provides the power necessary to let users build semantic templates. In versions 4.0.0 through 4.7.8, `Handlebars.compile()` accepts a pre-parsed AST object in addition to a template string. The `value` field of a `NumberLiteral` AST node is emitted directly into the generated JavaScript without quoting or sanitization. An attacker who can supply a crafted AST to `compile()` can therefore inject and execute arbitrary JavaScript, leading to Remote Code Execution on the server. Version 4.7.9 fixes the issue. Some workarounds are available. Validate input type before calling `Handlebars.compile()`; ensure the argument is always a  `string`, never a plain object or JSON-deserialized value. Use the Handlebars runtime-only build (`handlebars/runtime`) on the server if templates are pre-compiled at build time; `compile()` will be unavailable.

- [https://github.com/EQSTLab/CVE-2026-33937](https://github.com/EQSTLab/CVE-2026-33937) :  ![starts](https://img.shields.io/github/stars/EQSTLab/CVE-2026-33937.svg) ![forks](https://img.shields.io/github/forks/EQSTLab/CVE-2026-33937.svg)


## CVE-2026-33827
 Concurrent execution using shared resource with improper synchronization ('race condition') in Windows TCP/IP allows an unauthorized attacker to execute code over a network.

- [https://github.com/kaleth4/CVE-2026-33827](https://github.com/kaleth4/CVE-2026-33827) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-33827.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-33827.svg)


## CVE-2026-33826
 Improper input validation in Windows Active Directory allows an authorized attacker to execute code over an adjacent network.

- [https://github.com/kaleth4/CVE-2026-33826](https://github.com/kaleth4/CVE-2026-33826) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-33826.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-33826.svg)


## CVE-2026-33825
 Insufficient granularity of access control in Microsoft Defender allows an authorized attacker to elevate privileges locally.

- [https://github.com/kaleth4/CVE-2026-33825](https://github.com/kaleth4/CVE-2026-33825) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-33825.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-33825.svg)


## CVE-2026-33656
 EspoCRM is an open source customer relationship management application. Prior to version 9.3.4, EspoCRM's built-in formula scripting engine allowing updating attachment's sourceId thus allowing an authenticated admin to overwrite the `sourceId` field on `Attachment` entities. Because `sourceId` is concatenated directly into a file path with no sanitization in `EspoUploadDir::getFilePath()`, an attacker can redirect any file read or write operation to an arbitrary path within the web server's `open_basedir` scope. Version 9.3.4 fixes the issue.

- [https://github.com/JivaSecurity/ESPOCRM-RCE-POC-CVE-2026-33656](https://github.com/JivaSecurity/ESPOCRM-RCE-POC-CVE-2026-33656) :  ![starts](https://img.shields.io/github/stars/JivaSecurity/ESPOCRM-RCE-POC-CVE-2026-33656.svg) ![forks](https://img.shields.io/github/forks/JivaSecurity/ESPOCRM-RCE-POC-CVE-2026-33656.svg)


## CVE-2026-32201
 Improper input validation in Microsoft Office SharePoint allows an unauthorized attacker to perform spoofing over a network.

- [https://github.com/B1tBit/CVE-2026-32201-exploit](https://github.com/B1tBit/CVE-2026-32201-exploit) :  ![starts](https://img.shields.io/github/stars/B1tBit/CVE-2026-32201-exploit.svg) ![forks](https://img.shields.io/github/forks/B1tBit/CVE-2026-32201-exploit.svg)


## CVE-2026-26026
 GLPI is a free asset and IT management software package. From 11.0.0 to before 11.0.6, template injection by an administrator lead to RCE. This vulnerability is fixed in 11.0.6.

- [https://github.com/CEAarab/CVE-2026-26026-PoC](https://github.com/CEAarab/CVE-2026-26026-PoC) :  ![starts](https://img.shields.io/github/stars/CEAarab/CVE-2026-26026-PoC.svg) ![forks](https://img.shields.io/github/forks/CEAarab/CVE-2026-26026-PoC.svg)


## CVE-2026-25604
You should upgrade to 9.22.0 version of provider if you use AWS Auth Manager.

- [https://github.com/John-Jung/CVE-2026-25604-PoC](https://github.com/John-Jung/CVE-2026-25604-PoC) :  ![starts](https://img.shields.io/github/stars/John-Jung/CVE-2026-25604-PoC.svg) ![forks](https://img.shields.io/github/forks/John-Jung/CVE-2026-25604-PoC.svg)


## CVE-2026-21877
 n8n is an open source workflow automation platform. In versions 0.121.2 and below, an authenticated attacker may be able to execute malicious code using the n8n service. This could result in full compromise and can impact both self-hosted and n8n Cloud instances. This issue is fixed in version 1.121.3. Administrators can reduce exposure by disabling the Git node and limiting access for untrusted users, but upgrading to the latest version is recommended.

- [https://github.com/CVEs-Labs/CVE-2026-21877](https://github.com/CVEs-Labs/CVE-2026-21877) :  ![starts](https://img.shields.io/github/stars/CVEs-Labs/CVE-2026-21877.svg) ![forks](https://img.shields.io/github/forks/CVEs-Labs/CVE-2026-21877.svg)


## CVE-2026-21876
 The OWASP core rule set (CRS) is a set of generic attack detection rules for use with compatible web application firewalls. Prior to versions 4.22.0 and 3.3.8, the current rule 922110 has a bug when processing multipart requests with multiple parts. When the first rule in a chain iterates over a collection (like `MULTIPART_PART_HEADERS`), the capture variables (`TX:0`, `TX:1`) get overwritten with each iteration. Only the last captured value is available to the chained rule, which means malicious charsets in earlier parts can be missed if a later part has a legitimate charset. Versions 4.22.0 and 3.3.8 patch the issue.

- [https://github.com/CVEs-Labs/CVE-2026-21876](https://github.com/CVEs-Labs/CVE-2026-21876) :  ![starts](https://img.shields.io/github/stars/CVEs-Labs/CVE-2026-21876.svg) ![forks](https://img.shields.io/github/forks/CVEs-Labs/CVE-2026-21876.svg)


## CVE-2026-20687
 A use after free issue was addressed with improved memory management. This issue is fixed in iOS 18.7.7 and iPadOS 18.7.7, iOS 26.4 and iPadOS 26.4, macOS Sequoia 15.7.5, macOS Tahoe 26.4, tvOS 26.4, watchOS 26.4. An app may be able to cause unexpected system termination or write kernel memory.

- [https://github.com/enfilade-labs/CVE-2026-20687-AppleJPEGDriver-UAF](https://github.com/enfilade-labs/CVE-2026-20687-AppleJPEGDriver-UAF) :  ![starts](https://img.shields.io/github/stars/enfilade-labs/CVE-2026-20687-AppleJPEGDriver-UAF.svg) ![forks](https://img.shields.io/github/forks/enfilade-labs/CVE-2026-20687-AppleJPEGDriver-UAF.svg)


## CVE-2026-20637
 A use after free issue was addressed with improved memory management. This issue is fixed in iOS 18.7.7 and iPadOS 18.7.7, iOS 26.3 and iPadOS 26.3, macOS Sequoia 15.7.5, macOS Sonoma 14.8.5, macOS Tahoe 26.3, tvOS 26.3, visionOS 26.3, watchOS 26.3. An app may be able to cause unexpected system termination.

- [https://github.com/enfilade-labs/CVE-2026-20637-AppleSEPKeyStore-UAF](https://github.com/enfilade-labs/CVE-2026-20637-AppleSEPKeyStore-UAF) :  ![starts](https://img.shields.io/github/stars/enfilade-labs/CVE-2026-20637-AppleSEPKeyStore-UAF.svg) ![forks](https://img.shields.io/github/forks/enfilade-labs/CVE-2026-20637-AppleSEPKeyStore-UAF.svg)


## CVE-2026-6356
 A vulnerability in the web application allows standard users to escalate their privileges to those of a super administrator through parameter manipulation, enabling them to access and modify sensitive information.

- [https://github.com/Penguinsecq/CVE-2026-6356](https://github.com/Penguinsecq/CVE-2026-6356) :  ![starts](https://img.shields.io/github/stars/Penguinsecq/CVE-2026-6356.svg) ![forks](https://img.shields.io/github/forks/Penguinsecq/CVE-2026-6356.svg)


## CVE-2026-6355
 A vulnerability in the web application allows unauthorized users to access and manipulate sensitive data across different tenants by exploiting insecure direct object references. This could lead to unauthorized access to sensitive information and unauthorized changes to the tenant's configuration.

- [https://github.com/Penguinsecq/CVE-2026-6355](https://github.com/Penguinsecq/CVE-2026-6355) :  ![starts](https://img.shields.io/github/stars/Penguinsecq/CVE-2026-6355.svg) ![forks](https://img.shields.io/github/forks/Penguinsecq/CVE-2026-6355.svg)


## CVE-2026-4157
The specific flaw exists within the handling of OCPP messages. The issue results from the lack of proper validation of a user-supplied string before using it to execute a system call. An attacker can leverage this vulnerability to execute code in the context of root. Was ZDI-CAN-26338.

- [https://github.com/krraze/CVE-2026-41575](https://github.com/krraze/CVE-2026-41575) :  ![starts](https://img.shields.io/github/stars/krraze/CVE-2026-41575.svg) ![forks](https://img.shields.io/github/forks/krraze/CVE-2026-41575.svg)


## CVE-2026-2690
 A flaw has been found in itsourcecode Event Management System 1.0. Affected by this vulnerability is an unknown functionality of the file /admin/ajax.php?action=login of the component Admin Login. This manipulation of the argument Username causes sql injection. It is possible to initiate the attack remotely. The exploit has been published and may be used.

- [https://github.com/John-Jung/CVE-2026-26903-PoC](https://github.com/John-Jung/CVE-2026-26903-PoC) :  ![starts](https://img.shields.io/github/stars/John-Jung/CVE-2026-26903-PoC.svg) ![forks](https://img.shields.io/github/forks/John-Jung/CVE-2026-26903-PoC.svg)


## CVE-2026-1357
 The Migration, Backup, Staging – WPvivid Backup & Migration plugin for WordPress is vulnerable to Unauthenticated Arbitrary File Upload in versions up to and including 0.9.123. This is due to improper error handling in the RSA decryption process combined with a lack of path sanitization when writing uploaded files. When the plugin fails to decrypt a session key using openssl_private_decrypt(), it does not terminate execution and instead passes the boolean false value to the phpseclib library's AES cipher initialization. The library treats this false value as a string of null bytes, allowing an attacker to encrypt a malicious payload using a predictable null-byte key. Additionally, the plugin accepts filenames from the decrypted payload without sanitization, enabling directory traversal to escape the protected backup directory. This makes it possible for unauthenticated attackers to upload arbitrary PHP files to publicly accessible directories and achieve Remote Code Execution via the wpvivid_action=send_to_site parameter.

- [https://github.com/CVEs-Labs/CVE-2026-1357](https://github.com/CVEs-Labs/CVE-2026-1357) :  ![starts](https://img.shields.io/github/stars/CVEs-Labs/CVE-2026-1357.svg) ![forks](https://img.shields.io/github/forks/CVEs-Labs/CVE-2026-1357.svg)


## CVE-2026-0006
 In multiple locations, there is a possible out of bounds read and write due to a heap buffer overflow. This could lead to remote code execution with no additional execution privileges needed. User interaction is not needed for exploitation.

- [https://github.com/mobilehackinglab/CVE-2026-0006-openapv-poc](https://github.com/mobilehackinglab/CVE-2026-0006-openapv-poc) :  ![starts](https://img.shields.io/github/stars/mobilehackinglab/CVE-2026-0006-openapv-poc.svg) ![forks](https://img.shields.io/github/forks/mobilehackinglab/CVE-2026-0006-openapv-poc.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-55182
 A pre-authentication remote code execution vulnerability exists in React Server Components versions 19.0.0, 19.1.0, 19.1.1, and 19.2.0 including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints.

- [https://github.com/MuhammadWaseem29/React2Shell_Rce-cve-2025-55182](https://github.com/MuhammadWaseem29/React2Shell_Rce-cve-2025-55182) :  ![starts](https://img.shields.io/github/stars/MuhammadWaseem29/React2Shell_Rce-cve-2025-55182.svg) ![forks](https://img.shields.io/github/forks/MuhammadWaseem29/React2Shell_Rce-cve-2025-55182.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-24813
Users are recommended to upgrade to version 11.0.3, 10.1.35 or 9.0.99, which fixes the issue.

- [https://github.com/Enzo-Tssn/PCS3844-CVE_2025_24813](https://github.com/Enzo-Tssn/PCS3844-CVE_2025_24813) :  ![starts](https://img.shields.io/github/stars/Enzo-Tssn/PCS3844-CVE_2025_24813.svg) ![forks](https://img.shields.io/github/forks/Enzo-Tssn/PCS3844-CVE_2025_24813.svg)


## CVE-2025-7099
 A vulnerability has been found in BoyunCMS up to 1.21 on PHP7 and classified as critical. Affected by this vulnerability is an unknown functionality of the file install/install2.php of the component Installation Handler. The manipulation of the argument db_host leads to deserialization. The attack can be launched remotely. The complexity of an attack is rather high. The exploitation appears to be difficult. The exploit has been disclosed to the public and may be used.

- [https://github.com/ktauchathuranga/CVE-2025-70994](https://github.com/ktauchathuranga/CVE-2025-70994) :  ![starts](https://img.shields.io/github/stars/ktauchathuranga/CVE-2025-70994.svg) ![forks](https://img.shields.io/github/forks/ktauchathuranga/CVE-2025-70994.svg)


## CVE-2024-23897
 Jenkins 2.441 and earlier, LTS 2.426.2 and earlier does not disable a feature of its CLI command parser that replaces an '@' character followed by a file path in an argument with the file's contents, allowing unauthenticated attackers to read arbitrary files on the Jenkins controller file system.

- [https://github.com/w41l3r/jenkins_scan](https://github.com/w41l3r/jenkins_scan) :  ![starts](https://img.shields.io/github/stars/w41l3r/jenkins_scan.svg) ![forks](https://img.shields.io/github/forks/w41l3r/jenkins_scan.svg)


## CVE-2023-4863
 Heap buffer overflow in libwebp in Google Chrome prior to 116.0.5845.187 and libwebp 1.3.2 allowed a remote attacker to perform an out of bounds memory write via a crafted HTML page. (Chromium security severity: Critical)

- [https://github.com/jpselva/CVE-2023-4863](https://github.com/jpselva/CVE-2023-4863) :  ![starts](https://img.shields.io/github/stars/jpselva/CVE-2023-4863.svg) ![forks](https://img.shields.io/github/forks/jpselva/CVE-2023-4863.svg)


## CVE-2022-1026
 Kyocera multifunction printers running vulnerable versions of Net View unintentionally expose sensitive user information, including usernames and passwords, through an insufficiently protected address book export function.

- [https://github.com/D4RKMATT3R/KyoceraCredsDump](https://github.com/D4RKMATT3R/KyoceraCredsDump) :  ![starts](https://img.shields.io/github/stars/D4RKMATT3R/KyoceraCredsDump.svg) ![forks](https://img.shields.io/github/forks/D4RKMATT3R/KyoceraCredsDump.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/wolf1892/CVE-2021-41773](https://github.com/wolf1892/CVE-2021-41773) :  ![starts](https://img.shields.io/github/stars/wolf1892/CVE-2021-41773.svg) ![forks](https://img.shields.io/github/forks/wolf1892/CVE-2021-41773.svg)


## CVE-2020-13973
 OWASP json-sanitizer before 1.2.1 allows XSS. An attacker who controls a substring of the input JSON, and controls another substring adjacent to a SCRIPT element in which the output is embedded as JavaScript, may be able to confuse the HTML parser as to where the SCRIPT element ends, and cause non-script content to be interpreted as JavaScript.

- [https://github.com/epicosy/json-sanitizer](https://github.com/epicosy/json-sanitizer) :  ![starts](https://img.shields.io/github/stars/epicosy/json-sanitizer.svg) ![forks](https://img.shields.io/github/forks/epicosy/json-sanitizer.svg)
- [https://github.com/shoucheng3/OWASP__json-sanitizer_CVE-2020-13973_1-2-0](https://github.com/shoucheng3/OWASP__json-sanitizer_CVE-2020-13973_1-2-0) :  ![starts](https://img.shields.io/github/stars/shoucheng3/OWASP__json-sanitizer_CVE-2020-13973_1-2-0.svg) ![forks](https://img.shields.io/github/forks/shoucheng3/OWASP__json-sanitizer_CVE-2020-13973_1-2-0.svg)


## CVE-2020-13405
 userfiles/modules/users/controller/controller.php in Microweber before 1.1.20 allows an unauthenticated user to disclose the users database via a /modules/ POST request.

- [https://github.com/mrnazu/CVE-2020-13405](https://github.com/mrnazu/CVE-2020-13405) :  ![starts](https://img.shields.io/github/stars/mrnazu/CVE-2020-13405.svg) ![forks](https://img.shields.io/github/forks/mrnazu/CVE-2020-13405.svg)
- [https://github.com/Moniruzzaman995/CVE-2020-13405](https://github.com/Moniruzzaman995/CVE-2020-13405) :  ![starts](https://img.shields.io/github/stars/Moniruzzaman995/CVE-2020-13405.svg) ![forks](https://img.shields.io/github/forks/Moniruzzaman995/CVE-2020-13405.svg)


## CVE-2020-9376
 D-Link DIR-610 devices allow Information Disclosure via SERVICES=DEVICE.ACCOUNT%0AAUTHORIZED_GROUP=1 to getcfg.php. NOTE: This vulnerability only affects products that are no longer supported by the maintainer

- [https://github.com/renatoalencar/dlink-dir610-exploits](https://github.com/renatoalencar/dlink-dir610-exploits) :  ![starts](https://img.shields.io/github/stars/renatoalencar/dlink-dir610-exploits.svg) ![forks](https://img.shields.io/github/forks/renatoalencar/dlink-dir610-exploits.svg)


## CVE-2020-0796
 A remote code execution vulnerability exists in the way that the Microsoft Server Message Block 3.1.1 (SMBv3) protocol handles certain requests, aka 'Windows SMBv3 Client/Server Remote Code Execution Vulnerability'.

- [https://github.com/average-joe44/CVE-2020-0796-Forked-](https://github.com/average-joe44/CVE-2020-0796-Forked-) :  ![starts](https://img.shields.io/github/stars/average-joe44/CVE-2020-0796-Forked-.svg) ![forks](https://img.shields.io/github/forks/average-joe44/CVE-2020-0796-Forked-.svg)


## CVE-2018-6574
 Go before 1.8.7, Go 1.9.x before 1.9.4, and Go 1.10 pre-releases before Go 1.10rc2 allow "go get" remote command execution during source code build, by leveraging the gcc or clang plugin feature, because -fplugin= and -plugin= arguments were not blocked.

- [https://github.com/r00tpgp/CVE-2018-6574](https://github.com/r00tpgp/CVE-2018-6574) :  ![starts](https://img.shields.io/github/stars/r00tpgp/CVE-2018-6574.svg) ![forks](https://img.shields.io/github/forks/r00tpgp/CVE-2018-6574.svg)


## CVE-2018-6242
 Some NVIDIA Tegra mobile processors released prior to 2016 contain a buffer overflow vulnerability in BootROM Recovery Mode (RCM). An attacker with physical access to the device's USB and the ability to force the device to reboot into RCM could exploit the vulnerability to execute unverified code.

- [https://github.com/integerQuant/baitnswitch](https://github.com/integerQuant/baitnswitch) :  ![starts](https://img.shields.io/github/stars/integerQuant/baitnswitch.svg) ![forks](https://img.shields.io/github/forks/integerQuant/baitnswitch.svg)


## CVE-2017-11783
 Microsoft Windows 8.1, Windows Server 2012 R2, Windows RT 8.1, Windows 10 Gold, 1511, 1607, and 1703, and Windows Server 2016 allows an elevation of privilege vulnerability in the way it handles calls to Advanced Local Procedure Call (ALPC), aka "Windows Elevation of Privilege Vulnerability".

- [https://github.com/Sheisback/CVE-2017-11783](https://github.com/Sheisback/CVE-2017-11783) :  ![starts](https://img.shields.io/github/stars/Sheisback/CVE-2017-11783.svg) ![forks](https://img.shields.io/github/forks/Sheisback/CVE-2017-11783.svg)

