# Update 2026-04-18
## CVE-2026-40261
 Composer is a dependency manager for PHP. Versions 1.0 through 2.2.26 and 2.3 through 2.9.5 contain a command injection vulnerability in the Perforce::syncCodeBase() method, which appends the $sourceReference parameter to a shell command without proper escaping, and additionally in the Perforce::generateP4Command() method as in GHSA-wg36-wvj6-r67p / CVE-2026-40176, which interpolates user-supplied Perforce connection parameters (port, user, client) from the source url field without proper escaping. An attacker can inject arbitrary commands through crafted source reference or source url values containing shell metacharacters, even if Perforce is not installed. Unlike CVE-2026-40176, the source reference and url are provided as part of package metadata, meaning any compromised or malicious Composer repository can serve package metadata declaring perforce as a source type with malicious values. This vulnerability is exploitable when installing or updating dependencies from source, including the default behavior when installing dev-prefixed versions. This issue has been fixed in Composer 2.2.27 (2.2 LTS) and 2.9.6 (mainline). If developers are unable to immediately update, they can avoid installing dependencies from source by using --prefer-dist or the preferred-install: dist config setting, and only use trusted Composer repositories as a workaround.

- [https://github.com/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC](https://github.com/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC) :  ![starts](https://img.shields.io/github/stars/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC.svg) ![forks](https://img.shields.io/github/forks/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC.svg)


## CVE-2026-40176
 Composer is a dependency manager for PHP. Versions 1.0 through 2.2.26 and 2.3 through 2.9.5 contain a command injection vulnerability in the Perforce::generateP4Command() method, which constructs shell commands by interpolating user-supplied Perforce connection parameters (port, user, client) without proper escaping. An attacker can inject arbitrary commands through these values in a malicious composer.json declaring a Perforce VCS repository, leading to command execution in the context of the user running Composer, even if Perforce is not installed. VCS repositories are only loaded from the root composer.json or the composer config directory, so this cannot be exploited through composer.json files of packages installed as dependencies. Users are at risk if they run Composer commands on untrusted projects with attacker-supplied composer.json files. This issue has been fixed in Composer 2.2.27 (2.2 LTS) and 2.9.6 (mainline).

- [https://github.com/Saku0512/CVE-2026-40176-poc](https://github.com/Saku0512/CVE-2026-40176-poc) :  ![starts](https://img.shields.io/github/stars/Saku0512/CVE-2026-40176-poc.svg) ![forks](https://img.shields.io/github/forks/Saku0512/CVE-2026-40176-poc.svg)
- [https://github.com/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC](https://github.com/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC) :  ![starts](https://img.shields.io/github/stars/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC.svg) ![forks](https://img.shields.io/github/forks/terminat0r7031/composer-CVE-2026-40261-CVE-2026-40176-PoC.svg)


## CVE-2026-34486
Users are recommended to upgrade to version 11.0.21, 10.1.54 or 9.0.117, which fix the issue.

- [https://github.com/helGayhub233/CVE-2026-34486-Tribes](https://github.com/helGayhub233/CVE-2026-34486-Tribes) :  ![starts](https://img.shields.io/github/stars/helGayhub233/CVE-2026-34486-Tribes.svg) ![forks](https://img.shields.io/github/forks/helGayhub233/CVE-2026-34486-Tribes.svg)


## CVE-2026-34220
 MikroORM is a TypeScript ORM for Node.js based on Data Mapper, Unit of Work and Identity Map patterns. Prior to versions 6.6.10 and 7.0.6, there is a SQL injection vulnerability when specially crafted objects are interpreted as raw SQL query fragments. This issue has been patched in versions 6.6.10 and 7.0.6.

- [https://github.com/EQSTLab/CVE-2026-34220](https://github.com/EQSTLab/CVE-2026-34220) :  ![starts](https://img.shields.io/github/stars/EQSTLab/CVE-2026-34220.svg) ![forks](https://img.shields.io/github/forks/EQSTLab/CVE-2026-34220.svg)


## CVE-2026-33824
 Double free in Windows IKE Extension allows an unauthorized attacker to execute code over a network.

- [https://github.com/z3r0h3ro/CVE-2026-33824](https://github.com/z3r0h3ro/CVE-2026-33824) :  ![starts](https://img.shields.io/github/stars/z3r0h3ro/CVE-2026-33824.svg) ![forks](https://img.shields.io/github/forks/z3r0h3ro/CVE-2026-33824.svg)


## CVE-2026-33555
 An issue was discovered in HAProxy before 3.3.6. The HTTP/3 parser does not check that the received body length matches a previously announced content-length when the stream is closed via a frame with an empty payload. This can cause desynchronization issues with the backend server and could be used for request smuggling. The earliest affected version is 2.6.

- [https://github.com/r3verii/CVE-2026-33555](https://github.com/r3verii/CVE-2026-33555) :  ![starts](https://img.shields.io/github/stars/r3verii/CVE-2026-33555.svg) ![forks](https://img.shields.io/github/forks/r3verii/CVE-2026-33555.svg)


## CVE-2026-22679
 Weaver (Fanwei) E-cology 10.0 versions prior to 20260312 contain an unauthenticated remote code execution vulnerability in the /papi/esearch/data/devops/dubboApi/debug/method endpoint that allows attackers to execute arbitrary commands by invoking exposed debug functionality. Attackers can craft POST requests with attacker-controlled interfaceName and methodName parameters to reach command-execution helpers and achieve arbitrary command execution on the system. Exploitation evidence was first observed by the Shadowserver Foundation on 2026-03-31 (UTC).

- [https://github.com/keraattin/CVE-2026-22679](https://github.com/keraattin/CVE-2026-22679) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-22679.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-22679.svg)


## CVE-2026-21858
 n8n is an open source workflow automation platform. Versions starting with 1.65.0 and below 1.121.0 enable an attacker to access files on the underlying server through execution of certain form-based workflows. A vulnerable workflow could grant access to an unauthenticated remote attacker, resulting in exposure of sensitive information stored on the system and may enable further compromise depending on deployment configuration and workflow usage. This issue is fixed in version 1.121.0.

- [https://github.com/masterwok/PoC-CVE-2026-21858](https://github.com/masterwok/PoC-CVE-2026-21858) :  ![starts](https://img.shields.io/github/stars/masterwok/PoC-CVE-2026-21858.svg) ![forks](https://img.shields.io/github/forks/masterwok/PoC-CVE-2026-21858.svg)


## CVE-2026-5059
The specific flaw exists within the handling of the allowed commands list. The issue results from the lack of proper validation of a user-supplied string before using it to execute a system call. An attacker can leverage this vulnerability to execute code in the context of the MCP server. Was ZDI-CAN-27969.

- [https://github.com/venom203020/CVE-2026-5059-poc](https://github.com/venom203020/CVE-2026-5059-poc) :  ![starts](https://img.shields.io/github/stars/venom203020/CVE-2026-5059-poc.svg) ![forks](https://img.shields.io/github/forks/venom203020/CVE-2026-5059-poc.svg)


## CVE-2026-3891
 The Pix for WooCommerce plugin for WordPress is vulnerable to arbitrary file uploads due to missing capability check and missing file type validation in the 'lkn_pix_for_woocommerce_c6_save_settings' function in all versions up to, and including, 1.5.0. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/AnggaTechI/Mass-Scanner-CVE-2026-3891](https://github.com/AnggaTechI/Mass-Scanner-CVE-2026-3891) :  ![starts](https://img.shields.io/github/stars/AnggaTechI/Mass-Scanner-CVE-2026-3891.svg) ![forks](https://img.shields.io/github/forks/AnggaTechI/Mass-Scanner-CVE-2026-3891.svg)


## CVE-2026-3786
 A security flaw has been discovered in EasyCMS up to 1.6. The impacted element is an unknown function of the file /RbacuserAction.class.php of the component Request Parameter Handler. The manipulation of the argument _order results in sql injection. The attack can be launched remotely. The exploit has been released to the public and may be used for attacks. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/Mefhika120/CVE-2026-3786](https://github.com/Mefhika120/CVE-2026-3786) :  ![starts](https://img.shields.io/github/stars/Mefhika120/CVE-2026-3786.svg) ![forks](https://img.shields.io/github/forks/Mefhika120/CVE-2026-3786.svg)


## CVE-2026-3775
 The application's update service, when checking for updates, loads certain system libraries from a search path that includes directories writable by low‑privileged users and is not strictly restricted to trusted system locations. Because these libraries may be resolved and loaded from user‑writable locations, a local attacker can place a malicious library there and have it loaded with SYSTEM privileges, resulting in local privilege escalation and arbitrary code execution.

- [https://github.com/menevarad007/CVE-2026-37750](https://github.com/menevarad007/CVE-2026-37750) :  ![starts](https://img.shields.io/github/stars/menevarad007/CVE-2026-37750.svg) ![forks](https://img.shields.io/github/forks/menevarad007/CVE-2026-37750.svg)


## CVE-2026-3774
 The application allows PDF JavaScript and document/print actions (such as WillPrint/DidPrint) to update form fields, annotations, or optional content groups (OCGs) immediately before or after redaction, encryption, or printing. These script‑driven updates are not fully covered by the existing redaction, encryption, and printing logic, which, under specific document structures and user workflows, may cause a small amount of sensitive content to remain unremoved or unencrypted as expected, or result in printed output that slightly differs from what was reviewed on screen.

- [https://github.com/menevarad007/CVE-2026-37748](https://github.com/menevarad007/CVE-2026-37748) :  ![starts](https://img.shields.io/github/stars/menevarad007/CVE-2026-37748.svg) ![forks](https://img.shields.io/github/forks/menevarad007/CVE-2026-37748.svg)
- [https://github.com/menevarad007/CVE-2026-37749](https://github.com/menevarad007/CVE-2026-37749) :  ![starts](https://img.shields.io/github/stars/menevarad007/CVE-2026-37749.svg) ![forks](https://img.shields.io/github/forks/menevarad007/CVE-2026-37749.svg)


## CVE-2026-2749
 Vulnerability in Centreon Centreon Open Tickets on Central Server on Linux (Centroen Open Ticket modules).This issue affects Centreon Open Tickets on Central Server: from all before 25.10.3, 24.10.8, 24.04.7.

- [https://github.com/hakaioffsec/Centreon-Exploits-2026](https://github.com/hakaioffsec/Centreon-Exploits-2026) :  ![starts](https://img.shields.io/github/stars/hakaioffsec/Centreon-Exploits-2026.svg) ![forks](https://img.shields.io/github/forks/hakaioffsec/Centreon-Exploits-2026.svg)


## CVE-2026-1880
Refer to the 'Security Update for ASUS DriverHub' section on the ASUS Security Advisory for more information.

- [https://github.com/seokjohn/CVE-2026-1880](https://github.com/seokjohn/CVE-2026-1880) :  ![starts](https://img.shields.io/github/stars/seokjohn/CVE-2026-1880.svg) ![forks](https://img.shields.io/github/forks/seokjohn/CVE-2026-1880.svg)


## CVE-2026-0827
 During an internal security assessment, a potential vulnerability was discovered in Lenovo Diagnostics and the HardwareScanAddin used in Lenovo Vantage that, during installation or when using hardware scan, could allow a local authenticated user to perform an arbitrary file write with elevated privileges.

- [https://github.com/ZeroMemoryEx/CVE-2026-0827](https://github.com/ZeroMemoryEx/CVE-2026-0827) :  ![starts](https://img.shields.io/github/stars/ZeroMemoryEx/CVE-2026-0827.svg) ![forks](https://img.shields.io/github/forks/ZeroMemoryEx/CVE-2026-0827.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-transitive](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-transitive) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-transitive.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-transitive.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-rsc-webpack](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-rsc-webpack) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-rsc-webpack.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-rsc-webpack.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs.svg)
- [https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478](https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478) :  ![starts](https://img.shields.io/github/stars/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg) ![forks](https://img.shields.io/github/forks/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg)


## CVE-2025-59528
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5, Flowise is vulnerable to remote code execution. The CustomMCP node allows users to input configuration settings for connecting to an external MCP server. This node parses the user-provided mcpServerConfig string to build the MCP server configuration. However, during this process, it executes JavaScript code without any security validation. Specifically, inside the convertToValidJSONString function, user input is directly passed to the Function() constructor, which evaluates and executes the input as JavaScript code. Since this runs with full Node.js runtime privileges, it can access dangerous modules such as child_process and fs. This issue has been patched in version 3.0.6.

- [https://github.com/honney336/CVE-2025-58434_CVE-2025-59528](https://github.com/honney336/CVE-2025-58434_CVE-2025-59528) :  ![starts](https://img.shields.io/github/stars/honney336/CVE-2025-58434_CVE-2025-59528.svg) ![forks](https://img.shields.io/github/forks/honney336/CVE-2025-58434_CVE-2025-59528.svg)


## CVE-2025-58434
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5 and earlier, the `forgot-password` endpoint in Flowise returns sensitive information including a valid password reset `tempToken` without authentication or verification. This enables any attacker to generate a reset token for arbitrary users and directly reset their password, leading to a complete account takeover (ATO). This vulnerability applies to both the cloud service (`cloud.flowiseai.com`) and self-hosted/local Flowise deployments that expose the same API. Commit 9e178d68873eb876073846433a596590d3d9c863 in version 3.0.6 secures password reset endpoints. Several recommended remediation steps are available. Do not return reset tokens or sensitive account details in API responses. Tokens must only be delivered securely via the registered email channel. Ensure `forgot-password` responds with a generic success message regardless of input, to avoid user enumeration. Require strong validation of the `tempToken` (e.g., single-use, short expiry, tied to request origin, validated against email delivery). Apply the same fixes to both cloud and self-hosted/local deployments. Log and monitor password reset requests for suspicious activity. Consider multi-factor verification for sensitive accounts.

- [https://github.com/honney336/CVE-2025-58434_CVE-2025-59528](https://github.com/honney336/CVE-2025-58434_CVE-2025-59528) :  ![starts](https://img.shields.io/github/stars/honney336/CVE-2025-58434_CVE-2025-59528.svg) ![forks](https://img.shields.io/github/forks/honney336/CVE-2025-58434_CVE-2025-59528.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/hujiaozhuzhu/CVE-2025-29927__Next.js](https://github.com/hujiaozhuzhu/CVE-2025-29927__Next.js) :  ![starts](https://img.shields.io/github/stars/hujiaozhuzhu/CVE-2025-29927__Next.js.svg) ![forks](https://img.shields.io/github/forks/hujiaozhuzhu/CVE-2025-29927__Next.js.svg)
- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-24963
 Vitest is a testing framework powered by Vite. The `__screenshot-error` handler on the browser mode HTTP server that responds any file on the file system. Especially if the server is exposed on the network by `browser.api.host: true`, an attacker can send a request to that handler from remote to get the content of arbitrary files.This `__screenshot-error` handler on the browser mode HTTP server responds any file on the file system. This code was added by commit `2d62051`. Users explicitly exposing the browser mode server to the network by `browser.api.host: true` may get any files exposed. This issue has been addressed in versions 2.1.9 and 3.0.4. Users are advised to upgrade. There are no known workarounds for this vulnerability.

- [https://github.com/hiteshpatra/CVE-2025-24963](https://github.com/hiteshpatra/CVE-2025-24963) :  ![starts](https://img.shields.io/github/stars/hiteshpatra/CVE-2025-24963.svg) ![forks](https://img.shields.io/github/forks/hiteshpatra/CVE-2025-24963.svg)


## CVE-2025-15602
 Snipe-IT versions prior to 8.3.7 contain sensitive user attributes related to account privileges that are insufficiently protected against mass assignment. An authenticated, low-privileged user can craft a malicious API request to modify restricted fields of another user account, including the Super Admin account. By changing the email address of the Super Admin and triggering a password reset, an attacker can fully take over the Super Admin account, resulting in complete administrative control of the Snipe-IT instance.

- [https://github.com/Nxvh1337/CVE-2025-15602-PoC](https://github.com/Nxvh1337/CVE-2025-15602-PoC) :  ![starts](https://img.shields.io/github/stars/Nxvh1337/CVE-2025-15602-PoC.svg) ![forks](https://img.shields.io/github/forks/Nxvh1337/CVE-2025-15602-PoC.svg)


## CVE-2025-8110
 Improper Symbolic link handling in the PutContents API in Gogs allows Local Execution of Code.

- [https://github.com/hassan-hamadi/CVE-2025-8110-Silentium-HTB](https://github.com/hassan-hamadi/CVE-2025-8110-Silentium-HTB) :  ![starts](https://img.shields.io/github/stars/hassan-hamadi/CVE-2025-8110-Silentium-HTB.svg) ![forks](https://img.shields.io/github/forks/hassan-hamadi/CVE-2025-8110-Silentium-HTB.svg)


## CVE-2025-7096
 A vulnerability classified as critical was found in Comodo Internet Security Premium 12.3.4.8162. This vulnerability affects unknown code of the file cis_update_x64.xml of the component Manifest File Handler. The manipulation leads to improper validation of integrity check value. The attack can be initiated remotely. The complexity of an attack is rather high. The exploitation appears to be difficult. The exploit has been disclosed to the public and may be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/namaek2/CVE-2025-70962](https://github.com/namaek2/CVE-2025-70962) :  ![starts](https://img.shields.io/github/stars/namaek2/CVE-2025-70962.svg) ![forks](https://img.shields.io/github/forks/namaek2/CVE-2025-70962.svg)


## CVE-2025-6942
 The distributed engine versions 8.4.39.0 and earlier of Secret Server versions 11.7.49 and earlier can be exploited during an initial authorization event that would allow an attacker to impersonate another distributed engine.

- [https://github.com/jasetpen/CVE-2025-69428](https://github.com/jasetpen/CVE-2025-69428) :  ![starts](https://img.shields.io/github/stars/jasetpen/CVE-2025-69428.svg) ![forks](https://img.shields.io/github/forks/jasetpen/CVE-2025-69428.svg)


## CVE-2024-53677
You can find more details in  https://cwiki.apache.org/confluence/display/WW/S2-067

- [https://github.com/hiteshpatra/CVE-2024-53677](https://github.com/hiteshpatra/CVE-2024-53677) :  ![starts](https://img.shields.io/github/stars/hiteshpatra/CVE-2024-53677.svg) ![forks](https://img.shields.io/github/forks/hiteshpatra/CVE-2024-53677.svg)


## CVE-2024-42009
 A Cross-Site Scripting vulnerability in Roundcube through 1.5.7 and 1.6.x through 1.6.7 allows a remote attacker to steal and send emails of a victim via a crafted e-mail message that abuses a Desanitization issue in message_body() in program/actions/mail/show.php.

- [https://github.com/ZaidArif47/CVE-2024-42009](https://github.com/ZaidArif47/CVE-2024-42009) :  ![starts](https://img.shields.io/github/stars/ZaidArif47/CVE-2024-42009.svg) ![forks](https://img.shields.io/github/forks/ZaidArif47/CVE-2024-42009.svg)


## CVE-2024-30088
 Windows Kernel Elevation of Privilege Vulnerability

- [https://github.com/repo4Chu/CVE-2024-30088__Windows-TOCTOU-exploit](https://github.com/repo4Chu/CVE-2024-30088__Windows-TOCTOU-exploit) :  ![starts](https://img.shields.io/github/stars/repo4Chu/CVE-2024-30088__Windows-TOCTOU-exploit.svg) ![forks](https://img.shields.io/github/forks/repo4Chu/CVE-2024-30088__Windows-TOCTOU-exploit.svg)


## CVE-2024-3400
Cloud NGFW, Panorama appliances, and Prisma Access are not impacted by this vulnerability.

- [https://github.com/Zedocun/PAN-OS-CVE-2024-3400-Command-Injection-Investigation](https://github.com/Zedocun/PAN-OS-CVE-2024-3400-Command-Injection-Investigation) :  ![starts](https://img.shields.io/github/stars/Zedocun/PAN-OS-CVE-2024-3400-Command-Injection-Investigation.svg) ![forks](https://img.shields.io/github/forks/Zedocun/PAN-OS-CVE-2024-3400-Command-Injection-Investigation.svg)


## CVE-2023-21036
 In BitmapExport.java, there is a possible failure to truncate images due to a logic error in the code.Product: AndroidVersions: Android kernelAndroid ID: A-264261868References: N/A

- [https://github.com/PolitoInc/XWFAcropalypse](https://github.com/PolitoInc/XWFAcropalypse) :  ![starts](https://img.shields.io/github/stars/PolitoInc/XWFAcropalypse.svg) ![forks](https://img.shields.io/github/forks/PolitoInc/XWFAcropalypse.svg)


## CVE-2018-6892
 An issue was discovered in CloudMe before 1.11.0. An unauthenticated remote attacker that can connect to the "CloudMe Sync" client application listening on port 8888 can send a malicious payload causing a buffer overflow condition. This will result in an attacker controlling the program's execution flow and allowing arbitrary code execution.

- [https://github.com/crypticq/CLOUDME_B0F](https://github.com/crypticq/CLOUDME_B0F) :  ![starts](https://img.shields.io/github/stars/crypticq/CLOUDME_B0F.svg) ![forks](https://img.shields.io/github/forks/crypticq/CLOUDME_B0F.svg)


## CVE-2011-2523
 vsftpd 2.3.4 downloaded between 20110630 and 20110703 contains a backdoor which opens a shell on port 6200/tcp.

- [https://github.com/emilebarnard242/pentest-metasploitable2](https://github.com/emilebarnard242/pentest-metasploitable2) :  ![starts](https://img.shields.io/github/stars/emilebarnard242/pentest-metasploitable2.svg) ![forks](https://img.shields.io/github/forks/emilebarnard242/pentest-metasploitable2.svg)


## CVE-2010-2075
 UnrealIRCd 3.2.8.1, as distributed on certain mirror sites from November 2009 through June 2010, contains an externally introduced modification (Trojan Horse) in the DEBUG3_DOLOG_SYSTEM macro, which allows remote attackers to execute arbitrary commands.

- [https://github.com/Tc-XoNoR/CVE-2010-2075](https://github.com/Tc-XoNoR/CVE-2010-2075) :  ![starts](https://img.shields.io/github/stars/Tc-XoNoR/CVE-2010-2075.svg) ![forks](https://img.shields.io/github/forks/Tc-XoNoR/CVE-2010-2075.svg)

