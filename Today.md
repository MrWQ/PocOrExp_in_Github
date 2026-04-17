# Update 2026-04-17
## CVE-2026-39987
 marimo is a reactive Python notebook. Prior to 0.23.0, Marimo has a Pre-Auth RCE vulnerability. The terminal WebSocket endpoint /terminal/ws lacks authentication validation, allowing an unauthenticated attacker to obtain a full PTY shell and execute arbitrary system commands. Unlike other WebSocket endpoints (e.g., /ws) that correctly call validate_auth() for authentication, the /terminal/ws endpoint only checks the running mode and platform support before accepting connections, completely skipping authentication verification. This vulnerability is fixed in 0.23.0.

- [https://github.com/keraattin/CVE-2026-39987](https://github.com/keraattin/CVE-2026-39987) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-39987.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-39987.svg)


## CVE-2026-39808
 A improper neutralization of special elements used in an os command ('os command injection') vulnerability in Fortinet FortiSandbox 4.4.0 through 4.4.8 may allow attacker to execute unauthorized code or commands via insert attack vector here

- [https://github.com/samu-delucas/CVE-2026-39808](https://github.com/samu-delucas/CVE-2026-39808) :  ![starts](https://img.shields.io/github/stars/samu-delucas/CVE-2026-39808.svg) ![forks](https://img.shields.io/github/forks/samu-delucas/CVE-2026-39808.svg)
- [https://github.com/Lechansky/CVE-2026-39808](https://github.com/Lechansky/CVE-2026-39808) :  ![starts](https://img.shields.io/github/stars/Lechansky/CVE-2026-39808.svg) ![forks](https://img.shields.io/github/forks/Lechansky/CVE-2026-39808.svg)


## CVE-2026-35584
 FreeScout is a free help desk and shared inbox built with PHP's Laravel framework. Prior to 1.8.212, the endpoint GET /thread/read/{conversation_id}/{thread_id} does not require authentication and does not validate whether the given thread_id belongs to the given conversation_id. This allows any unauthenticated attacker to mark any thread as read by passing arbitrary IDs, enumerate valid thread IDs via HTTP response codes (200 vs 404), and manipulate opened_at timestamps across conversations (IDOR). This vulnerability is fixed in 1.8.212.

- [https://github.com/LeonardoNovais7/CVE-2026-35584](https://github.com/LeonardoNovais7/CVE-2026-35584) :  ![starts](https://img.shields.io/github/stars/LeonardoNovais7/CVE-2026-35584.svg) ![forks](https://img.shields.io/github/forks/LeonardoNovais7/CVE-2026-35584.svg)


## CVE-2026-35031
 Jellyfin is an open source self hosted media server. Versions prior to 10.11.7 contain a vulnerability chain in the subtitle upload endpoint (POST /Videos/{itemId}/Subtitles), where the Format field is not validated, allowing path traversal via the file extension and enabling arbitrary file write. This arbitrary file write can be chained into arbitrary file read via .strm files, database extraction, admin privilege escalation, and ultimately remote code execution as root via ld.so.preload. Exploitation requires an administrator account or a user that has been explicitly granted the "Upload Subtitles" permission. This issue has been fixed in version 10.11.7. If users are unable to upgrade immediately, they can grant non-administrator users Subtitle upload permissions to reduce attack surface.

- [https://github.com/keraattin/CVE-2026-35031](https://github.com/keraattin/CVE-2026-35031) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-35031.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-35031.svg)


## CVE-2026-34621
 Acrobat Reader versions 24.001.30356, 26.001.21367 and earlier are affected by an Improperly Controlled Modification of Object Prototype Attributes ('Prototype Pollution') vulnerability that could result in arbitrary code execution in the context of the current user. Exploitation of this issue requires user interaction in that a victim must open a malicious file.

- [https://github.com/NULL200OK/cve_2026_34621_advanced](https://github.com/NULL200OK/cve_2026_34621_advanced) :  ![starts](https://img.shields.io/github/stars/NULL200OK/cve_2026_34621_advanced.svg) ![forks](https://img.shields.io/github/forks/NULL200OK/cve_2026_34621_advanced.svg)


## CVE-2026-34486
Users are recommended to upgrade to version 11.0.21, 10.1.54 or 9.0.117, which fix the issue.

- [https://github.com/AirSkye/CVE-2026-34486-poc](https://github.com/AirSkye/CVE-2026-34486-poc) :  ![starts](https://img.shields.io/github/stars/AirSkye/CVE-2026-34486-poc.svg) ![forks](https://img.shields.io/github/forks/AirSkye/CVE-2026-34486-poc.svg)
- [https://github.com/404-src/CVE-2026-34486](https://github.com/404-src/CVE-2026-34486) :  ![starts](https://img.shields.io/github/stars/404-src/CVE-2026-34486.svg) ![forks](https://img.shields.io/github/forks/404-src/CVE-2026-34486.svg)
- [https://github.com/punitdarji/tomcat-cve-2026-34486](https://github.com/punitdarji/tomcat-cve-2026-34486) :  ![starts](https://img.shields.io/github/stars/punitdarji/tomcat-cve-2026-34486.svg) ![forks](https://img.shields.io/github/forks/punitdarji/tomcat-cve-2026-34486.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/masterwok/PoC-CVE-2026-33017](https://github.com/masterwok/PoC-CVE-2026-33017) :  ![starts](https://img.shields.io/github/stars/masterwok/PoC-CVE-2026-33017.svg) ![forks](https://img.shields.io/github/forks/masterwok/PoC-CVE-2026-33017.svg)


## CVE-2026-32286
 The DataRow.Decode function fails to properly validate field lengths. A malicious or compromised PostgreSQL server can send a DataRow message with a negative field length, causing a slice bounds out of range panic.

- [https://github.com/moisei-dev/go-dbmigrate](https://github.com/moisei-dev/go-dbmigrate) :  ![starts](https://img.shields.io/github/stars/moisei-dev/go-dbmigrate.svg) ![forks](https://img.shields.io/github/forks/moisei-dev/go-dbmigrate.svg)


## CVE-2026-20127
This vulnerability exists because the peering authentication mechanism in an affected system is not working properly. An attacker could exploit this vulnerability by sending crafted requests to an affected system. A successful exploit could allow the attacker to log in to an affected Cisco Catalyst SD-WAN Controller as an internal, high-privileged, non-root&nbsp;user account. Using this account, the attacker could access NETCONF, which would then allow the attacker to manipulate network configuration for the SD-WAN fabric.&nbsp;

- [https://github.com/gigachadusers/cve-2026-20127](https://github.com/gigachadusers/cve-2026-20127) :  ![starts](https://img.shields.io/github/stars/gigachadusers/cve-2026-20127.svg) ![forks](https://img.shields.io/github/forks/gigachadusers/cve-2026-20127.svg)


## CVE-2026-4057
 The Download Manager plugin for WordPress is vulnerable to unauthorized modification of data due to a missing capability check on the `makeMediaPublic()` and `makeMediaPrivate()` functions in all versions up to, and including, 3.3.51. This is due to the functions only checking for `edit_posts` capability without verifying post ownership via `current_user_can('edit_post', $id)`, and the destructive operations executing before the admin-level check in `mediaAccessControl()`. This makes it possible for authenticated attackers, with Contributor-level access and above, to strip all protection metadata (password, access restrictions, private flag) from any media file they do not own, making admin-protected files publicly accessible via their direct URL.

- [https://github.com/zebbernCVE/CVE-2026-40579](https://github.com/zebbernCVE/CVE-2026-40579) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-40579.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-40579.svg)


## CVE-2026-1357
 The Migration, Backup, Staging – WPvivid Backup & Migration plugin for WordPress is vulnerable to Unauthenticated Arbitrary File Upload in versions up to and including 0.9.123. This is due to improper error handling in the RSA decryption process combined with a lack of path sanitization when writing uploaded files. When the plugin fails to decrypt a session key using openssl_private_decrypt(), it does not terminate execution and instead passes the boolean false value to the phpseclib library's AES cipher initialization. The library treats this false value as a string of null bytes, allowing an attacker to encrypt a malicious payload using a predictable null-byte key. Additionally, the plugin accepts filenames from the decrypted payload without sanitization, enabling directory traversal to escape the protected backup directory. This makes it possible for unauthenticated attackers to upload arbitrary PHP files to publicly accessible directories and achieve Remote Code Execution via the wpvivid_action=send_to_site parameter.

- [https://github.com/masterwok/PoC-CVE-2026-1357](https://github.com/masterwok/PoC-CVE-2026-1357) :  ![starts](https://img.shields.io/github/stars/masterwok/PoC-CVE-2026-1357.svg) ![forks](https://img.shields.io/github/forks/masterwok/PoC-CVE-2026-1357.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-60710
 Improper link resolution before file access ('link following') in Host Process for Windows Tasks allows an authorized attacker to elevate privileges locally.

- [https://github.com/Wh04m1001/CVE-2025-60710](https://github.com/Wh04m1001/CVE-2025-60710) :  ![starts](https://img.shields.io/github/stars/Wh04m1001/CVE-2025-60710.svg) ![forks](https://img.shields.io/github/forks/Wh04m1001/CVE-2025-60710.svg)


## CVE-2025-59528
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5, Flowise is vulnerable to remote code execution. The CustomMCP node allows users to input configuration settings for connecting to an external MCP server. This node parses the user-provided mcpServerConfig string to build the MCP server configuration. However, during this process, it executes JavaScript code without any security validation. Specifically, inside the convertToValidJSONString function, user input is directly passed to the Function() constructor, which evaluates and executes the input as JavaScript code. Since this runs with full Node.js runtime privileges, it can access dangerous modules such as child_process and fs. This issue has been patched in version 3.0.6.

- [https://github.com/r3nsi15/Flowise-RCE-CVE-2025-59528](https://github.com/r3nsi15/Flowise-RCE-CVE-2025-59528) :  ![starts](https://img.shields.io/github/stars/r3nsi15/Flowise-RCE-CVE-2025-59528.svg) ![forks](https://img.shields.io/github/forks/r3nsi15/Flowise-RCE-CVE-2025-59528.svg)
- [https://github.com/maradonam18/-CVE-2025-59528-PoC](https://github.com/maradonam18/-CVE-2025-59528-PoC) :  ![starts](https://img.shields.io/github/stars/maradonam18/-CVE-2025-59528-PoC.svg) ![forks](https://img.shields.io/github/forks/maradonam18/-CVE-2025-59528-PoC.svg)


## CVE-2025-58434
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5 and earlier, the `forgot-password` endpoint in Flowise returns sensitive information including a valid password reset `tempToken` without authentication or verification. This enables any attacker to generate a reset token for arbitrary users and directly reset their password, leading to a complete account takeover (ATO). This vulnerability applies to both the cloud service (`cloud.flowiseai.com`) and self-hosted/local Flowise deployments that expose the same API. Commit 9e178d68873eb876073846433a596590d3d9c863 in version 3.0.6 secures password reset endpoints. Several recommended remediation steps are available. Do not return reset tokens or sensitive account details in API responses. Tokens must only be delivered securely via the registered email channel. Ensure `forgot-password` responds with a generic success message regardless of input, to avoid user enumeration. Require strong validation of the `tempToken` (e.g., single-use, short expiry, tied to request origin, validated against email delivery). Apply the same fixes to both cloud and self-hosted/local deployments. Log and monitor password reset requests for suspicious activity. Consider multi-factor verification for sensitive accounts.

- [https://github.com/r3nsi15/Flowise-CVE-2025-58434-PasswordReset](https://github.com/r3nsi15/Flowise-CVE-2025-58434-PasswordReset) :  ![starts](https://img.shields.io/github/stars/r3nsi15/Flowise-CVE-2025-58434-PasswordReset.svg) ![forks](https://img.shields.io/github/forks/r3nsi15/Flowise-CVE-2025-58434-PasswordReset.svg)


## CVE-2025-58060
 OpenPrinting CUPS is an open source printing system for Linux and other Unix-like operating systems. In versions 2.4.12 and earlier, when the `AuthType` is set to anything but `Basic`, if the request contains an `Authorization: Basic ...` header, the password is not checked. This results in authentication bypass. Any configuration that allows an `AuthType` that is not `Basic` is affected. Version 2.4.13 fixes the issue.

- [https://github.com/aniruddh-bhandarkar/cups-script-final-project](https://github.com/aniruddh-bhandarkar/cups-script-final-project) :  ![starts](https://img.shields.io/github/stars/aniruddh-bhandarkar/cups-script-final-project.svg) ![forks](https://img.shields.io/github/forks/aniruddh-bhandarkar/cups-script-final-project.svg)


## CVE-2025-51458
 SQL Injection in editor_sql_run and query_ex in eosphoros-ai DB-GPT 0.7.0 allows remote attackers to execute arbitrary SQL statements via crafted input passed to the /v1/editor/sql/run or /v1/editor/chart/run endpoints, interacting with api_editor_v1.editor_sql_run, editor_chart_run, and datasource.rdbms.base.query_ex.

- [https://github.com/q1uf3ng/CVE-2025-51458-exp](https://github.com/q1uf3ng/CVE-2025-51458-exp) :  ![starts](https://img.shields.io/github/stars/q1uf3ng/CVE-2025-51458-exp.svg) ![forks](https://img.shields.io/github/forks/q1uf3ng/CVE-2025-51458-exp.svg)


## CVE-2025-49132
 Pterodactyl is a free, open-source game server management panel. Prior to version 1.11.11, using the /locales/locale.json with the locale and namespace query parameters, a malicious actor is able to execute arbitrary code without being authenticated. With the ability to execute arbitrary code it could be used to gain access to the Panel's server, read credentials from the Panel's config, extract sensitive information from the database, access files of servers managed by the panel, etc. This issue has been patched in version 1.11.11. There are no software workarounds for this vulnerability, but use of an external Web Application Firewall (WAF) could help mitigate this attack.

- [https://github.com/V0idW1re/HTB-Pterodactyl-Writeup](https://github.com/V0idW1re/HTB-Pterodactyl-Writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/HTB-Pterodactyl-Writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/HTB-Pterodactyl-Writeup.svg)


## CVE-2025-49113
 Roundcube Webmail before 1.5.10 and 1.6.x before 1.6.11 allows remote code execution by authenticated users because the _from parameter in a URL is not validated in program/actions/settings/upload.php, leading to PHP Object Deserialization.

- [https://github.com/rippsec/CVE-2025-49113-Roundcube-RCE](https://github.com/rippsec/CVE-2025-49113-Roundcube-RCE) :  ![starts](https://img.shields.io/github/stars/rippsec/CVE-2025-49113-Roundcube-RCE.svg) ![forks](https://img.shields.io/github/forks/rippsec/CVE-2025-49113-Roundcube-RCE.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/MKIRAHMET/CVE-2025-29927-PoC](https://github.com/MKIRAHMET/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/MKIRAHMET/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/MKIRAHMET/CVE-2025-29927-PoC.svg)
- [https://github.com/enochgitgamefied/NextJS-CVE-2025-29927](https://github.com/enochgitgamefied/NextJS-CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/enochgitgamefied/NextJS-CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/enochgitgamefied/NextJS-CVE-2025-29927.svg)


## CVE-2025-27591
 A privilege escalation vulnerability existed in the Below service prior to v0.9.0 due to the creation of a world-writable directory at /var/log/below. This could have allowed local unprivileged users to escalate to root privileges through symlink attacks that manipulate files such as /etc/shadow.

- [https://github.com/rippsec/CVE-2025-27591-Meta-below-LPE](https://github.com/rippsec/CVE-2025-27591-Meta-below-LPE) :  ![starts](https://img.shields.io/github/stars/rippsec/CVE-2025-27591-Meta-below-LPE.svg) ![forks](https://img.shields.io/github/forks/rippsec/CVE-2025-27591-Meta-below-LPE.svg)


## CVE-2025-24893
 XWiki Platform is a generic wiki platform offering runtime services for applications built on top of it. Any guest can perform arbitrary remote code execution through a request to `SolrSearch`. This impacts the confidentiality, integrity and availability of the whole XWiki installation. To reproduce on an instance, without being logged in, go to `host/xwiki/bin/get/Main/SolrSearch?media=rss&text=%7D%7D%7D%7B%7Basync%20async%3Dfalse%7D%7D%7B%7Bgroovy%7D%7Dprintln%28"Hello%20from"%20%2B%20"%20search%20text%3A"%20%2B%20%2823%20%2B%2019%29%29%7B%7B%2Fgroovy%7D%7D%7B%7B%2Fasync%7D%7D%20`. If there is an output, and the title of the RSS feed contains `Hello from search text:42`, then the instance is vulnerable. This vulnerability has been patched in XWiki 15.10.11, 16.4.1 and 16.5.0RC1. Users are advised to upgrade. Users unable to upgrade may edit `Main.SolrSearchMacros` in `SolrSearchMacros.xml` on line 955 to match the `rawResponse` macro in `macros.vm#L2824` with a content type of `application/xml`, instead of simply outputting the content of the feed.

- [https://github.com/rippsec/CVE-2025-24893-XWiki-SSTI-RCE](https://github.com/rippsec/CVE-2025-24893-XWiki-SSTI-RCE) :  ![starts](https://img.shields.io/github/stars/rippsec/CVE-2025-24893-XWiki-SSTI-RCE.svg) ![forks](https://img.shields.io/github/forks/rippsec/CVE-2025-24893-XWiki-SSTI-RCE.svg)


## CVE-2025-13486
 The Advanced Custom Fields: Extended plugin for WordPress is vulnerable to Remote Code Execution in versions 0.9.0.5 through 0.9.1.1 via the prepare_form() function. This is due to the function accepting user input and then passing that through call_user_func_array(). This makes it possible for unauthenticated attackers to execute arbitrary code on the server, which can be leveraged to inject backdoors or create new administrative user accounts.

- [https://github.com/whattheslime/CVE-2025-13486](https://github.com/whattheslime/CVE-2025-13486) :  ![starts](https://img.shields.io/github/stars/whattheslime/CVE-2025-13486.svg) ![forks](https://img.shields.io/github/forks/whattheslime/CVE-2025-13486.svg)


## CVE-2025-8110
 Improper Symbolic link handling in the PutContents API in Gogs allows Local Execution of Code.

- [https://github.com/X4BROZER/CVE-2025-8110](https://github.com/X4BROZER/CVE-2025-8110) :  ![starts](https://img.shields.io/github/stars/X4BROZER/CVE-2025-8110.svg) ![forks](https://img.shields.io/github/forks/X4BROZER/CVE-2025-8110.svg)


## CVE-2025-6019
 A Local Privilege Escalation (LPE) vulnerability was found in libblockdev. Generally, the "allow_active" setting in Polkit permits a physically present user to take certain actions based on the session type. Due to the way libblockdev interacts with the udisks daemon, an "allow_active" user on a system may be able escalate to full root privileges on the target host. Normally, udisks mounts user-provided filesystem images with security flags like nosuid and nodev to prevent privilege escalation.  However, a local attacker can create a specially crafted XFS image containing a SUID-root shell, then trick udisks into resizing it. This mounts their malicious filesystem with root privileges, allowing them to execute their SUID-root shell and gain complete control of the system.

- [https://github.com/V0idW1re/HTB-Pterodactyl-Writeup](https://github.com/V0idW1re/HTB-Pterodactyl-Writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/HTB-Pterodactyl-Writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/HTB-Pterodactyl-Writeup.svg)


## CVE-2025-6018
 A Local Privilege Escalation (LPE) vulnerability has been discovered in pam-config within Linux Pluggable Authentication Modules (PAM). This flaw allows an unprivileged local attacker (for example, a user logged in via SSH) to obtain the elevated privileges normally reserved for a physically present, "allow_active" user. The highest risk is that the attacker can then perform all allow_active yes Polkit actions, which are typically restricted to console users, potentially gaining unauthorized control over system configurations, services, or other sensitive operations.

- [https://github.com/V0idW1re/HTB-Pterodactyl-Writeup](https://github.com/V0idW1re/HTB-Pterodactyl-Writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/HTB-Pterodactyl-Writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/HTB-Pterodactyl-Writeup.svg)


## CVE-2024-26229
 Windows CSC Service Elevation of Privilege Vulnerability

- [https://github.com/0xGunrunner/CVE-2024-26229-BOF](https://github.com/0xGunrunner/CVE-2024-26229-BOF) :  ![starts](https://img.shields.io/github/stars/0xGunrunner/CVE-2024-26229-BOF.svg) ![forks](https://img.shields.io/github/forks/0xGunrunner/CVE-2024-26229-BOF.svg)


## CVE-2024-12029
 A remote code execution vulnerability exists in invoke-ai/invokeai versions 5.3.1 through 5.4.2 via the /api/v2/models/install API. The vulnerability arises from unsafe deserialization of model files using torch.load without proper validation. Attackers can exploit this by embedding malicious code in model files, which is executed upon loading. This issue is fixed in version 5.4.3.

- [https://github.com/Lu3ky13/Alternative-Approach-Reverse-Shell-Callback-Test-InvokeAI-RCE](https://github.com/Lu3ky13/Alternative-Approach-Reverse-Shell-Callback-Test-InvokeAI-RCE) :  ![starts](https://img.shields.io/github/stars/Lu3ky13/Alternative-Approach-Reverse-Shell-Callback-Test-InvokeAI-RCE.svg) ![forks](https://img.shields.io/github/forks/Lu3ky13/Alternative-Approach-Reverse-Shell-Callback-Test-InvokeAI-RCE.svg)


## CVE-2024-3094
Through a series of complex obfuscations, the liblzma build process extracts a prebuilt object file from a disguised test file existing in the source code, which is then used to modify specific functions in the liblzma code. This results in a modified liblzma library that can be used by any software linked against this library, intercepting and modifying the data interaction with this library.

- [https://github.com/Ava-Vispilio/CVE-2024-3094](https://github.com/Ava-Vispilio/CVE-2024-3094) :  ![starts](https://img.shields.io/github/stars/Ava-Vispilio/CVE-2024-3094.svg) ![forks](https://img.shields.io/github/forks/Ava-Vispilio/CVE-2024-3094.svg)


## CVE-2023-3262
 The Dataprobe iBoot PDU running firmware version 1.43.03312023 or earlier uses hard-coded credentials for all interactions with the internal Postgres database.A malicious agent with the ability to execute operating system commands on the device can leverage this vulnerability to read, modify, or delete arbitrary database records.

- [https://github.com/SanjayRagavendar/Ubuntu-GameOver-Lay](https://github.com/SanjayRagavendar/Ubuntu-GameOver-Lay) :  ![starts](https://img.shields.io/github/stars/SanjayRagavendar/Ubuntu-GameOver-Lay.svg) ![forks](https://img.shields.io/github/forks/SanjayRagavendar/Ubuntu-GameOver-Lay.svg)
- [https://github.com/z3usx01/CVE-2023-2640-3262-PoC](https://github.com/z3usx01/CVE-2023-2640-3262-PoC) :  ![starts](https://img.shields.io/github/stars/z3usx01/CVE-2023-2640-3262-PoC.svg) ![forks](https://img.shields.io/github/forks/z3usx01/CVE-2023-2640-3262-PoC.svg)


## CVE-2023-3171
 A flaw was found in EAP-7 during deserialization of certain classes, which permits instantiation of HashMap and HashTable with no checks on resources consumed. This issue could allow an attacker to submit malicious requests using these classes, which could eventually exhaust the heap and result in a Denial of Service.

- [https://github.com/HritikThapa7/CVE-2023-31711](https://github.com/HritikThapa7/CVE-2023-31711) :  ![starts](https://img.shields.io/github/stars/HritikThapa7/CVE-2023-31711.svg) ![forks](https://img.shields.io/github/forks/HritikThapa7/CVE-2023-31711.svg)


## CVE-2022-35650
 The vulnerability was found in Moodle, occurs due to input validation error when importing lesson questions. This insufficient path checks results in arbitrary file read risk. This vulnerability allows a remote attacker to perform directory traversal attacks. The capability to access this feature is only available to teachers, managers and admins by default.

- [https://github.com/Gr4y-r0se/CVE-2022-35650](https://github.com/Gr4y-r0se/CVE-2022-35650) :  ![starts](https://img.shields.io/github/stars/Gr4y-r0se/CVE-2022-35650.svg) ![forks](https://img.shields.io/github/forks/Gr4y-r0se/CVE-2022-35650.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/puckiestyle/CVE-2021-41773](https://github.com/puckiestyle/CVE-2021-41773) :  ![starts](https://img.shields.io/github/stars/puckiestyle/CVE-2021-41773.svg) ![forks](https://img.shields.io/github/forks/puckiestyle/CVE-2021-41773.svg)


## CVE-2021-22986
 On BIG-IP versions 16.0.x before 16.0.1.1, 15.1.x before 15.1.2.1, 14.1.x before 14.1.4, 13.1.x before 13.1.3.6, and 12.1.x before 12.1.5.3 amd BIG-IQ 7.1.0.x before 7.1.0.3 and 7.0.0.x before 7.0.0.2, the iControl REST interface has an unauthenticated remote command execution vulnerability. Note: Software versions which have reached End of Software Development (EoSD) are not evaluated.

- [https://github.com/whatheheckisthis/CVE-2021-22986](https://github.com/whatheheckisthis/CVE-2021-22986) :  ![starts](https://img.shields.io/github/stars/whatheheckisthis/CVE-2021-22986.svg) ![forks](https://img.shields.io/github/forks/whatheheckisthis/CVE-2021-22986.svg)


## CVE-2020-15999
 Heap buffer overflow in Freetype in Google Chrome prior to 86.0.4240.111 allowed a remote attacker to potentially exploit heap corruption via a crafted HTML page.

- [https://github.com/oxfemale/CVE-2020-15999](https://github.com/oxfemale/CVE-2020-15999) :  ![starts](https://img.shields.io/github/stars/oxfemale/CVE-2020-15999.svg) ![forks](https://img.shields.io/github/forks/oxfemale/CVE-2020-15999.svg)
- [https://github.com/Marmeus/CVE-2020-15999](https://github.com/Marmeus/CVE-2020-15999) :  ![starts](https://img.shields.io/github/stars/Marmeus/CVE-2020-15999.svg) ![forks](https://img.shields.io/github/forks/Marmeus/CVE-2020-15999.svg)
- [https://github.com/maarlo/CVE-2020-15999](https://github.com/maarlo/CVE-2020-15999) :  ![starts](https://img.shields.io/github/stars/maarlo/CVE-2020-15999.svg) ![forks](https://img.shields.io/github/forks/maarlo/CVE-2020-15999.svg)


## CVE-2020-15568
 TerraMaster TOS before 4.1.29 has Invalid Parameter Checking that leads to code injection as root. This is a dynamic class method invocation vulnerability in include/exportUser.php, in which an attacker can trigger a call to the exec method with (for example) OS commands in the opt parameter.

- [https://github.com/divinepwner/TerraMaster-TOS-CVE-2020-15568](https://github.com/divinepwner/TerraMaster-TOS-CVE-2020-15568) :  ![starts](https://img.shields.io/github/stars/divinepwner/TerraMaster-TOS-CVE-2020-15568.svg) ![forks](https://img.shields.io/github/forks/divinepwner/TerraMaster-TOS-CVE-2020-15568.svg)
- [https://github.com/n0bugz/CVE-2020-15568](https://github.com/n0bugz/CVE-2020-15568) :  ![starts](https://img.shields.io/github/stars/n0bugz/CVE-2020-15568.svg) ![forks](https://img.shields.io/github/forks/n0bugz/CVE-2020-15568.svg)


## CVE-2020-15135
 save-server (npm package) before version 1.05 is affected by a CSRF vulnerability, as there is no CSRF mitigation (Tokens etc.). The fix introduced in version version 1.05 unintentionally breaks uploading so version v1.0.7 is the fixed version. This is patched by implementing Double submit. The CSRF attack would require you to navigate to a malicious site while you have an active session with Save-Server (Session key stored in cookies). The malicious user would then be able to perform some actions, including uploading/deleting files and adding redirects. If you are logged in as root, this attack is significantly more severe. They can in addition create, delete and update users. If they updated the password of a user, that user's files would then be available. If the root password is updated, all files would be visible if they logged in with the new password. Note that due to the same origin policy malicious actors cannot view the gallery or the response of any of the methods, nor be sure they succeeded. This issue has been patched in version 1.0.7.

- [https://github.com/ossf-cve-benchmark/CVE-2020-15135](https://github.com/ossf-cve-benchmark/CVE-2020-15135) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2020-15135.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2020-15135.svg)


## CVE-2020-11890
 An issue was discovered in Joomla! before 3.9.17. Improper input validations in the usergroup table class could lead to a broken ACL configuration.

- [https://github.com/HoangKien1020/CVE-2020-11890](https://github.com/HoangKien1020/CVE-2020-11890) :  ![starts](https://img.shields.io/github/stars/HoangKien1020/CVE-2020-11890.svg) ![forks](https://img.shields.io/github/forks/HoangKien1020/CVE-2020-11890.svg)


## CVE-2019-13720
 Use after free in WebAudio in Google Chrome prior to 78.0.3904.87 allowed a remote attacker to potentially exploit heap corruption via a crafted HTML page.

- [https://github.com/forrest-orr/WizardOpium](https://github.com/forrest-orr/WizardOpium) :  ![starts](https://img.shields.io/github/stars/forrest-orr/WizardOpium.svg) ![forks](https://img.shields.io/github/forks/forrest-orr/WizardOpium.svg)
- [https://github.com/bb33bb/CVE-2019-13720](https://github.com/bb33bb/CVE-2019-13720) :  ![starts](https://img.shields.io/github/stars/bb33bb/CVE-2019-13720.svg) ![forks](https://img.shields.io/github/forks/bb33bb/CVE-2019-13720.svg)
- [https://github.com/cve-2019-13720/cve-2019-13720](https://github.com/cve-2019-13720/cve-2019-13720) :  ![starts](https://img.shields.io/github/stars/cve-2019-13720/cve-2019-13720.svg) ![forks](https://img.shields.io/github/forks/cve-2019-13720/cve-2019-13720.svg)


## CVE-2019-10077
 A carefully crafted InterWiki link could trigger an XSS vulnerability on Apache JSPWiki 2.9.0 to 2.11.0.M3, which could lead to session hijacking.

- [https://github.com/shoucheng3/apache__jspwiki_CVE-2019-10077_2-11-0-M3](https://github.com/shoucheng3/apache__jspwiki_CVE-2019-10077_2-11-0-M3) :  ![starts](https://img.shields.io/github/stars/shoucheng3/apache__jspwiki_CVE-2019-10077_2-11-0-M3.svg) ![forks](https://img.shields.io/github/forks/shoucheng3/apache__jspwiki_CVE-2019-10077_2-11-0-M3.svg)
- [https://github.com/shoucheng3/apache__jspwiki_CVE-2019-10077_2_11_0_M4_fixed](https://github.com/shoucheng3/apache__jspwiki_CVE-2019-10077_2_11_0_M4_fixed) :  ![starts](https://img.shields.io/github/stars/shoucheng3/apache__jspwiki_CVE-2019-10077_2_11_0_M4_fixed.svg) ![forks](https://img.shields.io/github/forks/shoucheng3/apache__jspwiki_CVE-2019-10077_2_11_0_M4_fixed.svg)


## CVE-2019-9053
 An issue was discovered in CMS Made Simple 2.2.8. It is possible with the News module, through a crafted URL, to achieve unauthenticated blind time-based SQL injection via the m1_idlist parameter.

- [https://github.com/iTzR1g/CVE-2019-9053](https://github.com/iTzR1g/CVE-2019-9053) :  ![starts](https://img.shields.io/github/stars/iTzR1g/CVE-2019-9053.svg) ![forks](https://img.shields.io/github/forks/iTzR1g/CVE-2019-9053.svg)


## CVE-2018-1235
 Dell EMC RecoverPoint versions prior to 5.1.2 and RecoverPoint for VMs versions prior to 5.1.1.3, contain a command injection vulnerability. An unauthenticated remote attacker may potentially exploit this vulnerability to execute arbitrary commands on the affected system with root privilege.

- [https://github.com/AbsoZed/CVE-2018-1235](https://github.com/AbsoZed/CVE-2018-1235) :  ![starts](https://img.shields.io/github/stars/AbsoZed/CVE-2018-1235.svg) ![forks](https://img.shields.io/github/forks/AbsoZed/CVE-2018-1235.svg)


## CVE-2003-0264
 Multiple buffer overflows in SLMail 5.1.0.4420 allows remote attackers to execute arbitrary code via (1) a long EHLO argument to slmail.exe, (2) a long XTRN argument to slmail.exe, (3) a long string to POPPASSWD, or (4) a long password to the POP3 server.

- [https://github.com/TheMalwareGuardian/CVE-2003-0264](https://github.com/TheMalwareGuardian/CVE-2003-0264) :  ![starts](https://img.shields.io/github/stars/TheMalwareGuardian/CVE-2003-0264.svg) ![forks](https://img.shields.io/github/forks/TheMalwareGuardian/CVE-2003-0264.svg)


## CVE-2003-0127
 The kernel module loader in Linux kernel 2.2.x before 2.2.25, and 2.4.x before 2.4.21, allows local users to gain root privileges by using ptrace to attach to a child process that is spawned by the kernel.

- [https://github.com/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation](https://github.com/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation) :  ![starts](https://img.shields.io/github/stars/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation.svg) ![forks](https://img.shields.io/github/forks/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation.svg)

