# Update 2026-03-30
## CVE-2026-33937
 Handlebars provides the power necessary to let users build semantic templates. In versions 4.0.0 through 4.7.8, `Handlebars.compile()` accepts a pre-parsed AST object in addition to a template string. The `value` field of a `NumberLiteral` AST node is emitted directly into the generated JavaScript without quoting or sanitization. An attacker who can supply a crafted AST to `compile()` can therefore inject and execute arbitrary JavaScript, leading to Remote Code Execution on the server. Version 4.7.9 fixes the issue. Some workarounds are available. Validate input type before calling `Handlebars.compile()`; ensure the argument is always a  `string`, never a plain object or JSON-deserialized value. Use the Handlebars runtime-only build (`handlebars/runtime`) on the server if templates are pre-compiled at build time; `compile()` will be unavailable.

- [https://github.com/dinhvaren/cve-2026-33937](https://github.com/dinhvaren/cve-2026-33937) :  ![starts](https://img.shields.io/github/stars/dinhvaren/cve-2026-33937.svg) ![forks](https://img.shields.io/github/forks/dinhvaren/cve-2026-33937.svg)


## CVE-2026-31802
 node-tar is a full-featured Tar for Node.js. Prior to version 7.5.11, tar (npm) can be tricked into creating a symlink that points outside the extraction directory by using a drive-relative symlink target such as C:../../../target.txt, which enables file overwrite outside cwd during normal tar.x() extraction. This vulnerability is fixed in 7.5.11.

- [https://github.com/Recorded-texteditor120/CVE-2026-31802](https://github.com/Recorded-texteditor120/CVE-2026-31802) :  ![starts](https://img.shields.io/github/stars/Recorded-texteditor120/CVE-2026-31802.svg) ![forks](https://img.shields.io/github/forks/Recorded-texteditor120/CVE-2026-31802.svg)


## CVE-2026-28466
 OpenClaw versions prior to 2026.2.14 contain a vulnerability in the gateway in which it fails to sanitize internal approval fields in node.invoke parameters, allowing authenticated clients to bypass exec approval gating for system.run commands. Attackers with valid gateway credentials can inject approval control fields to execute arbitrary commands on connected node hosts, potentially compromising developer workstations and CI runners.

- [https://github.com/Orioning/CVE-2026-28466](https://github.com/Orioning/CVE-2026-28466) :  ![starts](https://img.shields.io/github/stars/Orioning/CVE-2026-28466.svg) ![forks](https://img.shields.io/github/forks/Orioning/CVE-2026-28466.svg)


## CVE-2026-25099
This issue was fixed in 3.18.4.

- [https://github.com/yahiahamza/CVE-2026-25099](https://github.com/yahiahamza/CVE-2026-25099) :  ![starts](https://img.shields.io/github/stars/yahiahamza/CVE-2026-25099.svg) ![forks](https://img.shields.io/github/forks/yahiahamza/CVE-2026-25099.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/d3vn0mi/CVE-2026-23744-POC](https://github.com/d3vn0mi/CVE-2026-23744-POC) :  ![starts](https://img.shields.io/github/stars/d3vn0mi/CVE-2026-23744-POC.svg) ![forks](https://img.shields.io/github/forks/d3vn0mi/CVE-2026-23744-POC.svg)
- [https://github.com/d0x-awrqxavc/CVE-2026-23744-HACKTHEBOX](https://github.com/d0x-awrqxavc/CVE-2026-23744-HACKTHEBOX) :  ![starts](https://img.shields.io/github/stars/d0x-awrqxavc/CVE-2026-23744-HACKTHEBOX.svg) ![forks](https://img.shields.io/github/forks/d0x-awrqxavc/CVE-2026-23744-HACKTHEBOX.svg)


## CVE-2026-21643
 An improper neutralization of special elements used in an sql command ('sql injection') vulnerability in Fortinet FortiClientEMS 7.4.4 may allow an unauthenticated attacker to execute unauthorized code or commands via specifically crafted HTTP requests.

- [https://github.com/0xBlackash/CVE-2026-21643](https://github.com/0xBlackash/CVE-2026-21643) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-21643.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-21643.svg)


## CVE-2026-20079
 This vulnerability is due to an improper system process that is created at boot time. An attacker could exploit this vulnerability by sending crafted HTTP requests to an affected device. A successful exploit could allow the attacker to execute a variety of scripts and commands that allow root access to the device.

- [https://github.com/0xBlackash/CVE-2026-20079](https://github.com/0xBlackash/CVE-2026-20079) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-20079.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-20079.svg)


## CVE-2026-5000
 A vulnerability was detected in PromtEngineer localGPT up to 4d41c7d1713b16b216d8e062e51a5dd88b20b054. Impacted is the function LocalGPTHandler of the file backend/server.py of the component API Endpoint. The manipulation of the argument BaseHTTPRequestHandler results in missing authentication. The attack can be executed remotely. This product implements a rolling release for ongoing delivery, which means version information for affected or updated releases is unavailable. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/Perl-Code/CVE-2026-5000](https://github.com/Perl-Code/CVE-2026-5000) :  ![starts](https://img.shields.io/github/stars/Perl-Code/CVE-2026-5000.svg) ![forks](https://img.shields.io/github/forks/Perl-Code/CVE-2026-5000.svg)


## CVE-2026-1657
 The EventPrime plugin for WordPress is vulnerable to unauthorized image file upload in all versions up to, and including, 4.2.8.4. This is due to the plugin registering the upload_file_media AJAX action as publicly accessible (nopriv-enabled) without implementing any authentication, authorization, or nonce verification despite a nonce being created. This makes it possible for unauthenticated attackers to upload image files to the WordPress uploads directory and create Media Library attachments via the ep_upload_file_media endpoint.

- [https://github.com/Vimash-Dilsara/-CVE-2026-1657](https://github.com/Vimash-Dilsara/-CVE-2026-1657) :  ![starts](https://img.shields.io/github/stars/Vimash-Dilsara/-CVE-2026-1657.svg) ![forks](https://img.shields.io/github/forks/Vimash-Dilsara/-CVE-2026-1657.svg)


## CVE-2026-0766
The specific flaw exists within the load_tool_module_by_id function. The issue results from the lack of proper validation of a user-supplied string before using it to execute Python code. An attacker can leverage this vulnerability to execute code in the context of the service account. Was ZDI-CAN-28257.

- [https://github.com/bitt0n/CVE-2026-0766](https://github.com/bitt0n/CVE-2026-0766) :  ![starts](https://img.shields.io/github/stars/bitt0n/CVE-2026-0766.svg) ![forks](https://img.shields.io/github/forks/bitt0n/CVE-2026-0766.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-66034
 fontTools is a library for manipulating fonts, written in Python. In versions from 4.33.0 to before 4.60.2, the fonttools varLib (or python3 -m fontTools.varLib) script has an arbitrary file write vulnerability that leads to remote code execution when a malicious .designspace file is processed. The vulnerability affects the main() code path of fontTools.varLib, used by the fonttools varLib CLI and any code that invokes fontTools.varLib.main(). This issue has been patched in version 4.60.2.

- [https://github.com/4nuxd/CVE-2025-66034](https://github.com/4nuxd/CVE-2025-66034) :  ![starts](https://img.shields.io/github/stars/4nuxd/CVE-2025-66034.svg) ![forks](https://img.shields.io/github/forks/4nuxd/CVE-2025-66034.svg)


## CVE-2025-54123
 Hoverfly is an open source API simulation tool. In versions 1.11.3 and prior, the middleware functionality in Hoverfly is vulnerable to command injection vulnerability at `/api/v2/hoverfly/middleware` endpoint due to insufficient validation and sanitization in user input. The vulnerability exists in the middleware management API endpoint `/api/v2/hoverfly/middleware`. This issue is born due to combination of three code level flaws: Insufficient Input Validation in middleware.go line 94-96; Unsafe Command Execution in local_middleware.go line 14-19; and Immediate Execution During Testing in hoverfly_service.go line 173. This allows an attacker to gain remote code execution (RCE) on any system running the vulnerable Hoverfly service. Since the input is directly passed to system commands without proper checks, an attacker can upload a malicious payload or directly execute arbitrary commands (including reverse shells) on the host server with the privileges of the Hoverfly process. Commit 17e60a9bc78826deb4b782dca1c1abd3dbe60d40 in version 1.12.0 disables the set middleware API by default, and subsequent changes to documentation make users aware of the security changes of exposing the set middleware API.

- [https://github.com/kasem545/CVE-2025-54123-Poc](https://github.com/kasem545/CVE-2025-54123-Poc) :  ![starts](https://img.shields.io/github/stars/kasem545/CVE-2025-54123-Poc.svg) ![forks](https://img.shields.io/github/forks/kasem545/CVE-2025-54123-Poc.svg)
- [https://github.com/0xzap/CVE-2025-54123](https://github.com/0xzap/CVE-2025-54123) :  ![starts](https://img.shields.io/github/stars/0xzap/CVE-2025-54123.svg) ![forks](https://img.shields.io/github/forks/0xzap/CVE-2025-54123.svg)


## CVE-2025-47181
 Improper link resolution before file access ('link following') in Microsoft Edge (Chromium-based) allows an authorized attacker to elevate privileges locally.

- [https://github.com/d3vn0mi/CVE-2025-471812-POC](https://github.com/d3vn0mi/CVE-2025-471812-POC) :  ![starts](https://img.shields.io/github/stars/d3vn0mi/CVE-2025-471812-POC.svg) ![forks](https://img.shields.io/github/forks/d3vn0mi/CVE-2025-471812-POC.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/MKIRAHMET/CVE-2025-29927-PoC](https://github.com/MKIRAHMET/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/MKIRAHMET/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/MKIRAHMET/CVE-2025-29927-PoC.svg)


## CVE-2025-4138
Note that none of these vulnerabilities significantly affect the installation of source distributions which are tar archives as source distributions already allow arbitrary code execution during the build process. However when evaluating source distributions it's important to avoid installing source distributions with suspicious links.

- [https://github.com/d3vn0mi/CVE-2025-4138-POC](https://github.com/d3vn0mi/CVE-2025-4138-POC) :  ![starts](https://img.shields.io/github/stars/d3vn0mi/CVE-2025-4138-POC.svg) ![forks](https://img.shields.io/github/forks/d3vn0mi/CVE-2025-4138-POC.svg)


## CVE-2025-2304
When a user wishes to change his password, the 'updated_ajax' method of the UsersController is called. The vulnerability stems from the use of the dangerous permit! method, which allows all parameters to pass through without any filtering.

- [https://github.com/d3vn0mi/CVE-2025-2304-POC](https://github.com/d3vn0mi/CVE-2025-2304-POC) :  ![starts](https://img.shields.io/github/stars/d3vn0mi/CVE-2025-2304-POC.svg) ![forks](https://img.shields.io/github/forks/d3vn0mi/CVE-2025-2304-POC.svg)


## CVE-2023-43208
 NextGen Healthcare Mirth Connect before version 4.4.1 is vulnerable to unauthenticated remote code execution. Note that this vulnerability is caused by the incomplete patch of CVE-2023-37679.

- [https://github.com/Humberto-pixel/CVE-2023-43208-PoC](https://github.com/Humberto-pixel/CVE-2023-43208-PoC) :  ![starts](https://img.shields.io/github/stars/Humberto-pixel/CVE-2023-43208-PoC.svg) ![forks](https://img.shields.io/github/forks/Humberto-pixel/CVE-2023-43208-PoC.svg)


## CVE-2022-46364
 A SSRF vulnerability in parsing the href attribute of XOP:Include in MTOM requests in versions of Apache CXF before 3.5.5 and 3.4.10 allows an attacker to perform SSRF style attacks on webservices that take at least one parameter of any type. 

- [https://github.com/kasem545/CVE-2022-46364-Poc](https://github.com/kasem545/CVE-2022-46364-Poc) :  ![starts](https://img.shields.io/github/stars/kasem545/CVE-2022-46364-Poc.svg) ![forks](https://img.shields.io/github/forks/kasem545/CVE-2022-46364-Poc.svg)
- [https://github.com/cybermaksxx/CVE-2022-46364-Proof-of-the-concept](https://github.com/cybermaksxx/CVE-2022-46364-Proof-of-the-concept) :  ![starts](https://img.shields.io/github/stars/cybermaksxx/CVE-2022-46364-Proof-of-the-concept.svg) ![forks](https://img.shields.io/github/forks/cybermaksxx/CVE-2022-46364-Proof-of-the-concept.svg)
- [https://github.com/Shashivanth009/CVE-2022-46364---Apache-CXF-XOP-Include-LFI-PoC](https://github.com/Shashivanth009/CVE-2022-46364---Apache-CXF-XOP-Include-LFI-PoC) :  ![starts](https://img.shields.io/github/stars/Shashivanth009/CVE-2022-46364---Apache-CXF-XOP-Include-LFI-PoC.svg) ![forks](https://img.shields.io/github/forks/Shashivanth009/CVE-2022-46364---Apache-CXF-XOP-Include-LFI-PoC.svg)


## CVE-2022-25927
 Versions of the package ua-parser-js from 0.7.30 and before 0.7.33, from 0.8.1 and before 1.0.33 are vulnerable to Regular Expression Denial of Service (ReDoS) via the trim() function.

- [https://github.com/Sleuth-in-town/CVE-2022-25927-test](https://github.com/Sleuth-in-town/CVE-2022-25927-test) :  ![starts](https://img.shields.io/github/stars/Sleuth-in-town/CVE-2022-25927-test.svg) ![forks](https://img.shields.io/github/forks/Sleuth-in-town/CVE-2022-25927-test.svg)


## CVE-2021-33045
 The identity authentication bypass vulnerability found in some Dahua products during the login process. Attackers can bypass device identity authentication by constructing malicious data packets.

- [https://github.com/Bd-Mutant7/DahuaLoginBypass](https://github.com/Bd-Mutant7/DahuaLoginBypass) :  ![starts](https://img.shields.io/github/stars/Bd-Mutant7/DahuaLoginBypass.svg) ![forks](https://img.shields.io/github/forks/Bd-Mutant7/DahuaLoginBypass.svg)


## CVE-2021-33044
 The identity authentication bypass vulnerability found in some Dahua products during the login process. Attackers can bypass device identity authentication by constructing malicious data packets.

- [https://github.com/Bd-Mutant7/DahuaLoginBypass](https://github.com/Bd-Mutant7/DahuaLoginBypass) :  ![starts](https://img.shields.io/github/stars/Bd-Mutant7/DahuaLoginBypass.svg) ![forks](https://img.shields.io/github/forks/Bd-Mutant7/DahuaLoginBypass.svg)


## CVE-2021-23369
 The package handlebars before 4.7.7 are vulnerable to Remote Code Execution (RCE) when selecting certain compiling options to compile templates coming from an untrusted source.

- [https://github.com/dinhvaren/cve-2021-23369](https://github.com/dinhvaren/cve-2021-23369) :  ![starts](https://img.shields.io/github/stars/dinhvaren/cve-2021-23369.svg) ![forks](https://img.shields.io/github/forks/dinhvaren/cve-2021-23369.svg)

