# Update 2026-04-22
## CVE-2026-35616
 A improper access control vulnerability in Fortinet FortiClientEMS 7.4.5 through 7.4.6 may allow an unauthenticated attacker to execute unauthorized code or commands via crafted requests.

- [https://github.com/wa6n3r/CVE-2026-35616](https://github.com/wa6n3r/CVE-2026-35616) :  ![starts](https://img.shields.io/github/stars/wa6n3r/CVE-2026-35616.svg) ![forks](https://img.shields.io/github/forks/wa6n3r/CVE-2026-35616.svg)


## CVE-2026-35570
 OpenClaude is an open-source coding-agent command line interface for cloud and local model providers. Versions prior to 0.5.1 have a logic flaw in `bashToolHasPermission()` inside `src/tools/BashTool/bashPermissions.ts`. When the sandbox auto-allow feature is active and no explicit deny rule is configured, the function returns an `allow` result immediately — before the path constraint filter (`checkPathConstraints`) is ever evaluated. This allows commands containing path traversal sequences (e.g., `../../../../../etc/passwd`) to bypass directory restrictions entirely. Version 0.5.1 contains a patch for the issue.

- [https://github.com/Rickidevs/CVE-2026-35570](https://github.com/Rickidevs/CVE-2026-35570) :  ![starts](https://img.shields.io/github/stars/Rickidevs/CVE-2026-35570.svg) ![forks](https://img.shields.io/github/forks/Rickidevs/CVE-2026-35570.svg)


## CVE-2026-34197
Users are recommended to upgrade to version 5.19.4 or 6.2.3, which fixes the issue

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)
- [https://github.com/xshysjhq/CVE-2026-34197-payload-Apache-ActiveMQ-](https://github.com/xshysjhq/CVE-2026-34197-payload-Apache-ActiveMQ-) :  ![starts](https://img.shields.io/github/stars/xshysjhq/CVE-2026-34197-payload-Apache-ActiveMQ-.svg) ![forks](https://img.shields.io/github/forks/xshysjhq/CVE-2026-34197-payload-Apache-ActiveMQ-.svg)


## CVE-2026-33825
 Insufficient granularity of access control in Microsoft Defender allows an authorized attacker to elevate privileges locally.

- [https://github.com/Bilal3755/Detecting_blue_hammer_vuln](https://github.com/Bilal3755/Detecting_blue_hammer_vuln) :  ![starts](https://img.shields.io/github/stars/Bilal3755/Detecting_blue_hammer_vuln.svg) ![forks](https://img.shields.io/github/forks/Bilal3755/Detecting_blue_hammer_vuln.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/Jorrit-VM/CVE-2026-33017](https://github.com/Jorrit-VM/CVE-2026-33017) :  ![starts](https://img.shields.io/github/stars/Jorrit-VM/CVE-2026-33017.svg) ![forks](https://img.shields.io/github/forks/Jorrit-VM/CVE-2026-33017.svg)


## CVE-2026-32746
 telnetd in GNU inetutils through 2.7 allows an out-of-bounds write in the LINEMODE SLC (Set Local Characters) suboption handler because add_slc does not check whether the buffer is full.

- [https://github.com/duduLiu8787/CVE-2026-32746-Exploit](https://github.com/duduLiu8787/CVE-2026-32746-Exploit) :  ![starts](https://img.shields.io/github/stars/duduLiu8787/CVE-2026-32746-Exploit.svg) ![forks](https://img.shields.io/github/forks/duduLiu8787/CVE-2026-32746-Exploit.svg)


## CVE-2026-30615
 A prompt injection vulnerability in Windsurf 1.9544.26 allows remote attackers to execute arbitrary commands on a victim system. When Windsurf processes attacker-controlled HTML content, malicious instructions can cause unauthorized modification of the local MCP configuration and automatic registration of a malicious MCP STDIO server, resulting in execution of arbitrary commands without further user interaction. Successful exploitation may allow attackers to execute commands on behalf of the user, persist malicious MCP configuration changes, and access sensitive information exposed through the application.

- [https://github.com/TreRB/ai-ide-config-guard](https://github.com/TreRB/ai-ide-config-guard) :  ![starts](https://img.shields.io/github/stars/TreRB/ai-ide-config-guard.svg) ![forks](https://img.shields.io/github/forks/TreRB/ai-ide-config-guard.svg)


## CVE-2026-26399
 A stack-use-after-return issue exists in the Arduino_Core_STM32 library prior to version 1.7.0. The pwm_start() function allocates a TIM_HandleTypeDef structure on the stack and passes its address to HAL initialization routines, where it is stored in a global timer handle registry. After the function returns, interrupt service routines may dereference this dangling pointer, resulting in memory corruption.

- [https://github.com/Acen28/CVE-2026-26399-Disclosure](https://github.com/Acen28/CVE-2026-26399-Disclosure) :  ![starts](https://img.shields.io/github/stars/Acen28/CVE-2026-26399-Disclosure.svg) ![forks](https://img.shields.io/github/forks/Acen28/CVE-2026-26399-Disclosure.svg)


## CVE-2026-21852
 Claude Code is an agentic coding tool. Prior to version 2.0.65, vulnerability in Claude Code's project-load flow allowed malicious repositories to exfiltrate data including Anthropic API keys before users confirmed trust. An attacker-controlled repository could include a settings file that sets ANTHROPIC_BASE_URL to an attacker-controlled endpoint and when the repository was opened, Claude Code would read the configuration and immediately issue API requests before showing the trust prompt, potentially leaking the user's API keys. Users on standard Claude Code auto-update have received this fix already. Users performing manual updates are advised to update to version 2.0.65, which contains a patch, or to the latest version.

- [https://github.com/TreRB/ai-ide-config-guard](https://github.com/TreRB/ai-ide-config-guard) :  ![starts](https://img.shields.io/github/stars/TreRB/ai-ide-config-guard.svg) ![forks](https://img.shields.io/github/forks/TreRB/ai-ide-config-guard.svg)


## CVE-2026-5760
 SGLang's reranking endpoint (/v1/rerank) achieves Remote Code Execution (RCE) when a model file containing a malcious tokenizer.chat_template is loaded, as the Jinja2 chat templates are rendered using an unsandboxed jinja2.Environment().

- [https://github.com/Stuub/SGLang-0.5.9-RCE](https://github.com/Stuub/SGLang-0.5.9-RCE) :  ![starts](https://img.shields.io/github/stars/Stuub/SGLang-0.5.9-RCE.svg) ![forks](https://img.shields.io/github/forks/Stuub/SGLang-0.5.9-RCE.svg)


## CVE-2026-4484
 The Masteriyo LMS plugin for WordPress is vulnerable to Privilege Escalation in all versions up to, and including, 2.1.6. This is due to the plugin allowing a user to update the user role through the 'InstructorsController::prepare_object_for_database' function. This makes it possible for authenticated attackers, with Student-level access and above, to elevate their privileges to that of an administrator.

- [https://github.com/PegasusMetaSec/PEGASUS-CVE-2026-4484](https://github.com/PegasusMetaSec/PEGASUS-CVE-2026-4484) :  ![starts](https://img.shields.io/github/stars/PegasusMetaSec/PEGASUS-CVE-2026-4484.svg) ![forks](https://img.shields.io/github/forks/PegasusMetaSec/PEGASUS-CVE-2026-4484.svg)


## CVE-2026-2754
 Navtor NavBox exposes sensitive configuration and operational data due to missing authentication on HTTP API endpoints. An unauthenticated remote attacker with network access to the device can execute HTTP GET requests to TCP port 8080 to retrieve internal network parameters including ECDIS & OT Information, device identifiers, and service status logs.

- [https://github.com/PegasusMetaSec/PEGASUS-CVE-2026-2754](https://github.com/PegasusMetaSec/PEGASUS-CVE-2026-2754) :  ![starts](https://img.shields.io/github/stars/PegasusMetaSec/PEGASUS-CVE-2026-2754.svg) ![forks](https://img.shields.io/github/forks/PegasusMetaSec/PEGASUS-CVE-2026-2754.svg)


## CVE-2026-2600
 The ElementsKit Elementor Addons and Templates plugin for WordPress is vulnerable to Stored Cross-Site Scripting via the 'ekit_tab_title' parameter in the Simple Tab widget in all versions up to, and including, 3.7.9 due to insufficient input sanitization and output escaping on user supplied attributes. This makes it possible for authenticated attackers, with contributor-level access and above, to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page.

- [https://github.com/FOLKS-iwd/CVE-2026-2600-POC](https://github.com/FOLKS-iwd/CVE-2026-2600-POC) :  ![starts](https://img.shields.io/github/stars/FOLKS-iwd/CVE-2026-2600-POC.svg) ![forks](https://img.shields.io/github/forks/FOLKS-iwd/CVE-2026-2600-POC.svg)


## CVE-2025-68999
 Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection') vulnerability in HappyMonster Happy Addons for Elementor happy-elementor-addons allows Blind SQL Injection.This issue affects Happy Addons for Elementor: from n/a through = 3.20.4.

- [https://github.com/FOLKS-iwd/CVE-2025-68999-POC](https://github.com/FOLKS-iwd/CVE-2025-68999-POC) :  ![starts](https://img.shields.io/github/stars/FOLKS-iwd/CVE-2025-68999-POC.svg) ![forks](https://img.shields.io/github/forks/FOLKS-iwd/CVE-2025-68999-POC.svg)


## CVE-2025-66954
 A vulnerability exists in the Buffalo Link Station version 1.85-0.01 that allows unauthenticated or guest-level users to enumerate valid usernames and their associated privilege roles. The issue is triggered by modifying a parameter within requests sent to the /nasapi endpoint.

- [https://github.com/DBmonster19/CVE-2025-66954](https://github.com/DBmonster19/CVE-2025-66954) :  ![starts](https://img.shields.io/github/stars/DBmonster19/CVE-2025-66954.svg) ![forks](https://img.shields.io/github/forks/DBmonster19/CVE-2025-66954.svg)


## CVE-2025-59536
 Claude Code is an agentic coding tool. Versions before 1.0.111 were vulnerable to Code Injection due to a bug in the startup trust dialog implementation. Claude Code could be tricked to execute code contained in a project before the user accepted the startup trust dialog. Exploiting this requires a user to start Claude Code in an untrusted directory. Users on standard Claude Code auto-update will have received this fix automatically. Users performing manual updates are advised to update to the latest version. This issue is fixed in version 1.0.111.

- [https://github.com/TreRB/ai-ide-config-guard](https://github.com/TreRB/ai-ide-config-guard) :  ![starts](https://img.shields.io/github/stars/TreRB/ai-ide-config-guard.svg) ![forks](https://img.shields.io/github/forks/TreRB/ai-ide-config-guard.svg)


## CVE-2025-58434
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5 and earlier, the `forgot-password` endpoint in Flowise returns sensitive information including a valid password reset `tempToken` without authentication or verification. This enables any attacker to generate a reset token for arbitrary users and directly reset their password, leading to a complete account takeover (ATO). This vulnerability applies to both the cloud service (`cloud.flowiseai.com`) and self-hosted/local Flowise deployments that expose the same API. Commit 9e178d68873eb876073846433a596590d3d9c863 in version 3.0.6 secures password reset endpoints. Several recommended remediation steps are available. Do not return reset tokens or sensitive account details in API responses. Tokens must only be delivered securely via the registered email channel. Ensure `forgot-password` responds with a generic success message regardless of input, to avoid user enumeration. Require strong validation of the `tempToken` (e.g., single-use, short expiry, tied to request origin, validated against email delivery). Apply the same fixes to both cloud and self-hosted/local deployments. Log and monitor password reset requests for suspicious activity. Consider multi-factor verification for sensitive accounts.

- [https://github.com/SteamPunk424/CVE-2025-58434-Unauthenticated-Password-Reset-Flowwise](https://github.com/SteamPunk424/CVE-2025-58434-Unauthenticated-Password-Reset-Flowwise) :  ![starts](https://img.shields.io/github/stars/SteamPunk424/CVE-2025-58434-Unauthenticated-Password-Reset-Flowwise.svg) ![forks](https://img.shields.io/github/forks/SteamPunk424/CVE-2025-58434-Unauthenticated-Password-Reset-Flowwise.svg)


## CVE-2025-32711
 Ai command injection in M365 Copilot allows an unauthorized attacker to disclose information over a network.

- [https://github.com/TreRB/markdown-exfil-tester](https://github.com/TreRB/markdown-exfil-tester) :  ![starts](https://img.shields.io/github/stars/TreRB/markdown-exfil-tester.svg) ![forks](https://img.shields.io/github/forks/TreRB/markdown-exfil-tester.svg)


## CVE-2025-31161
 CrushFTP 10 before 10.8.4 and 11 before 11.3.1 allows authentication bypass and takeover of the crushadmin account (unless a DMZ proxy instance is used), as exploited in the wild in March and April 2025, aka "Unauthenticated HTTP(S) port access." A race condition exists in the AWS4-HMAC (compatible with S3) authorization method of the HTTP component of the FTP server. The server first verifies the existence of the user by performing a call to login_user_pass() with no password requirement. This will authenticate the session through the HMAC verification process and up until the server checks for user verification once more. The vulnerability can be further stabilized, eliminating the need for successfully triggering a race condition, by sending a mangled AWS4-HMAC header. By providing only the username and a following slash (/), the server will successfully find a username, which triggers the successful anypass authentication process, but the server will fail to find the expected SignedHeaders entry, resulting in an index-out-of-bounds error that stops the code from reaching the session cleanup. Together, these issues make it trivial to authenticate as any known or guessable user (e.g., crushadmin), and can lead to a full compromise of the system by obtaining an administrative account.

- [https://github.com/0xBlackash/CVE-2025-31161](https://github.com/0xBlackash/CVE-2025-31161) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-31161.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-31161.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/KaztoRay/CVE-2025-29927-Research](https://github.com/KaztoRay/CVE-2025-29927-Research) :  ![starts](https://img.shields.io/github/stars/KaztoRay/CVE-2025-29927-Research.svg) ![forks](https://img.shields.io/github/forks/KaztoRay/CVE-2025-29927-Research.svg)


## CVE-2025-11460
 Use after free in Storage in Google Chrome prior to 141.0.7390.65 allowed a remote attacker to execute arbitrary code via a crafted video file. (Chromium security severity: High)

- [https://github.com/lylzjnqe/CVE-2025-11460-Chrome-RCE](https://github.com/lylzjnqe/CVE-2025-11460-Chrome-RCE) :  ![starts](https://img.shields.io/github/stars/lylzjnqe/CVE-2025-11460-Chrome-RCE.svg) ![forks](https://img.shields.io/github/forks/lylzjnqe/CVE-2025-11460-Chrome-RCE.svg)


## CVE-2025-2563
 The User Registration & Membership  WordPress plugin before 4.1.2 does not prevent users to set their account role when the Membership Addon is enabled, leading to a privilege escalation issue and allowing unauthenticated users to gain admin privileges

- [https://github.com/dokter69/CVE-2025-2563](https://github.com/dokter69/CVE-2025-2563) :  ![starts](https://img.shields.io/github/stars/dokter69/CVE-2025-2563.svg) ![forks](https://img.shields.io/github/forks/dokter69/CVE-2025-2563.svg)


## CVE-2024-46987
 Camaleon CMS is a dynamic and advanced content management system based on Ruby on Rails. A path traversal vulnerability accessible via MediaController's download_private_file method allows authenticated users to download any file on the web server Camaleon CMS is running on (depending on the file permissions). This issue may lead to Information Disclosure. This issue has been addressed in release version 2.8.2. Users are advised to upgrade. There are no known workarounds for this vulnerability.

- [https://github.com/ramzerk/CVE-2024-46987](https://github.com/ramzerk/CVE-2024-46987) :  ![starts](https://img.shields.io/github/stars/ramzerk/CVE-2024-46987.svg) ![forks](https://img.shields.io/github/forks/ramzerk/CVE-2024-46987.svg)


## CVE-2024-3094
Through a series of complex obfuscations, the liblzma build process extracts a prebuilt object file from a disguised test file existing in the source code, which is then used to modify specific functions in the liblzma code. This results in a modified liblzma library that can be used by any software linked against this library, intercepting and modifying the data interaction with this library.

- [https://github.com/vnchk1/sec_review_cve-2024-3094](https://github.com/vnchk1/sec_review_cve-2024-3094) :  ![starts](https://img.shields.io/github/stars/vnchk1/sec_review_cve-2024-3094.svg) ![forks](https://img.shields.io/github/forks/vnchk1/sec_review_cve-2024-3094.svg)


## CVE-2023-20198
 Cisco is providing an update for the ongoing investigation into observed exploitation of the web UI feature in Cisco IOS XE Software. We are updating the list of fixed releases and adding the Software Checker. Our investigation has determined that the actors exploited two previously unknown issues. The attacker first exploited CVE-2023-20198 to gain initial access and issued a privilege 15 command to create a local user and password combination. This allowed the user to log in with normal user access. The attacker then exploited another component of the web UI feature, leveraging the new local user to elevate privilege to root and write the implant to the file system. Cisco has assigned CVE-2023-20273 to this issue. CVE-2023-20198 has been assigned a CVSS Score of 10.0. CVE-2023-20273 has been assigned a CVSS Score of 7.2. Both of these CVEs are being tracked by CSCwh87343.

- [https://github.com/AjayKalbhile/Cisco-SD-WAN-Auth-Bypass-Pentest](https://github.com/AjayKalbhile/Cisco-SD-WAN-Auth-Bypass-Pentest) :  ![starts](https://img.shields.io/github/stars/AjayKalbhile/Cisco-SD-WAN-Auth-Bypass-Pentest.svg) ![forks](https://img.shields.io/github/forks/AjayKalbhile/Cisco-SD-WAN-Auth-Bypass-Pentest.svg)


## CVE-2022-46364
 A SSRF vulnerability in parsing the href attribute of XOP:Include in MTOM requests in versions of Apache CXF before 3.5.5 and 3.4.10 allows an attacker to perform SSRF style attacks on webservices that take at least one parameter of any type. 

- [https://github.com/cybermaksx/CVE-2022-46364-Proof-of-the-concept](https://github.com/cybermaksx/CVE-2022-46364-Proof-of-the-concept) :  ![starts](https://img.shields.io/github/stars/cybermaksx/CVE-2022-46364-Proof-of-the-concept.svg) ![forks](https://img.shields.io/github/forks/cybermaksx/CVE-2022-46364-Proof-of-the-concept.svg)


## CVE-2004-2687
 distcc 2.x, as used in XCode 1.5 and others, when not configured to restrict access to the server port, allows remote attackers to execute arbitrary commands via compilation jobs, which are executed by the server without authorization checks.

- [https://github.com/micheaol/distccd_rce_CVE-2004-2687](https://github.com/micheaol/distccd_rce_CVE-2004-2687) :  ![starts](https://img.shields.io/github/stars/micheaol/distccd_rce_CVE-2004-2687.svg) ![forks](https://img.shields.io/github/forks/micheaol/distccd_rce_CVE-2004-2687.svg)

