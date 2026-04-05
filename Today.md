# Update 2026-04-05
## CVE-2026-34838
 Group-Office is an enterprise customer relationship management and groupware tool. Prior to versions 6.8.156, 25.0.90, and 26.0.12, a vulnerability in the AbstractSettingsCollection model leads to insecure deserialization when these settings are loaded. By injecting a serialized FileCookieJar object into a setting string, an authenticated attacker can achieve Arbitrary File Write, leading directly to Remote Code Execution (RCE) on the server. This issue has been patched in versions 6.8.156, 25.0.90, and 26.0.12.

- [https://github.com/bamuwe/CVE-2026-34838](https://github.com/bamuwe/CVE-2026-34838) :  ![starts](https://img.shields.io/github/stars/bamuwe/CVE-2026-34838.svg) ![forks](https://img.shields.io/github/forks/bamuwe/CVE-2026-34838.svg)


## CVE-2026-34156
 NocoBase is an AI-powered no-code/low-code platform for building business applications and enterprise solutions. Prior to version 2.0.28, NocoBase's Workflow Script Node executes user-supplied JavaScript inside a Node.js vm sandbox with a custom require allowlist (controlled by WORKFLOW_SCRIPT_MODULES env var). However, the console object passed into the sandbox context exposes host-realm WritableWorkerStdio stream objects via console._stdout and console._stderr. An authenticated attacker can traverse the prototype chain to escape the sandbox and achieve Remote Code Execution as root. This issue has been patched in version 2.0.28.

- [https://github.com/0xBlackash/CVE-2026-34156](https://github.com/0xBlackash/CVE-2026-34156) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-34156.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-34156.svg)


## CVE-2026-33310
 Intake is a package for finding, investigating, loading and disseminating data. Prior to version 2.0.9, the shell() syntax within parameter default values appears to be automatically expanded during the catalog parsing process. If a catalog contains a parameter default such as shell(command), the command may be executed when the catalog source is accessed. This means that if a user loads a malicious catalog YAML, embedded commands could execute on the host system. Version 2.0.9 mitigates the issue by making getshell False by default everywhere.

- [https://github.com/redyank/CVE-2026-33310](https://github.com/redyank/CVE-2026-33310) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-33310.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-33310.svg)


## CVE-2026-33154
 dynaconf is a configuration management tool for Python. Prior to version 3.2.13, Dynaconf is vulnerable to Server-Side Template Injection (SSTI) due to unsafe template evaluation in the @Jinja resolver. When the jinja2 package is installed, Dynaconf evaluates template expressions embedded in configuration values without a sandboxed environment. This issue has been patched in version 3.2.13.

- [https://github.com/redyank/CVE-2026-33154](https://github.com/redyank/CVE-2026-33154) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-33154.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-33154.svg)


## CVE-2026-33149
 Tandoor Recipes is an application for managing recipes, planning meals, and building shopping lists. Versions up to and including 2.5.3 set ALLOWED_HOSTS = '*' by default, which causes Django to accept any value in the HTTP Host header without validation. The application uses request.build_absolute_uri() to generate absolute URLs in multiple contexts, including invite link emails, API pagination, and OpenAPI schema generation. An attacker who can send requests to the application with a crafted Host header can manipulate all server-generated absolute URLs. The most critical impact is invite link poisoning: when an admin creates an invite and the application sends the invite email, the link points to the attacker's server instead of the real application. When the victim clicks the link, the invite token is sent to the attacker, who can then use it at the real application. As of time of publication, it is unknown if a patched version is available.

- [https://github.com/FilipeGaudard/CVE-2026-33149-PoC](https://github.com/FilipeGaudard/CVE-2026-33149-PoC) :  ![starts](https://img.shields.io/github/stars/FilipeGaudard/CVE-2026-33149-PoC.svg) ![forks](https://img.shields.io/github/forks/FilipeGaudard/CVE-2026-33149-PoC.svg)


## CVE-2026-33147
 GMT is an open source collection of command-line tools for manipulating geographic and Cartesian data sets. In versions from 6.6.0 and prior, a stack-based buffer overflow vulnerability was identified in the gmt_remote_dataset_id function within src/gmt_remote.c. This issue occurs when a specially crafted long string is passed as a dataset identifier (e.g., via the which module), leading to a crash or potential arbitrary code execution. This issue has been patched via commit 0ad2b49.

- [https://github.com/redyank/CVE-2026-33147](https://github.com/redyank/CVE-2026-33147) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-33147.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-33147.svg)


## CVE-2026-33032
 Nginx UI is a web user interface for the Nginx web server. In versions 2.3.5 and prior, the nginx-ui MCP (Model Context Protocol) integration exposes two HTTP endpoints: /mcp and /mcp_message. While /mcp requires both IP whitelisting and authentication (AuthRequired() middleware), the /mcp_message endpoint only applies IP whitelisting - and the default IP whitelist is empty, which the middleware treats as "allow all". This means any network attacker can invoke all MCP tools without authentication, including restarting nginx, creating/modifying/deleting nginx configuration files, and triggering automatic config reloads - achieving complete nginx service takeover. At time of publication, there are no publicly available patches.

- [https://github.com/Twinson333/cve-2026-33032-scanner](https://github.com/Twinson333/cve-2026-33032-scanner) :  ![starts](https://img.shields.io/github/stars/Twinson333/cve-2026-33032-scanner.svg) ![forks](https://img.shields.io/github/forks/Twinson333/cve-2026-33032-scanner.svg)


## CVE-2026-32662
 Development and test API endpoints are present that mirror production functionality.

- [https://github.com/MichaelAdamGroberman/CVE-2026-32662](https://github.com/MichaelAdamGroberman/CVE-2026-32662) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-32662.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-32662.svg)
- [https://github.com/MichaelAdamGroberman/ICSA-26-055-03](https://github.com/MichaelAdamGroberman/ICSA-26-055-03) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/ICSA-26-055-03.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/ICSA-26-055-03.svg)


## CVE-2026-32646
 A specific administrative endpoint is accessible without proper authentication, exposing device management functions.

- [https://github.com/MichaelAdamGroberman/CVE-2026-32646](https://github.com/MichaelAdamGroberman/CVE-2026-32646) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-32646.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-32646.svg)
- [https://github.com/MichaelAdamGroberman/ICSA-26-055-03](https://github.com/MichaelAdamGroberman/ICSA-26-055-03) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/ICSA-26-055-03.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/ICSA-26-055-03.svg)


## CVE-2026-29000
 pac4j-jwt versions prior to 4.5.9, 5.7.9, and 6.3.3 contain an authentication bypass vulnerability in JwtAuthenticator when processing encrypted JWTs that allows remote attackers to forge authentication tokens. Attackers who possess the server's RSA public key can create a JWE-wrapped PlainJWT with arbitrary subject and role claims, bypassing signature verification to authenticate as any user including administrators.

- [https://github.com/yasirr10/CVE-2026-29000](https://github.com/yasirr10/CVE-2026-29000) :  ![starts](https://img.shields.io/github/stars/yasirr10/CVE-2026-29000.svg) ![forks](https://img.shields.io/github/forks/yasirr10/CVE-2026-29000.svg)


## CVE-2026-28767
 A specific administrative endpoint notifications is accessible without proper authentication.

- [https://github.com/MichaelAdamGroberman/CVE-2026-28767](https://github.com/MichaelAdamGroberman/CVE-2026-28767) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-28767.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-28767.svg)
- [https://github.com/MichaelAdamGroberman/ICSA-26-055-03](https://github.com/MichaelAdamGroberman/ICSA-26-055-03) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/ICSA-26-055-03.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/ICSA-26-055-03.svg)


## CVE-2026-28766
 A specific endpoint exposes all user account information for registered Gardyn users without requiring authentication.

- [https://github.com/MichaelAdamGroberman/CVE-2026-28766](https://github.com/MichaelAdamGroberman/CVE-2026-28766) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-28766.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-28766.svg)
- [https://github.com/MichaelAdamGroberman/ICSA-26-055-03](https://github.com/MichaelAdamGroberman/ICSA-26-055-03) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/ICSA-26-055-03.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/ICSA-26-055-03.svg)


## CVE-2026-25197
 A specific endpoint allows authenticated users to pivot to other user profiles by modifying the id number in the API call.

- [https://github.com/MichaelAdamGroberman/CVE-2026-25197](https://github.com/MichaelAdamGroberman/CVE-2026-25197) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-25197.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-25197.svg)
- [https://github.com/MichaelAdamGroberman/ICSA-26-055-03](https://github.com/MichaelAdamGroberman/ICSA-26-055-03) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/ICSA-26-055-03.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/ICSA-26-055-03.svg)


## CVE-2026-24516
 A command injection vulnerability exists in DigitalOcean Droplet Agent through 1.3.2. The troubleshooting actioner component (internal/troubleshooting/actioner/actioner.go) processes metadata from the metadata service endpoint and executes commands specified in the TroubleshootingAgent.Requesting array without adequate input validation. While the code validates that artifacts exist in the validInvestigationArtifacts map, it fails to sanitize the actual command content after the "command:" prefix. This allows an attacker who can control metadata responses to inject and execute arbitrary OS commands with root privileges. The attack is triggered by sending a TCP packet with specific sequence numbers to the SSH port, which causes the agent to fetch metadata from http://169.254.169.254/metadata/v1.json. The vulnerability affects the command execution flow in internal/troubleshooting/actioner/actioner.go (insufficient validation), internal/troubleshooting/command/exec.go (direct exec.CommandContext call), and internal/troubleshooting/command/command.go (command parsing without sanitization). This can lead to complete system compromise, data exfiltration, privilege escalation, and potential lateral movement across cloud infrastructure.

- [https://github.com/poxsky/CVE-2026-24516-DigitalOcean-RCE.](https://github.com/poxsky/CVE-2026-24516-DigitalOcean-RCE.) :  ![starts](https://img.shields.io/github/stars/poxsky/CVE-2026-24516-DigitalOcean-RCE..svg) ![forks](https://img.shields.io/github/forks/poxsky/CVE-2026-24516-DigitalOcean-RCE..svg)


## CVE-2026-22738
This issue affects Spring AI: from 1.0.0 before 1.0.5, from 1.1.0 before 1.1.4.

- [https://github.com/rockmelodies/CVE-2026-22738](https://github.com/rockmelodies/CVE-2026-22738) :  ![starts](https://img.shields.io/github/stars/rockmelodies/CVE-2026-22738.svg) ![forks](https://img.shields.io/github/forks/rockmelodies/CVE-2026-22738.svg)


## CVE-2026-5147
 A security flaw has been discovered in YunaiV yudao-cloud up to 2026.01. This affects an unknown part of the file /admin-api/system/tenant/get-by-website. The manipulation of the argument Website results in sql injection. It is possible to launch the attack remotely. The exploit has been released to the public and may be used for attacks. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/lan1oc/cve-2026-5147-exp](https://github.com/lan1oc/cve-2026-5147-exp) :  ![starts](https://img.shields.io/github/stars/lan1oc/cve-2026-5147-exp.svg) ![forks](https://img.shields.io/github/forks/lan1oc/cve-2026-5147-exp.svg)


## CVE-2026-5027
 The 'POST /api/v2/files' endpoint does not sanitize the 'filename' parameter from the multipart form data, allowing an attacker to write files to arbitrary locations on the filesystem using path traversal sequences ('../').

- [https://github.com/0xBlackash/CVE-2026-5027](https://github.com/0xBlackash/CVE-2026-5027) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-5027.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-5027.svg)
- [https://github.com/min8282/CVE-2026-5027](https://github.com/min8282/CVE-2026-5027) :  ![starts](https://img.shields.io/github/stars/min8282/CVE-2026-5027.svg) ![forks](https://img.shields.io/github/forks/min8282/CVE-2026-5027.svg)
- [https://github.com/EQSTLab/CVE-2026-5027](https://github.com/EQSTLab/CVE-2026-5027) :  ![starts](https://img.shields.io/github/stars/EQSTLab/CVE-2026-5027.svg) ![forks](https://img.shields.io/github/forks/EQSTLab/CVE-2026-5027.svg)


## CVE-2026-2991
 The KiviCare – Clinic & Patient Management System (EHR) plugin for WordPress is vulnerable to Authentication Bypass in all versions up to, and including, 4.1.2. This is due to the `patientSocialLogin()` function not verifying the social provider access token before authenticating a user. This makes it possible for unauthenticated attackers to log in as any patient registered on the system by providing only their email address and an arbitrary value for the access token, bypassing all credential verification. The attacker gains access to sensitive medical records, appointments, prescriptions, and billing information (PII/PHI breach). Additionally, authentication cookies are set before the role check, meaning the auth cookies for non-patient users (including administrators) are also set in the HTTP response headers, even though a 403 response is returned.

- [https://github.com/Jumpthereness578/CVE-2026-2991](https://github.com/Jumpthereness578/CVE-2026-2991) :  ![starts](https://img.shields.io/github/stars/Jumpthereness578/CVE-2026-2991.svg) ![forks](https://img.shields.io/github/forks/Jumpthereness578/CVE-2026-2991.svg)


## CVE-2026-0770
The specific flaw exists within the handling of the exec_globals parameter provided to the validate endpoint. The issue results from the inclusion of a resource from an untrusted control sphere. An attacker can leverage this vulnerability to execute code in the context of root. Was ZDI-CAN-27325.

- [https://github.com/0xBlackash/CVE-2026-0770](https://github.com/0xBlackash/CVE-2026-0770) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-0770.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-0770.svg)


## CVE-2025-59059
Users are recommended to upgrade to version 2.8.0, which fixes this issue.

- [https://github.com/pl4tyz/CVE-2025-59059-Misattributed-RCE-in-Apache-Ranger-Static-Analysis-Correction](https://github.com/pl4tyz/CVE-2025-59059-Misattributed-RCE-in-Apache-Ranger-Static-Analysis-Correction) :  ![starts](https://img.shields.io/github/stars/pl4tyz/CVE-2025-59059-Misattributed-RCE-in-Apache-Ranger-Static-Analysis-Correction.svg) ![forks](https://img.shields.io/github/forks/pl4tyz/CVE-2025-59059-Misattributed-RCE-in-Apache-Ranger-Static-Analysis-Correction.svg)


## CVE-2025-54236
 Adobe Commerce versions 2.4.9-alpha2, 2.4.8-p2, 2.4.7-p7, 2.4.6-p12, 2.4.5-p14, 2.4.4-p15 and earlier are affected by an Improper Input Validation vulnerability. A successful attacker can abuse this to achieve session takeover, increasing the confidentiality, and integrity impact to high. Exploitation of this issue does not require user interaction.

- [https://github.com/qoliber/magento-open-source-security](https://github.com/qoliber/magento-open-source-security) :  ![starts](https://img.shields.io/github/stars/qoliber/magento-open-source-security.svg) ![forks](https://img.shields.io/github/forks/qoliber/magento-open-source-security.svg)


## CVE-2025-32957
 baserCMS is a website development framework. Prior to version 5.2.3, the application's restore function allows users to upload a .zip file, which is then automatically extracted. A PHP file inside the archive is included using require_once without validating or restricting the filename. An attacker can craft a malicious PHP file within the zip and achieve arbitrary code execution when it is included. This issue has been patched in version 5.2.3.

- [https://github.com/toratako/CVE-2025-32957-PoC](https://github.com/toratako/CVE-2025-32957-PoC) :  ![starts](https://img.shields.io/github/stars/toratako/CVE-2025-32957-PoC.svg) ![forks](https://img.shields.io/github/forks/toratako/CVE-2025-32957-PoC.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/elshaheedy/CVE-2025-29927-Sigma-Rule](https://github.com/elshaheedy/CVE-2025-29927-Sigma-Rule) :  ![starts](https://img.shields.io/github/stars/elshaheedy/CVE-2025-29927-Sigma-Rule.svg) ![forks](https://img.shields.io/github/forks/elshaheedy/CVE-2025-29927-Sigma-Rule.svg)
- [https://github.com/hujiaozhuzhu/CVE-2025-29927__Next.js](https://github.com/hujiaozhuzhu/CVE-2025-29927__Next.js) :  ![starts](https://img.shields.io/github/stars/hujiaozhuzhu/CVE-2025-29927__Next.js.svg) ![forks](https://img.shields.io/github/forks/hujiaozhuzhu/CVE-2025-29927__Next.js.svg)


## CVE-2025-24257
 An out-of-bounds write issue was addressed with improved input validation. This issue is fixed in iOS 18.4 and iPadOS 18.4, macOS Sequoia 15.4, visionOS 2.4, watchOS 11.4. An app may be able to cause unexpected system termination or write kernel memory.

- [https://github.com/Learningdisordercapital35/CVE_2025_24257----NOT-MINE](https://github.com/Learningdisordercapital35/CVE_2025_24257----NOT-MINE) :  ![starts](https://img.shields.io/github/stars/Learningdisordercapital35/CVE_2025_24257----NOT-MINE.svg) ![forks](https://img.shields.io/github/forks/Learningdisordercapital35/CVE_2025_24257----NOT-MINE.svg)


## CVE-2025-24054
 External control of file name or path in Windows NTLM allows an unauthorized attacker to perform spoofing over a network.

- [https://github.com/kaleth4/CVE--2025-24054](https://github.com/kaleth4/CVE--2025-24054) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE--2025-24054.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE--2025-24054.svg)


## CVE-2025-23970
 Incorrect Privilege Assignment vulnerability in aonetheme Service Finder Booking sf-booking allows Privilege Escalation.This issue affects Service Finder Booking: from n/a through = 6.1.

- [https://github.com/PegasusMetaSec/PEGASUS-CVE-2025-23970](https://github.com/PegasusMetaSec/PEGASUS-CVE-2025-23970) :  ![starts](https://img.shields.io/github/stars/PegasusMetaSec/PEGASUS-CVE-2025-23970.svg) ![forks](https://img.shields.io/github/forks/PegasusMetaSec/PEGASUS-CVE-2025-23970.svg)


## CVE-2025-10681
 Storage credentials are hardcoded in the mobile app and device firmware. These credentials do not adequately limit end user permissions and do not expire within a reasonable amount of time. This vulnerability may grant unauthorized access to production storage containers.

- [https://github.com/MichaelAdamGroberman/CVE-2025-10681](https://github.com/MichaelAdamGroberman/CVE-2025-10681) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2025-10681.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2025-10681.svg)
- [https://github.com/MichaelAdamGroberman/ICSA-26-055-03](https://github.com/MichaelAdamGroberman/ICSA-26-055-03) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/ICSA-26-055-03.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/ICSA-26-055-03.svg)


## CVE-2024-2370
 DO NOT USE THIS CVE ID NUMBER. Consult IDs: CVE-2018-5341. Reason: This CVE Record is a duplicate of CVE-2018-5341. Notes: All CVE users should reference CVE-2018-5341 instead of this record.

- [https://github.com/kaitokidc500/CVE-2024-23700-C2-Server](https://github.com/kaitokidc500/CVE-2024-23700-C2-Server) :  ![starts](https://img.shields.io/github/stars/kaitokidc500/CVE-2024-23700-C2-Server.svg) ![forks](https://img.shields.io/github/forks/kaitokidc500/CVE-2024-23700-C2-Server.svg)


## CVE-2022-46364
 A SSRF vulnerability in parsing the href attribute of XOP:Include in MTOM requests in versions of Apache CXF before 3.5.5 and 3.4.10 allows an attacker to perform SSRF style attacks on webservices that take at least one parameter of any type. 

- [https://github.com/jwsly12/CVE-2022-46364-htb-ctf](https://github.com/jwsly12/CVE-2022-46364-htb-ctf) :  ![starts](https://img.shields.io/github/stars/jwsly12/CVE-2022-46364-htb-ctf.svg) ![forks](https://img.shields.io/github/forks/jwsly12/CVE-2022-46364-htb-ctf.svg)


## CVE-2022-46363
 A vulnerability in Apache CXF before versions 3.5.5 and 3.4.10 allows an attacker to perform a remote directory listing or code exfiltration. The vulnerability only applies when the CXFServlet is configured with both the static-resources-list and redirect-query-check attributes. These attributes are not supposed to be used together, and so the vulnerability can only arise if the CXF service is misconfigured.

- [https://github.com/jwsly12/CVE-2022-46364-htb-ctf](https://github.com/jwsly12/CVE-2022-46364-htb-ctf) :  ![starts](https://img.shields.io/github/stars/jwsly12/CVE-2022-46364-htb-ctf.svg) ![forks](https://img.shields.io/github/forks/jwsly12/CVE-2022-46364-htb-ctf.svg)


## CVE-2022-30075
 In TP-Link Router AX50 firmware 210730 and older, import of a malicious backup file via web interface can lead to remote code execution due to improper validation.

- [https://github.com/RhestCorp/TP-L-NK-SIZMA-EXPLO-T](https://github.com/RhestCorp/TP-L-NK-SIZMA-EXPLO-T) :  ![starts](https://img.shields.io/github/stars/RhestCorp/TP-L-NK-SIZMA-EXPLO-T.svg) ![forks](https://img.shields.io/github/forks/RhestCorp/TP-L-NK-SIZMA-EXPLO-T.svg)


## CVE-2019-6225
 A memory corruption issue was addressed with improved validation. This issue is fixed in iOS 12.1.3, macOS Mojave 10.14.3, tvOS 12.1.2. A malicious application may be able to elevate privileges.

- [https://github.com/ox1111/jailbreak-iOS12](https://github.com/ox1111/jailbreak-iOS12) :  ![starts](https://img.shields.io/github/stars/ox1111/jailbreak-iOS12.svg) ![forks](https://img.shields.io/github/forks/ox1111/jailbreak-iOS12.svg)


## CVE-2019-2215
 A use-after-free in binder.c allows an elevation of privilege from an application to the Linux Kernel. No user interaction is required to exploit this vulnerability, however exploitation does require either the installation of a malicious local application or a separate vulnerability in a network facing application.Product: AndroidAndroid ID: A-141720095

- [https://github.com/codecat007/CVE-2019-2215](https://github.com/codecat007/CVE-2019-2215) :  ![starts](https://img.shields.io/github/stars/codecat007/CVE-2019-2215.svg) ![forks](https://img.shields.io/github/forks/codecat007/CVE-2019-2215.svg)

