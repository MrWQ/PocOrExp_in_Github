# Update 2026-04-14
## CVE-2026-40175
 Axios is a promise based HTTP client for the browser and Node.js. Prior to 1.15.0, the Axios library is vulnerable to a specific "Gadget" attack chain that allows Prototype Pollution in any third-party dependency to be escalated into Remote Code Execution (RCE) or Full Cloud Compromise (via AWS IMDSv2 bypass). This vulnerability is fixed in 1.15.0.

- [https://github.com/0xBlackash/CVE-2026-40175](https://github.com/0xBlackash/CVE-2026-40175) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-40175.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-40175.svg)


## CVE-2026-39987
 marimo is a reactive Python notebook. Prior to 0.23.0, Marimo has a Pre-Auth RCE vulnerability. The terminal WebSocket endpoint /terminal/ws lacks authentication validation, allowing an unauthenticated attacker to obtain a full PTY shell and execute arbitrary system commands. Unlike other WebSocket endpoints (e.g., /ws) that correctly call validate_auth() for authentication, the /terminal/ws endpoint only checks the running mode and platform support before accepting connections, completely skipping authentication verification. This vulnerability is fixed in 0.23.0.

- [https://github.com/0xBlackash/CVE-2026-39987](https://github.com/0xBlackash/CVE-2026-39987) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-39987.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-39987.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/oscar-mine/CVE-2026-33017-Exploit](https://github.com/oscar-mine/CVE-2026-33017-Exploit) :  ![starts](https://img.shields.io/github/stars/oscar-mine/CVE-2026-33017-Exploit.svg) ![forks](https://img.shields.io/github/forks/oscar-mine/CVE-2026-33017-Exploit.svg)


## CVE-2026-31413
dst = 0 and naturally computes the correct result for any opcode.

- [https://github.com/Rat5ak/CVE-2026-31413-BPF-Container-Escape](https://github.com/Rat5ak/CVE-2026-31413-BPF-Container-Escape) :  ![starts](https://img.shields.io/github/stars/Rat5ak/CVE-2026-31413-BPF-Container-Escape.svg) ![forks](https://img.shields.io/github/forks/Rat5ak/CVE-2026-31413-BPF-Container-Escape.svg)


## CVE-2026-29145
Users are recommended to upgrade to version Tomcat Native 1.3.7 or 2.0.14 and Tomcat 11.0.20, 10.1.53 and 9.0.116, which fix the issue.

- [https://github.com/gregk4sec/cve-2026-29145](https://github.com/gregk4sec/cve-2026-29145) :  ![starts](https://img.shields.io/github/stars/gregk4sec/cve-2026-29145.svg) ![forks](https://img.shields.io/github/forks/gregk4sec/cve-2026-29145.svg)


## CVE-2026-25854
Users are recommended to upgrade to version 11.0.20, 10.1.53 or 9.0.116, which fix the issue.

- [https://github.com/gregk4sec/cve-2026-25854](https://github.com/gregk4sec/cve-2026-25854) :  ![starts](https://img.shields.io/github/stars/gregk4sec/cve-2026-25854.svg) ![forks](https://img.shields.io/github/forks/gregk4sec/cve-2026-25854.svg)


## CVE-2026-23980
Users are recommended to upgrade to version 6.0.0, which fixes the issue.

- [https://github.com/oscar-mine/CVE-2026-23980-Exploit](https://github.com/oscar-mine/CVE-2026-23980-Exploit) :  ![starts](https://img.shields.io/github/stars/oscar-mine/CVE-2026-23980-Exploit.svg) ![forks](https://img.shields.io/github/forks/oscar-mine/CVE-2026-23980-Exploit.svg)


## CVE-2026-23520
 Arcane provides modern docker management. Prior to 1.13.0, Arcane has a command injection in the updater service. Arcane’s updater service supported lifecycle labels com.getarcaneapp.arcane.lifecycle.pre-update and com.getarcaneapp.arcane.lifecycle.post-update that allowed defining a command to run before or after a container update. The label value is passed directly to /bin/sh -c without sanitization or validation. Because any authenticated user (not limited to administrators) can create projects through the API, an attacker can create a project that specifies one of these lifecycle labels with a malicious command. When an administrator later triggers a container update (either manually or via scheduled update checks), Arcane reads the lifecycle label and executes its value as a shell command inside the container. This vulnerability is fixed in 1.13.0.

- [https://github.com/secopssite/HTB](https://github.com/secopssite/HTB) :  ![starts](https://img.shields.io/github/stars/secopssite/HTB.svg) ![forks](https://img.shields.io/github/forks/secopssite/HTB.svg)


## CVE-2026-6111
 A security flaw has been discovered in FoundationAgents MetaGPT up to 0.8.1. This impacts the function decode_image of the file metagpt/utils/common.py. The manipulation of the argument img_url_or_b64 results in server-side request forgery. It is possible to launch the attack remotely. The exploit has been released to the public and may be used for attacks. The project was informed of the problem early through an issue report but has not responded yet.

- [https://github.com/MonsterWsr-hub/CVE-2026-6111](https://github.com/MonsterWsr-hub/CVE-2026-6111) :  ![starts](https://img.shields.io/github/stars/MonsterWsr-hub/CVE-2026-6111.svg) ![forks](https://img.shields.io/github/forks/MonsterWsr-hub/CVE-2026-6111.svg)


## CVE-2026-3909
 Out of bounds write in Skia in Google Chrome prior to 146.0.7680.75 allowed a remote attacker to perform out of bounds memory access via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/anansi2safe/CVE-2026-3909-PoC](https://github.com/anansi2safe/CVE-2026-3909-PoC) :  ![starts](https://img.shields.io/github/stars/anansi2safe/CVE-2026-3909-PoC.svg) ![forks](https://img.shields.io/github/forks/anansi2safe/CVE-2026-3909-PoC.svg)


## CVE-2026-3805
a data pointer pointing into already freed memory.

- [https://github.com/Rat5ak/CVE-2026-3805-curl-SMB-UAF](https://github.com/Rat5ak/CVE-2026-3805-curl-SMB-UAF) :  ![starts](https://img.shields.io/github/stars/Rat5ak/CVE-2026-3805-curl-SMB-UAF.svg) ![forks](https://img.shields.io/github/forks/Rat5ak/CVE-2026-3805-curl-SMB-UAF.svg)


## CVE-2025-67246
 A local information disclosure vulnerability exists in the Ludashi driver before 5.1025 due to a lack of access control in the IOCTL handler. This driver exposes a device interface accessible to a normal user and handles attacker-controlled structures containing the lower 4GB of physical addresses. The handler maps arbitrary physical memory via MmMapIoSpace and copies data back to user mode without verifying the caller's privileges or the target address range. This allows unprivileged users to read arbitrary physical memory, potentially exposing kernel data structures, kernel pointers, security tokens, and other sensitive information. This vulnerability can be further exploited to bypass the Kernel Address Space Layout Rules (KASLR) and achieve local privilege escalation.

- [https://github.com/CDipper/CVE-2025-67246](https://github.com/CDipper/CVE-2025-67246) :  ![starts](https://img.shields.io/github/stars/CDipper/CVE-2025-67246.svg) ![forks](https://img.shields.io/github/forks/CDipper/CVE-2025-67246.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg)


## CVE-2025-66034
 fontTools is a library for manipulating fonts, written in Python. In versions from 4.33.0 to before 4.60.2, the fonttools varLib (or python3 -m fontTools.varLib) script has an arbitrary file write vulnerability that leads to remote code execution when a malicious .designspace file is processed. The vulnerability affects the main() code path of fontTools.varLib, used by the fonttools varLib CLI and any code that invokes fontTools.varLib.main(). This issue has been patched in version 4.60.2.

- [https://github.com/secopssite/HTB](https://github.com/secopssite/HTB) :  ![starts](https://img.shields.io/github/stars/secopssite/HTB.svg) ![forks](https://img.shields.io/github/forks/secopssite/HTB.svg)


## CVE-2025-59719
 An improper verification of cryptographic signature vulnerability in Fortinet FortiWeb 8.0.0, FortiWeb 7.6.0 through 7.6.4, FortiWeb 7.4.0 through 7.4.9 may allow an unauthenticated attacker to bypass the FortiCloud SSO login authentication via a crafted SAML response message.

- [https://github.com/moften/CVE-2025-59718-Fortinet-Poc](https://github.com/moften/CVE-2025-59718-Fortinet-Poc) :  ![starts](https://img.shields.io/github/stars/moften/CVE-2025-59718-Fortinet-Poc.svg) ![forks](https://img.shields.io/github/forks/moften/CVE-2025-59718-Fortinet-Poc.svg)


## CVE-2025-59528
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5, Flowise is vulnerable to remote code execution. The CustomMCP node allows users to input configuration settings for connecting to an external MCP server. This node parses the user-provided mcpServerConfig string to build the MCP server configuration. However, during this process, it executes JavaScript code without any security validation. Specifically, inside the convertToValidJSONString function, user input is directly passed to the Function() constructor, which evaluates and executes the input as JavaScript code. Since this runs with full Node.js runtime privileges, it can access dangerous modules such as child_process and fs. This issue has been patched in version 3.0.6.

- [https://github.com/secopssite/HTB](https://github.com/secopssite/HTB) :  ![starts](https://img.shields.io/github/stars/secopssite/HTB.svg) ![forks](https://img.shields.io/github/forks/secopssite/HTB.svg)
- [https://github.com/TYehan/CVE-2025-58434-59528](https://github.com/TYehan/CVE-2025-58434-59528) :  ![starts](https://img.shields.io/github/stars/TYehan/CVE-2025-58434-59528.svg) ![forks](https://img.shields.io/github/forks/TYehan/CVE-2025-58434-59528.svg)


## CVE-2025-58434
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5 and earlier, the `forgot-password` endpoint in Flowise returns sensitive information including a valid password reset `tempToken` without authentication or verification. This enables any attacker to generate a reset token for arbitrary users and directly reset their password, leading to a complete account takeover (ATO). This vulnerability applies to both the cloud service (`cloud.flowiseai.com`) and self-hosted/local Flowise deployments that expose the same API. Commit 9e178d68873eb876073846433a596590d3d9c863 in version 3.0.6 secures password reset endpoints. Several recommended remediation steps are available. Do not return reset tokens or sensitive account details in API responses. Tokens must only be delivered securely via the registered email channel. Ensure `forgot-password` responds with a generic success message regardless of input, to avoid user enumeration. Require strong validation of the `tempToken` (e.g., single-use, short expiry, tied to request origin, validated against email delivery). Apply the same fixes to both cloud and self-hosted/local deployments. Log and monitor password reset requests for suspicious activity. Consider multi-factor verification for sensitive accounts.

- [https://github.com/TYehan/CVE-2025-58434-59528](https://github.com/TYehan/CVE-2025-58434-59528) :  ![starts](https://img.shields.io/github/stars/TYehan/CVE-2025-58434-59528.svg) ![forks](https://img.shields.io/github/forks/TYehan/CVE-2025-58434-59528.svg)
- [https://github.com/kartik2005221/CVE-2025-58434-poc](https://github.com/kartik2005221/CVE-2025-58434-poc) :  ![starts](https://img.shields.io/github/stars/kartik2005221/CVE-2025-58434-poc.svg) ![forks](https://img.shields.io/github/forks/kartik2005221/CVE-2025-58434-poc.svg)
- [https://github.com/p1ctur3p3rf3ct/CVE-2025-58434](https://github.com/p1ctur3p3rf3ct/CVE-2025-58434) :  ![starts](https://img.shields.io/github/stars/p1ctur3p3rf3ct/CVE-2025-58434.svg) ![forks](https://img.shields.io/github/forks/p1ctur3p3rf3ct/CVE-2025-58434.svg)
- [https://github.com/kartik2005221/CVE-2025-58434-AND-59528-POC](https://github.com/kartik2005221/CVE-2025-58434-AND-59528-POC) :  ![starts](https://img.shields.io/github/stars/kartik2005221/CVE-2025-58434-AND-59528-POC.svg) ![forks](https://img.shields.io/github/forks/kartik2005221/CVE-2025-58434-AND-59528-POC.svg)
- [https://github.com/jwsly12/CVE-2025-58434-59528-htb-ctf](https://github.com/jwsly12/CVE-2025-58434-59528-htb-ctf) :  ![starts](https://img.shields.io/github/stars/jwsly12/CVE-2025-58434-59528-htb-ctf.svg) ![forks](https://img.shields.io/github/forks/jwsly12/CVE-2025-58434-59528-htb-ctf.svg)


## CVE-2025-54068
 Livewire is a full-stack framework for Laravel. In Livewire v3 up to and including v3.6.3, a vulnerability allows unauthenticated attackers to achieve remote command execution in specific scenarios. The issue stems from how certain component property updates are hydrated. This vulnerability is unique to Livewire v3 and does not affect prior major versions. Exploitation requires a component to be mounted and configured in a particular way, but does not require authentication or user interaction. This issue has been patched in Livewire v3.6.4. All users are strongly encouraged to upgrade to this version or later as soon as possible. No known workarounds are available.

- [https://github.com/HelgeSverre/livewire-honeypot](https://github.com/HelgeSverre/livewire-honeypot) :  ![starts](https://img.shields.io/github/stars/HelgeSverre/livewire-honeypot.svg) ![forks](https://img.shields.io/github/forks/HelgeSverre/livewire-honeypot.svg)


## CVE-2025-34065
 An authentication bypass vulnerability exists in AVTECH IP camera, DVR, and NVR devices’ streamd web server. The strstr() function allows unauthenticated access to any request containing "/nobody" in the URL, bypassing login controls.

- [https://github.com/Savanooo/avtech-cve-2025-34065-analysis](https://github.com/Savanooo/avtech-cve-2025-34065-analysis) :  ![starts](https://img.shields.io/github/stars/Savanooo/avtech-cve-2025-34065-analysis.svg) ![forks](https://img.shields.io/github/forks/Savanooo/avtech-cve-2025-34065-analysis.svg)


## CVE-2025-32429
 XWiki Platform is a generic wiki platform offering runtime services for applications built on top of it. In versions 9.4-rc-1 through 16.10.5 and 17.0.0-rc-1 through 17.2.2, it's possible for anyone to inject SQL using the parameter sort of the getdeleteddocuments.vm. It's injected as is as an ORDER BY value. This is fixed in versions 16.10.6 and 17.3.0-rc-1.

- [https://github.com/TheNaderr/CVE-2025-32429](https://github.com/TheNaderr/CVE-2025-32429) :  ![starts](https://img.shields.io/github/stars/TheNaderr/CVE-2025-32429.svg) ![forks](https://img.shields.io/github/forks/TheNaderr/CVE-2025-32429.svg)


## CVE-2025-14894
 Livewire Filemanager, commonly used in Laravel applications, contains LivewireFilemanagerComponent.php, which does not perform file type and MIME validation, allowing for RCE through upload of a malicious php file that can then be executed via the /storage/ URL if a commonly performed setup process within Laravel applications has been completed.

- [https://github.com/HelgeSverre/livewire-honeypot](https://github.com/HelgeSverre/livewire-honeypot) :  ![starts](https://img.shields.io/github/stars/HelgeSverre/livewire-honeypot.svg) ![forks](https://img.shields.io/github/forks/HelgeSverre/livewire-honeypot.svg)


## CVE-2025-8110
 Improper Symbolic link handling in the PutContents API in Gogs allows Local Execution of Code.

- [https://github.com/secopssite/HTB](https://github.com/secopssite/HTB) :  ![starts](https://img.shields.io/github/stars/secopssite/HTB.svg) ![forks](https://img.shields.io/github/forks/secopssite/HTB.svg)
- [https://github.com/TYehan/CVE-2025-8110-Gogs-RCE-Exploit](https://github.com/TYehan/CVE-2025-8110-Gogs-RCE-Exploit) :  ![starts](https://img.shields.io/github/stars/TYehan/CVE-2025-8110-Gogs-RCE-Exploit.svg) ![forks](https://img.shields.io/github/forks/TYehan/CVE-2025-8110-Gogs-RCE-Exploit.svg)
- [https://github.com/0dgt/CVE-2025-8110](https://github.com/0dgt/CVE-2025-8110) :  ![starts](https://img.shields.io/github/stars/0dgt/CVE-2025-8110.svg) ![forks](https://img.shields.io/github/forks/0dgt/CVE-2025-8110.svg)
- [https://github.com/manbahadurthapa1248/CVE-2025-8110-Authenticated-Remote-Code-Execution-on-Gogs-v0.13.3-](https://github.com/manbahadurthapa1248/CVE-2025-8110-Authenticated-Remote-Code-Execution-on-Gogs-v0.13.3-) :  ![starts](https://img.shields.io/github/stars/manbahadurthapa1248/CVE-2025-8110-Authenticated-Remote-Code-Execution-on-Gogs-v0.13.3-.svg) ![forks](https://img.shields.io/github/forks/manbahadurthapa1248/CVE-2025-8110-Authenticated-Remote-Code-Execution-on-Gogs-v0.13.3-.svg)


## CVE-2025-4720
 A vulnerability was found in SourceCodester Student Result Management System 1.0. It has been declared as critical. This vulnerability affects unknown code of the file academic/core/drop_student.php. The manipulation of the argument img leads to path traversal. The attack can be initiated remotely. The exploit has been disclosed to the public and may be used.

- [https://github.com/Xmyronn/duplicate-CVE-2025-4720-](https://github.com/Xmyronn/duplicate-CVE-2025-4720-) :  ![starts](https://img.shields.io/github/stars/Xmyronn/duplicate-CVE-2025-4720-.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/duplicate-CVE-2025-4720-.svg)


## CVE-2025-2945
This issue affects pgAdmin 4: before 9.2.

- [https://github.com/secopssite/HTB](https://github.com/secopssite/HTB) :  ![starts](https://img.shields.io/github/stars/secopssite/HTB.svg) ![forks](https://img.shields.io/github/forks/secopssite/HTB.svg)


## CVE-2024-47823
 Livewire is a full-stack framework for Laravel that allows for dynamic UI components without leaving PHP. In livewire/livewire prior to `2.12.7` and `v3.5.2`, the file extension of an uploaded file is guessed based on the MIME type. As a result, the actual file extension from the file name is not validated. An attacker can therefore bypass the validation by uploading a file with a valid MIME type (e.g., `image/png`) and a “.php” file extension. If the following criteria are met, the attacker can carry out an RCE attack: 1. Filename is composed of the original file name using `$file-getClientOriginalName()`. 2. Files stored directly on your server in a public storage disk. 3. Webserver is configured to execute “.php” files. This issue has been addressed in release versions `2.12.7` and `3.5.2`. All users are advised to upgrade. There are no known workarounds for this vulnerability.

- [https://github.com/HelgeSverre/livewire-honeypot](https://github.com/HelgeSverre/livewire-honeypot) :  ![starts](https://img.shields.io/github/stars/HelgeSverre/livewire-honeypot.svg) ![forks](https://img.shields.io/github/forks/HelgeSverre/livewire-honeypot.svg)


## CVE-2024-34351
 Next.js is a React framework that can provide building blocks to create web applications. A Server-Side Request Forgery (SSRF) vulnerability was identified in Next.js Server Actions. If the `Host` header is modified, and the below conditions are also met, an attacker may be able to make requests that appear to be originating from the Next.js application server itself. The required conditions are 1) Next.js is running in a self-hosted manner; 2) the Next.js application makes use of Server Actions; and 3) the Server Action performs a redirect to a relative path which starts with a `/`. This vulnerability was fixed in Next.js `14.1.1`.

- [https://github.com/Jinlei-Chen-UWO/cve-2024-34351-demo](https://github.com/Jinlei-Chen-UWO/cve-2024-34351-demo) :  ![starts](https://img.shields.io/github/stars/Jinlei-Chen-UWO/cve-2024-34351-demo.svg) ![forks](https://img.shields.io/github/forks/Jinlei-Chen-UWO/cve-2024-34351-demo.svg)


## CVE-2024-25082
 Splinefont in FontForge through 20230101 allows command injection via crafted archives or compressed files.

- [https://github.com/secopssite/HTB](https://github.com/secopssite/HTB) :  ![starts](https://img.shields.io/github/stars/secopssite/HTB.svg) ![forks](https://img.shields.io/github/forks/secopssite/HTB.svg)


## CVE-2024-23828
 Nginx-UI is a web interface to manage Nginx configurations. It is vulnerable to an authenticated arbitrary command execution via CRLF attack when changing the value of test_config_cmd or start_cmd. This vulnerability exists due to an incomplete fix for CVE-2024-22197 and CVE-2024-22198. This vulnerability has been patched in version 2.0.0.beta.12.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2024-4367
 A type check was missing when handling fonts in PDF.js, which would allow arbitrary JavaScript execution in the PDF.js context. This vulnerability affects Firefox  126, Firefox ESR  115.11, and Thunderbird  115.11.

- [https://github.com/John-Popovici/CVE-2022-0543-redis-sandbox-escape](https://github.com/John-Popovici/CVE-2022-0543-redis-sandbox-escape) :  ![starts](https://img.shields.io/github/stars/John-Popovici/CVE-2022-0543-redis-sandbox-escape.svg) ![forks](https://img.shields.io/github/forks/John-Popovici/CVE-2022-0543-redis-sandbox-escape.svg)


## CVE-2023-48251
 The vulnerability allows a remote attacker to authenticate to the SSH service with root privileges through a hidden hard-coded account.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2023-38941
 django-sspanel v2022.2.2 was discovered to contain a remote command execution (RCE) vulnerability via the component sspanel/admin_view.py - GoodsCreateView._post.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2023-38408
 The PKCS#11 feature in ssh-agent in OpenSSH before 9.3p2 has an insufficiently trustworthy search path, leading to remote code execution if an agent is forwarded to an attacker-controlled system. (Code in /usr/lib is not necessarily safe for loading into ssh-agent.) NOTE: this issue exists because of an incomplete fix for CVE-2016-10009.

- [https://github.com/nonosticisiguzo-command/nmap-scan-results](https://github.com/nonosticisiguzo-command/nmap-scan-results) :  ![starts](https://img.shields.io/github/stars/nonosticisiguzo-command/nmap-scan-results.svg) ![forks](https://img.shields.io/github/forks/nonosticisiguzo-command/nmap-scan-results.svg)


## CVE-2022-29078
 The ejs (aka Embedded JavaScript templates) package 3.1.6 for Node.js allows server-side template injection in settings[view options][outputFunctionName]. This is parsed as an internal option, and overwrites the outputFunctionName option with an arbitrary OS command (which is executed upon template compilation).

- [https://github.com/amusedx/CVE-2022-29078](https://github.com/amusedx/CVE-2022-29078) :  ![starts](https://img.shields.io/github/stars/amusedx/CVE-2022-29078.svg) ![forks](https://img.shields.io/github/forks/amusedx/CVE-2022-29078.svg)


## CVE-2022-0847
 A flaw was found in the way the "flags" member of the new pipe buffer structure was lacking proper initialization in copy_page_to_iter_pipe and push_pipe functions in the Linux kernel and could thus contain stale values. An unprivileged local user could use this flaw to write to pages in the page cache backed by read only files and as such escalate their privileges on the system.

- [https://github.com/Scouserr/cve-2022-0847-poc-dockerimage](https://github.com/Scouserr/cve-2022-0847-poc-dockerimage) :  ![starts](https://img.shields.io/github/stars/Scouserr/cve-2022-0847-poc-dockerimage.svg) ![forks](https://img.shields.io/github/forks/Scouserr/cve-2022-0847-poc-dockerimage.svg)


## CVE-2022-0543
 It was discovered, that redis, a persistent key-value database, due to a packaging issue, is prone to a (Debian-specific) Lua sandbox escape, which could result in remote code execution.

- [https://github.com/John-Popovici/CVE-2022-0543-redis-sandbox-escape](https://github.com/John-Popovici/CVE-2022-0543-redis-sandbox-escape) :  ![starts](https://img.shields.io/github/stars/John-Popovici/CVE-2022-0543-redis-sandbox-escape.svg) ![forks](https://img.shields.io/github/forks/John-Popovici/CVE-2022-0543-redis-sandbox-escape.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper](https://github.com/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper) :  ![starts](https://img.shields.io/github/stars/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper.svg) ![forks](https://img.shields.io/github/forks/Kouf320/attacker-lab-cve-2017-5638-cve-2021-41773-paper.svg)


## CVE-2021-40101
 An issue was discovered in Concrete CMS before 8.5.7. The Dashboard allows a user's password to be changed without a prompt for the current password.

- [https://github.com/S1lkys/CVE-2021-40101](https://github.com/S1lkys/CVE-2021-40101) :  ![starts](https://img.shields.io/github/stars/S1lkys/CVE-2021-40101.svg) ![forks](https://img.shields.io/github/forks/S1lkys/CVE-2021-40101.svg)


## CVE-2021-24884
 The Formidable Form Builder WordPress plugin before 4.09.05 allows to inject certain HTML Tags like audio,video,img,a andbutton.This could allow an unauthenticated, remote attacker to exploit a HTML-injection byinjecting a malicous link. The HTML-injection may trick authenticated users to follow the link. If the Link gets clicked, Javascript code can be executed. The vulnerability is due to insufficient sanitization of the "data-frmverify" tag for links in the web-based entry inspection page of affected systems. A successful exploitation incomibantion with CSRF could allow the attacker to perform arbitrary actions on an affected system with the privileges of the user. These actions include stealing the users account by changing their password or allowing attackers to submit their own code through an authenticated user resulting in Remote Code Execution. If an authenticated user who is able to edit Wordpress PHP Code in any kind, clicks the malicious link, PHP code can be edited.

- [https://github.com/S1lkys/CVE-2021-24884](https://github.com/S1lkys/CVE-2021-24884) :  ![starts](https://img.shields.io/github/stars/S1lkys/CVE-2021-24884.svg) ![forks](https://img.shields.io/github/forks/S1lkys/CVE-2021-24884.svg)


## CVE-2021-3560
 It was found that polkit could be tricked into bypassing the credential checks for D-Bus requests, elevating the privileges of the requestor to the root user. This flaw could be used by an unprivileged local attacker to, for example, create a new local administrator. The highest threat from this vulnerability is to data confidentiality and integrity as well as system availability.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2021-2394
 Vulnerability in the Oracle WebLogic Server product of Oracle Fusion Middleware (component: Core). Supported versions that are affected are 10.3.6.0.0, 12.1.3.0.0, 12.2.1.3.0, 12.2.1.4.0 and 14.1.1.0.0. Easily exploitable vulnerability allows unauthenticated attacker with network access via T3, IIOP to compromise Oracle WebLogic Server. Successful attacks of this vulnerability can result in takeover of Oracle WebLogic Server. CVSS 3.1 Base Score 9.8 (Confidentiality, Integrity and Availability impacts). CVSS Vector: (CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H).

- [https://github.com/lz2y/CVE-2021-2394](https://github.com/lz2y/CVE-2021-2394) :  ![starts](https://img.shields.io/github/stars/lz2y/CVE-2021-2394.svg) ![forks](https://img.shields.io/github/forks/lz2y/CVE-2021-2394.svg)
- [https://github.com/freeide/CVE-2021-2394](https://github.com/freeide/CVE-2021-2394) :  ![starts](https://img.shields.io/github/stars/freeide/CVE-2021-2394.svg) ![forks](https://img.shields.io/github/forks/freeide/CVE-2021-2394.svg)
- [https://github.com/BabyTeam1024/CVE-2021-2394](https://github.com/BabyTeam1024/CVE-2021-2394) :  ![starts](https://img.shields.io/github/stars/BabyTeam1024/CVE-2021-2394.svg) ![forks](https://img.shields.io/github/forks/BabyTeam1024/CVE-2021-2394.svg)
- [https://github.com/fasanhlieu/CVE-2021-2394](https://github.com/fasanhlieu/CVE-2021-2394) :  ![starts](https://img.shields.io/github/stars/fasanhlieu/CVE-2021-2394.svg) ![forks](https://img.shields.io/github/forks/fasanhlieu/CVE-2021-2394.svg)


## CVE-2020-29254
 TikiWiki 21.2 allows templates to be edited without CSRF protection. This could allow an unauthenticated, remote attacker to conduct a cross-site request forgery (CSRF) attack and perform arbitrary actions on an affected system. The vulnerability is due to insufficient CSRF protections for the web-based management interface of the affected system. An attacker could exploit this vulnerability by persuading a user of the interface to follow a maliciously crafted link. A successful exploit could allow the attacker to perform arbitrary actions on an affected system with the privileges of the user. These action include allowing attackers to submit their own code through an authenticated user resulting in local file Inclusion. If an authenticated user who is able to edit TikiWiki templates visits an malicious website, template code can be edited.

- [https://github.com/S1lkys/CVE-2020-29254](https://github.com/S1lkys/CVE-2020-29254) :  ![starts](https://img.shields.io/github/stars/S1lkys/CVE-2020-29254.svg) ![forks](https://img.shields.io/github/forks/S1lkys/CVE-2020-29254.svg)


## CVE-2020-24586
 The 802.11 standard that underpins Wi-Fi Protected Access (WPA, WPA2, and WPA3) and Wired Equivalent Privacy (WEP) doesn't require that received fragments be cleared from memory after (re)connecting to a network. Under the right circumstances, when another device sends fragmented frames encrypted using WEP, CCMP, or GCMP, this can be abused to inject arbitrary network packets and/or exfiltrate user data.

- [https://github.com/elvira-alec/fracture](https://github.com/elvira-alec/fracture) :  ![starts](https://img.shields.io/github/stars/elvira-alec/fracture.svg) ![forks](https://img.shields.io/github/forks/elvira-alec/fracture.svg)


## CVE-2020-15906
 tiki-login.php in Tiki before 21.2 sets the admin password to a blank value after 50 invalid login attempts.

- [https://github.com/S1lkys/CVE-2020-15906](https://github.com/S1lkys/CVE-2020-15906) :  ![starts](https://img.shields.io/github/stars/S1lkys/CVE-2020-15906.svg) ![forks](https://img.shields.io/github/forks/S1lkys/CVE-2020-15906.svg)


## CVE-2020-12446
 The ene.sys driver in G.SKILL Trident Z Lighting Control through 1.00.08 exposes mapping and un-mapping of physical memory, reading and writing to Model Specific Register (MSR) registers, and input from and output to I/O ports to local non-privileged users. This leads to privilege escalation to NT AUTHORITY\SYSTEM.

- [https://github.com/S1lkys/Eneio64-LPE](https://github.com/S1lkys/Eneio64-LPE) :  ![starts](https://img.shields.io/github/stars/S1lkys/Eneio64-LPE.svg) ![forks](https://img.shields.io/github/forks/S1lkys/Eneio64-LPE.svg)


## CVE-2020-11107
 An issue was discovered in XAMPP before 7.2.29, 7.3.x before 7.3.16 , and 7.4.x before 7.4.4 on Windows. An unprivileged user can change a .exe configuration in xampp-contol.ini for all users (including admins) to enable arbitrary command execution.

- [https://github.com/S1lkys/CVE-2020-11107](https://github.com/S1lkys/CVE-2020-11107) :  ![starts](https://img.shields.io/github/stars/S1lkys/CVE-2020-11107.svg) ![forks](https://img.shields.io/github/forks/S1lkys/CVE-2020-11107.svg)


## CVE-2019-12881
 i915_gem_userptr_get_pages in drivers/gpu/drm/i915/i915_gem_userptr.c in the Linux kernel 4.15.0 on Ubuntu 18.04.2 allows local users to cause a denial of service (NULL pointer dereference and BUG) or possibly have unspecified other impact via crafted ioctl calls to /dev/dri/card0.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)

