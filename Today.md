# Update 2026-04-25
## CVE-2026-41651
3. Late flag read at execution time (lines 2273–2277): The scheduler's idle callback reads cached_transaction_flags at dispatch time, not at authorization time. If flags were overwritten between authorization and execution, the backend sees the attacker's flags.

- [https://github.com/Vozec/CVE-2026-41651](https://github.com/Vozec/CVE-2026-41651) :  ![starts](https://img.shields.io/github/stars/Vozec/CVE-2026-41651.svg) ![forks](https://img.shields.io/github/forks/Vozec/CVE-2026-41651.svg)
- [https://github.com/CipherCloak/CVE-2026-41651](https://github.com/CipherCloak/CVE-2026-41651) :  ![starts](https://img.shields.io/github/stars/CipherCloak/CVE-2026-41651.svg) ![forks](https://img.shields.io/github/forks/CipherCloak/CVE-2026-41651.svg)


## CVE-2026-41303
 OpenClaw before 2026.3.28 contains an authorization bypass vulnerability in Discord text approval commands that allows non-approvers to resolve pending exec approvals. Attackers can send Discord text commands to bypass the channels.discord.execApprovals.approvers allowlist and approve pending host execution requests.

- [https://github.com/kaleth4/CVE-2026-41303](https://github.com/kaleth4/CVE-2026-41303) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-41303.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-41303.svg)


## CVE-2026-39813
 A path traversal: '../filedir' vulnerability in Fortinet FortiSandbox 5.0.0 through 5.0.5, FortiSandbox 4.4.0 through 4.4.8 may allow attacker to escalation of privilege via insert attack vector here

- [https://github.com/0xBlackash/CVE-2026-39813](https://github.com/0xBlackash/CVE-2026-39813) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-39813.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-39813.svg)


## CVE-2026-34159
 llama.cpp is an inference of several LLM models in C/C++. Prior to version b8492, the RPC backend's deserialize_tensor() skips all bounds validation when a tensor's buffer field is 0. An unauthenticated attacker can read and write arbitrary process memory via crafted GRAPH_COMPUTE messages. Combined with pointer leaks from ALLOC_BUFFER/BUFFER_GET_BASE, this gives full ASLR bypass and remote code execution. No authentication required, just TCP access to the RPC server port. This issue has been patched in version b8492.

- [https://github.com/casp3r0x0/CVE-2026-34159](https://github.com/casp3r0x0/CVE-2026-34159) :  ![starts](https://img.shields.io/github/stars/casp3r0x0/CVE-2026-34159.svg) ![forks](https://img.shields.io/github/forks/casp3r0x0/CVE-2026-34159.svg)


## CVE-2026-33725
 Metabase is an open source business intelligence and embedded analytics tool. In Metabase Enterprise prior to versions 1.54.22, 1.55.22, 1.56.22, 1.57.16, 1.58.10, and 1.59.4, authenticated admins on Metabase Enterprise Edition can achieve Remote Code Execution (RCE) and Arbitrary File Read via the `POST /api/ee/serialization/import` endpoint. A crafted serialization archive injects an `INIT` property into the H2 JDBC spec, which can execute arbitrary SQL during a database sync. We confirmed this was possible on Metabase Cloud. This only affects Metabase Enterprise. Metabase OSS lacks the affected codepaths. All versions of Metabase Enterprise that have serialization, which dates back to at least version 1.47, are affected. Metabase Enterprise versions 1.54.22, 1.55.22, 1.56.22, 1.57.16, 1.58.10, and 1.59.4 patch the issue. As a workaround, disable the serialization import endpoint in their Metabase instance to prevent access to the vulnerable codepaths.

- [https://github.com/hakaioffsec/CVE-2026-33725](https://github.com/hakaioffsec/CVE-2026-33725) :  ![starts](https://img.shields.io/github/stars/hakaioffsec/CVE-2026-33725.svg) ![forks](https://img.shields.io/github/forks/hakaioffsec/CVE-2026-33725.svg)


## CVE-2026-29145
Users are recommended to upgrade to version Tomcat Native 1.3.7 or 2.0.14 and Tomcat 11.0.20, 10.1.53 and 9.0.116, which fix the issue.

- [https://github.com/sancliffe/CVE-2026-29145-Tester](https://github.com/sancliffe/CVE-2026-29145-Tester) :  ![starts](https://img.shields.io/github/stars/sancliffe/CVE-2026-29145-Tester.svg) ![forks](https://img.shields.io/github/forks/sancliffe/CVE-2026-29145-Tester.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/d0x-awrqxavc/CVE-2026-23744](https://github.com/d0x-awrqxavc/CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/d0x-awrqxavc/CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/d0x-awrqxavc/CVE-2026-23744.svg)


## CVE-2026-4106
 The HT Mega Addons for Elementor  WordPress plugin before 3.0.7 contains an unauthenticated AJAX action returning some PII (such as full name, city, state and country) of customers who placed orders in the last 7 days

- [https://github.com/ef3tr/CVE-2026-4106](https://github.com/ef3tr/CVE-2026-4106) :  ![starts](https://img.shields.io/github/stars/ef3tr/CVE-2026-4106.svg) ![forks](https://img.shields.io/github/forks/ef3tr/CVE-2026-4106.svg)


## CVE-2026-1459
 A post-authentication command injection vulnerability in the TR-369 certificate download CGI program of the Zyxel VMG3625-T50B firmware versions through 5.50(ABPM.9.7)C0 could allow an authenticated attacker with administrator privileges to execute operating system (OS) commands on an affected device.

- [https://github.com/Toouch67/CVE-2026-1459-POC](https://github.com/Toouch67/CVE-2026-1459-POC) :  ![starts](https://img.shields.io/github/stars/Toouch67/CVE-2026-1459-POC.svg) ![forks](https://img.shields.io/github/forks/Toouch67/CVE-2026-1459-POC.svg)


## CVE-2026-0603
 A flaw was found in Hibernate. A remote attacker with low privileges could exploit a second-order SQL injection vulnerability by providing specially crafted, unsanitized non-alphanumeric characters in the ID column when the InlineIdsOrClauseBuilder is used. This could lead to sensitive information disclosure, such as reading system files, and allow for data manipulation or deletion within the application's database, resulting in an application level denial of service.

- [https://github.com/EQSTLab/CVE-2026-0603](https://github.com/EQSTLab/CVE-2026-0603) :  ![starts](https://img.shields.io/github/stars/EQSTLab/CVE-2026-0603.svg) ![forks](https://img.shields.io/github/forks/EQSTLab/CVE-2026-0603.svg)


## CVE-2025-70994
 Yadea T5 Electric Bicycles (models manufactured in/after 2024) have a weak authentication mechanism in their keyless entry system. The system utilizes the EV1527 fixed-code RF protocol without implementing rolling codes or cryptographic challenge-response mechanisms. This is vulnerable to signal forgery after a local attacker intercepts any legitimate key fob transmission, allowing for complete unauthorized vehicle operation via a replay attack.

- [https://github.com/ktauchathuranga/CVE-2025-70994](https://github.com/ktauchathuranga/CVE-2025-70994) :  ![starts](https://img.shields.io/github/stars/ktauchathuranga/CVE-2025-70994.svg) ![forks](https://img.shields.io/github/forks/ktauchathuranga/CVE-2025-70994.svg)


## CVE-2025-59528
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5, Flowise is vulnerable to remote code execution. The CustomMCP node allows users to input configuration settings for connecting to an external MCP server. This node parses the user-provided mcpServerConfig string to build the MCP server configuration. However, during this process, it executes JavaScript code without any security validation. Specifically, inside the convertToValidJSONString function, user input is directly passed to the Function() constructor, which evaluates and executes the input as JavaScript code. Since this runs with full Node.js runtime privileges, it can access dangerous modules such as child_process and fs. This issue has been patched in version 3.0.6.

- [https://github.com/karimelsheikh1/HTB-Silentium-Writeup](https://github.com/karimelsheikh1/HTB-Silentium-Writeup) :  ![starts](https://img.shields.io/github/stars/karimelsheikh1/HTB-Silentium-Writeup.svg) ![forks](https://img.shields.io/github/forks/karimelsheikh1/HTB-Silentium-Writeup.svg)


## CVE-2025-58434
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5 and earlier, the `forgot-password` endpoint in Flowise returns sensitive information including a valid password reset `tempToken` without authentication or verification. This enables any attacker to generate a reset token for arbitrary users and directly reset their password, leading to a complete account takeover (ATO). This vulnerability applies to both the cloud service (`cloud.flowiseai.com`) and self-hosted/local Flowise deployments that expose the same API. Commit 9e178d68873eb876073846433a596590d3d9c863 in version 3.0.6 secures password reset endpoints. Several recommended remediation steps are available. Do not return reset tokens or sensitive account details in API responses. Tokens must only be delivered securely via the registered email channel. Ensure `forgot-password` responds with a generic success message regardless of input, to avoid user enumeration. Require strong validation of the `tempToken` (e.g., single-use, short expiry, tied to request origin, validated against email delivery). Apply the same fixes to both cloud and self-hosted/local deployments. Log and monitor password reset requests for suspicious activity. Consider multi-factor verification for sensitive accounts.

- [https://github.com/karimelsheikh1/HTB-Silentium-Writeup](https://github.com/karimelsheikh1/HTB-Silentium-Writeup) :  ![starts](https://img.shields.io/github/stars/karimelsheikh1/HTB-Silentium-Writeup.svg) ![forks](https://img.shields.io/github/forks/karimelsheikh1/HTB-Silentium-Writeup.svg)


## CVE-2025-55182
 A pre-authentication remote code execution vulnerability exists in React Server Components versions 19.0.0, 19.1.0, 19.1.1, and 19.2.0 including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints.

- [https://github.com/TrixSec/CVE-2025-55182-Scanner](https://github.com/TrixSec/CVE-2025-55182-Scanner) :  ![starts](https://img.shields.io/github/stars/TrixSec/CVE-2025-55182-Scanner.svg) ![forks](https://img.shields.io/github/forks/TrixSec/CVE-2025-55182-Scanner.svg)


## CVE-2025-47812
 In Wing FTP Server before 7.4.4. the user and admin web interfaces mishandle '\0' bytes, ultimately allowing injection of arbitrary Lua code into user session files. This can be used to execute arbitrary system commands with the privileges of the FTP service (root or SYSTEM by default). This is thus a remote code execution vulnerability that guarantees a total server compromise. This is also exploitable via anonymous FTP accounts.

- [https://github.com/AmogelangMongwaketse/cs50-final-project](https://github.com/AmogelangMongwaketse/cs50-final-project) :  ![starts](https://img.shields.io/github/stars/AmogelangMongwaketse/cs50-final-project.svg) ![forks](https://img.shields.io/github/forks/AmogelangMongwaketse/cs50-final-project.svg)


## CVE-2025-31207
 A logic issue was addressed with improved checks. This issue is fixed in iOS 18.5 and iPadOS 18.5. An app may be able to enumerate a user's installed apps.

- [https://github.com/iCrazeiOS/AppEnumFix](https://github.com/iCrazeiOS/AppEnumFix) :  ![starts](https://img.shields.io/github/stars/iCrazeiOS/AppEnumFix.svg) ![forks](https://img.shields.io/github/forks/iCrazeiOS/AppEnumFix.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/MKIRAHMET/CVE-2025-29927-PoC](https://github.com/MKIRAHMET/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/MKIRAHMET/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/MKIRAHMET/CVE-2025-29927-PoC.svg)


## CVE-2025-10353
 File upload leading to remote code execution (RCE) in the “melis-cms-slider” module of Melis Technology's Melis Platform. This vulnerability allows an attacker to upload a malicious file via a POST request to '/melis/MelisCmsSlider/MelisCmsSliderDetails/saveDetailsForm' using the 'mcsdetail_img' parameter.

- [https://github.com/ivansmc/CVE-2025-10353-POC](https://github.com/ivansmc/CVE-2025-10353-POC) :  ![starts](https://img.shields.io/github/stars/ivansmc/CVE-2025-10353-POC.svg) ![forks](https://img.shields.io/github/forks/ivansmc/CVE-2025-10353-POC.svg)


## CVE-2025-10352
 Vulnerability in the melis-core module of Melis Technology's Melis Platform, which, if exploited, allows an unauthenticated attacker to create an administrator account via a request to '/melis/MelisCore/ToolUser/addNewUser'.

- [https://github.com/ivansmc/CVE-2025-10352-POC](https://github.com/ivansmc/CVE-2025-10352-POC) :  ![starts](https://img.shields.io/github/stars/ivansmc/CVE-2025-10352-POC.svg) ![forks](https://img.shields.io/github/forks/ivansmc/CVE-2025-10352-POC.svg)


## CVE-2025-10351
 SQL injection vulnerability based on the melis-cms module of the Melis platform from Melis Technology. This vulnerability allows an attacker to retrieve, create, update, and delete databases through the 'idPage' parameter in the '/melis/MelisCms/PageEdition/getTinyTemplates' endpoint.

- [https://github.com/ivansmc/CVE-2025-10351-POC](https://github.com/ivansmc/CVE-2025-10351-POC) :  ![starts](https://img.shields.io/github/stars/ivansmc/CVE-2025-10351-POC.svg) ![forks](https://img.shields.io/github/forks/ivansmc/CVE-2025-10351-POC.svg)


## CVE-2025-8110
 Improper Symbolic link handling in the PutContents API in Gogs allows Local Execution of Code.

- [https://github.com/karimelsheikh1/HTB-Silentium-Writeup](https://github.com/karimelsheikh1/HTB-Silentium-Writeup) :  ![starts](https://img.shields.io/github/stars/karimelsheikh1/HTB-Silentium-Writeup.svg) ![forks](https://img.shields.io/github/forks/karimelsheikh1/HTB-Silentium-Writeup.svg)


## CVE-2025-6018
 A Local Privilege Escalation (LPE) vulnerability has been discovered in pam-config within Linux Pluggable Authentication Modules (PAM). This flaw allows an unprivileged local attacker (for example, a user logged in via SSH) to obtain the elevated privileges normally reserved for a physically present, "allow_active" user. The highest risk is that the attacker can then perform all allow_active yes Polkit actions, which are typically restricted to console users, potentially gaining unauthorized control over system configurations, services, or other sensitive operations.

- [https://github.com/karimelsheikh1/HTB-Pterodactyl-Writeup](https://github.com/karimelsheikh1/HTB-Pterodactyl-Writeup) :  ![starts](https://img.shields.io/github/stars/karimelsheikh1/HTB-Pterodactyl-Writeup.svg) ![forks](https://img.shields.io/github/forks/karimelsheikh1/HTB-Pterodactyl-Writeup.svg)


## CVE-2025-5880
 A vulnerability has been found in Whistle 2.9.98 and classified as problematic. This vulnerability affects unknown code of the file /cgi-bin/sessions/get-temp-file. The manipulation of the argument filename leads to path traversal. The exploit has been disclosed to the public and may be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/yacine-rm/CVE-2025-5880-PoC](https://github.com/yacine-rm/CVE-2025-5880-PoC) :  ![starts](https://img.shields.io/github/stars/yacine-rm/CVE-2025-5880-PoC.svg) ![forks](https://img.shields.io/github/forks/yacine-rm/CVE-2025-5880-PoC.svg)


## CVE-2024-30088
 Windows Kernel Elevation of Privilege Vulnerability

- [https://github.com/oioio-space/maldev](https://github.com/oioio-space/maldev) :  ![starts](https://img.shields.io/github/stars/oioio-space/maldev.svg) ![forks](https://img.shields.io/github/forks/oioio-space/maldev.svg)


## CVE-2024-29296
 A user enumeration vulnerability was found in Portainer CE 2.19.4. This issue occurs during user authentication process, where a difference in response time could allow a remote unauthenticated user to determine if a username is valid or not.

- [https://github.com/Lavender-exe/CVE-2024-29296-PoC](https://github.com/Lavender-exe/CVE-2024-29296-PoC) :  ![starts](https://img.shields.io/github/stars/Lavender-exe/CVE-2024-29296-PoC.svg) ![forks](https://img.shields.io/github/forks/Lavender-exe/CVE-2024-29296-PoC.svg)


## CVE-2024-3094
Through a series of complex obfuscations, the liblzma build process extracts a prebuilt object file from a disguised test file existing in the source code, which is then used to modify specific functions in the liblzma code. This results in a modified liblzma library that can be used by any software linked against this library, intercepting and modifying the data interaction with this library.

- [https://github.com/0xBlackash/CVE-2024-3094](https://github.com/0xBlackash/CVE-2024-3094) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2024-3094.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2024-3094.svg)


## CVE-2023-44487
 The HTTP/2 protocol allows a denial of service (server resource consumption) because request cancellation can reset many streams quickly, as exploited in the wild in August through October 2023.

- [https://github.com/galletitaconpate/CVE-2023-44487](https://github.com/galletitaconpate/CVE-2023-44487) :  ![starts](https://img.shields.io/github/stars/galletitaconpate/CVE-2023-44487.svg) ![forks](https://img.shields.io/github/forks/galletitaconpate/CVE-2023-44487.svg)


## CVE-2023-0386
 A flaw was found in the Linux kernel, where unauthorized access to the execution of the setuid file with capabilities was found in the Linux kernel’s OverlayFS subsystem in how a user copies a capable file from a nosuid mount into another mount. This uid mapping bug allows a local user to escalate their privileges on the system.

- [https://github.com/karimelsheikh1/HTB-TwoMillion-Writeup](https://github.com/karimelsheikh1/HTB-TwoMillion-Writeup) :  ![starts](https://img.shields.io/github/stars/karimelsheikh1/HTB-TwoMillion-Writeup.svg) ![forks](https://img.shields.io/github/forks/karimelsheikh1/HTB-TwoMillion-Writeup.svg)


## CVE-2022-42889
 Apache Commons Text performs variable interpolation, allowing properties to be dynamically evaluated and expanded. The standard format for interpolation is "${prefix:name}", where "prefix" is used to locate an instance of org.apache.commons.text.lookup.StringLookup that performs the interpolation. Starting with version 1.5 and continuing through 1.9, the set of default Lookup instances included interpolators that could result in arbitrary code execution or contact with remote servers. These lookups are: - "script" - execute expressions using the JVM script execution engine (javax.script) - "dns" - resolve dns records - "url" - load values from urls, including from remote servers Applications using the interpolation defaults in the affected versions may be vulnerable to remote code execution or unintentional contact with remote servers if untrusted configuration values are used. Users are recommended to upgrade to Apache Commons Text 1.10.0, which disables the problematic interpolators by default.

- [https://github.com/alebrestado/CVE-2022-42889-Text4Shell-POC](https://github.com/alebrestado/CVE-2022-42889-Text4Shell-POC) :  ![starts](https://img.shields.io/github/stars/alebrestado/CVE-2022-42889-Text4Shell-POC.svg) ![forks](https://img.shields.io/github/forks/alebrestado/CVE-2022-42889-Text4Shell-POC.svg)


## CVE-2022-31890
 SQL Injection vulnerability in audit/class.audit.php in osTicket osTicket-plugins before commit a7842d494889fd5533d13deb3c6a7789768795ae via the order parameter to the getOrder function.

- [https://github.com/reewardius/CVE-2022-31890](https://github.com/reewardius/CVE-2022-31890) :  ![starts](https://img.shields.io/github/stars/reewardius/CVE-2022-31890.svg) ![forks](https://img.shields.io/github/forks/reewardius/CVE-2022-31890.svg)


## CVE-2022-27434
 UNIT4 TETA Mobile Edition (ME) before 29.5.HF17 was discovered to contain a SQL injection vulnerability via the ProfileName parameter in the errorReporting page.

- [https://github.com/LongWayHomie/CVE-2022-27434](https://github.com/LongWayHomie/CVE-2022-27434) :  ![starts](https://img.shields.io/github/stars/LongWayHomie/CVE-2022-27434.svg) ![forks](https://img.shields.io/github/forks/LongWayHomie/CVE-2022-27434.svg)


## CVE-2021-43936
 The software allows the attacker to upload or transfer files of dangerous types to the WebHMI portal, that may be automatically processed within the product's environment or lead to arbitrary code execution.

- [https://github.com/LongWayHomie/CVE-2021-43936](https://github.com/LongWayHomie/CVE-2021-43936) :  ![starts](https://img.shields.io/github/stars/LongWayHomie/CVE-2021-43936.svg) ![forks](https://img.shields.io/github/forks/LongWayHomie/CVE-2021-43936.svg)


## CVE-2021-43857
 Gerapy is a distributed crawler management framework. Gerapy prior to version 0.9.8 is vulnerable to remote code execution, and this issue is patched in version 0.9.8.

- [https://github.com/LongWayHomie/CVE-2021-43857](https://github.com/LongWayHomie/CVE-2021-43857) :  ![starts](https://img.shields.io/github/stars/LongWayHomie/CVE-2021-43857.svg) ![forks](https://img.shields.io/github/forks/LongWayHomie/CVE-2021-43857.svg)


## CVE-2021-43798
 Grafana is an open-source platform for monitoring and observability. Grafana versions 8.0.0-beta1 through 8.3.0 (except for patched versions) iss vulnerable to directory traversal, allowing access to local files. The vulnerable URL path is: `grafana_host_url/public/plugins//`, where is the plugin ID for any installed plugin. At no time has Grafana Cloud been vulnerable. Users are advised to upgrade to patched versions 8.0.7, 8.1.8, 8.2.7, or 8.3.1. The GitHub Security Advisory contains more information about vulnerable URL paths, mitigation, and the disclosure timeline.

- [https://github.com/LongWayHomie/CVE-2021-43798](https://github.com/LongWayHomie/CVE-2021-43798) :  ![starts](https://img.shields.io/github/stars/LongWayHomie/CVE-2021-43798.svg) ![forks](https://img.shields.io/github/forks/LongWayHomie/CVE-2021-43798.svg)


## CVE-2019-13292
 A SQL Injection issue was discovered in webERP 4.15. Payments.php accepts payment data in base64 format. After this is decoded, it is deserialized. Then, this deserialized data goes directly into a SQL query, with no sanitizing checks.

- [https://github.com/alealeluyah/CVE-2019-13292-WebERP_4.15](https://github.com/alealeluyah/CVE-2019-13292-WebERP_4.15) :  ![starts](https://img.shields.io/github/stars/alealeluyah/CVE-2019-13292-WebERP_4.15.svg) ![forks](https://img.shields.io/github/forks/alealeluyah/CVE-2019-13292-WebERP_4.15.svg)


## CVE-2019-7609
 Kibana versions before 5.6.15 and 6.6.1 contain an arbitrary code execution flaw in the Timelion visualizer. An attacker with access to the Timelion application could send a request that will attempt to execute javascript code. This could possibly lead to an attacker executing arbitrary commands with permissions of the Kibana process on the host system.

- [https://github.com/toxxxaka/CVE-2019-7609](https://github.com/toxxxaka/CVE-2019-7609) :  ![starts](https://img.shields.io/github/stars/toxxxaka/CVE-2019-7609.svg) ![forks](https://img.shields.io/github/forks/toxxxaka/CVE-2019-7609.svg)


## CVE-2018-9276
 An issue was discovered in PRTG Network Monitor before 18.2.39. An attacker who has access to the PRTG System Administrator web console with administrative privileges can exploit an OS command injection vulnerability (both on the server and on devices) by sending malformed parameters in sensor or notification management scenarios.

- [https://github.com/alvinsmith-eroad/CVE-2018-9276](https://github.com/alvinsmith-eroad/CVE-2018-9276) :  ![starts](https://img.shields.io/github/stars/alvinsmith-eroad/CVE-2018-9276.svg) ![forks](https://img.shields.io/github/forks/alvinsmith-eroad/CVE-2018-9276.svg)


## CVE-2017-1000486
 Primetek Primefaces 5.x is vulnerable to a weak encryption flaw resulting in remote code execution

- [https://github.com/LongWayHomie/CVE-2017-1000486](https://github.com/LongWayHomie/CVE-2017-1000486) :  ![starts](https://img.shields.io/github/stars/LongWayHomie/CVE-2017-1000486.svg) ![forks](https://img.shields.io/github/forks/LongWayHomie/CVE-2017-1000486.svg)


## CVE-2017-12617
 When running Apache Tomcat versions 9.0.0.M1 to 9.0.0, 8.5.0 to 8.5.22, 8.0.0.RC1 to 8.0.46 and 7.0.0 to 7.0.81 with HTTP PUTs enabled (e.g. via setting the readonly initialisation parameter of the Default servlet to false) it was possible to upload a JSP file to the server via a specially crafted request. This JSP could then be requested and any code it contained would be executed by the server.

- [https://github.com/LongWayHomie/CVE-2017-12617](https://github.com/LongWayHomie/CVE-2017-12617) :  ![starts](https://img.shields.io/github/stars/LongWayHomie/CVE-2017-12617.svg) ![forks](https://img.shields.io/github/forks/LongWayHomie/CVE-2017-12617.svg)


## CVE-2017-0144
 The SMBv1 server in Microsoft Windows Vista SP2; Windows Server 2008 SP2 and R2 SP1; Windows 7 SP1; Windows 8.1; Windows Server 2012 Gold and R2; Windows RT 8.1; and Windows 10 Gold, 1511, and 1607; and Windows Server 2016 allows remote attackers to execute arbitrary code via crafted packets, aka "Windows SMB Remote Code Execution Vulnerability." This vulnerability is different from those described in CVE-2017-0143, CVE-2017-0145, CVE-2017-0146, and CVE-2017-0148.

- [https://github.com/dannic145/EternalBlue-Exploit-Demonstration](https://github.com/dannic145/EternalBlue-Exploit-Demonstration) :  ![starts](https://img.shields.io/github/stars/dannic145/EternalBlue-Exploit-Demonstration.svg) ![forks](https://img.shields.io/github/forks/dannic145/EternalBlue-Exploit-Demonstration.svg)
- [https://github.com/ichhyak22/EternalBlue-Exploit-Demonstration-MS17-010](https://github.com/ichhyak22/EternalBlue-Exploit-Demonstration-MS17-010) :  ![starts](https://img.shields.io/github/stars/ichhyak22/EternalBlue-Exploit-Demonstration-MS17-010.svg) ![forks](https://img.shields.io/github/forks/ichhyak22/EternalBlue-Exploit-Demonstration-MS17-010.svg)


## CVE-2016-10924
 The ebook-download plugin before 1.2 for WordPress has directory traversal.

- [https://github.com/alealeluyah/cve-2016-10924-POC](https://github.com/alealeluyah/cve-2016-10924-POC) :  ![starts](https://img.shields.io/github/stars/alealeluyah/cve-2016-10924-POC.svg) ![forks](https://img.shields.io/github/forks/alealeluyah/cve-2016-10924-POC.svg)


## CVE-2014-6271
 GNU Bash through 4.3 processes trailing strings after function definitions in the values of environment variables, which allows remote attackers to execute arbitrary code via a crafted environment, as demonstrated by vectors involving the ForceCommand feature in OpenSSH sshd, the mod_cgi and mod_cgid modules in the Apache HTTP Server, scripts executed by unspecified DHCP clients, and other situations in which setting the environment occurs across a privilege boundary from Bash execution, aka "ShellShock."  NOTE: the original fix for this issue was incorrect; CVE-2014-7169 has been assigned to cover the vulnerability that is still present after the incorrect fix.

- [https://github.com/im2nerd/CVE-2014-6271](https://github.com/im2nerd/CVE-2014-6271) :  ![starts](https://img.shields.io/github/stars/im2nerd/CVE-2014-6271.svg) ![forks](https://img.shields.io/github/forks/im2nerd/CVE-2014-6271.svg)

