# Update 2026-04-10
## CVE-2026-39363
 Vite is a frontend tooling framework for JavaScript. From 6.0.0 to before 6.4.2, 7.3.2, and 8.0.5, if it is possible to connect to the Vite dev server’s WebSocket without an Origin header, an attacker can invoke fetchModule via the custom WebSocket event vite:invoke and combine file://... with ?raw (or ?inline) to retrieve the contents of arbitrary files on the server as a JavaScript string (e.g., export default "..."). The access control enforced in the HTTP request path (such as server.fs.allow) is not applied to this WebSocket-based execution path. This vulnerability is fixed in 6.4.2, 7.3.2, and 8.0.5.

- [https://github.com/Firebasky/CVE-2026-39363](https://github.com/Firebasky/CVE-2026-39363) :  ![starts](https://img.shields.io/github/stars/Firebasky/CVE-2026-39363.svg) ![forks](https://img.shields.io/github/forks/Firebasky/CVE-2026-39363.svg)


## CVE-2026-34197
Users are recommended to upgrade to version 5.19.4 or 6.2.3, which fixes the issue

- [https://github.com/dinosn/CVE-2026-34197](https://github.com/dinosn/CVE-2026-34197) :  ![starts](https://img.shields.io/github/stars/dinosn/CVE-2026-34197.svg) ![forks](https://img.shields.io/github/forks/dinosn/CVE-2026-34197.svg)
- [https://github.com/0xBlackash/CVE-2026-34197](https://github.com/0xBlackash/CVE-2026-34197) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-34197.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-34197.svg)
- [https://github.com/DEVSECURITYSPRO/CVE-2026-34197](https://github.com/DEVSECURITYSPRO/CVE-2026-34197) :  ![starts](https://img.shields.io/github/stars/DEVSECURITYSPRO/CVE-2026-34197.svg) ![forks](https://img.shields.io/github/forks/DEVSECURITYSPRO/CVE-2026-34197.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/oscarmine/CVE-2026-33017-Exploit](https://github.com/oscarmine/CVE-2026-33017-Exploit) :  ![starts](https://img.shields.io/github/stars/oscarmine/CVE-2026-33017-Exploit.svg) ![forks](https://img.shields.io/github/forks/oscarmine/CVE-2026-33017-Exploit.svg)


## CVE-2026-27739
 The Angular SSR is a server-rise rendering tool for Angular applications. Versions prior to 21.2.0-rc.1, 21.1.5, 20.3.17, and 19.2.21 have a Server-Side Request Forgery (SSRF) vulnerability in the Angular SSR request handling pipeline. The vulnerability exists because Angular’s internal URL reconstruction logic directly trusts and consumes user-controlled HTTP headers specifically the Host and `X-Forwarded-*` family to determine the application's base origin without any validation of the destination domain. Specifically, the framework didn't have checks for the host domain, path and character sanitization, and port validation. This vulnerability manifests in two primary ways: implicit relative URL resolution and explicit manual construction. When successfully exploited, this vulnerability allows for arbitrary internal request steering. This can lead to credential exfiltration, internal network probing, and a confidentiality breach. In order to be vulnerable, the victim application must use Angular SSR (Server-Side Rendering), the application must perform `HttpClient` requests using relative URLs OR manually construct URLs using the unvalidated `Host` / `X-Forwarded-*` headers using the `REQUEST` object, the application server must be reachable by an attacker who can influence these headers without strict validation from a front-facing proxy, and the infrastructure (Cloud, CDN, or Load Balancer) must not sanitize or validate incoming headers. Versions 21.2.0-rc.1, 21.1.5, 20.3.17, and 19.2.21 contain a patch. Some workarounds are available. Avoid using `req.headers` for URL construction. Instead, use trusted variables for base API paths. Those who cannot upgrade immediately should implement a middleware in their `server.ts` to enforce numeric ports and validated hostnames.

- [https://github.com/mr-redoo7/CVE-2026-27739-POC](https://github.com/mr-redoo7/CVE-2026-27739-POC) :  ![starts](https://img.shields.io/github/stars/mr-redoo7/CVE-2026-27739-POC.svg) ![forks](https://img.shields.io/github/forks/mr-redoo7/CVE-2026-27739-POC.svg)


## CVE-2026-25253
 OpenClaw (aka clawdbot or Moltbot) before 2026.1.29 obtains a gatewayUrl value from a query string and automatically makes a WebSocket connection without prompting, sending a token value.

- [https://github.com/msaleme/start-here](https://github.com/msaleme/start-here) :  ![starts](https://img.shields.io/github/stars/msaleme/start-here.svg) ![forks](https://img.shields.io/github/forks/msaleme/start-here.svg)


## CVE-2026-23980
Users are recommended to upgrade to version 6.0.0, which fixes the issue.

- [https://github.com/oscarmine/CVE-2026-23980-Exploit](https://github.com/oscarmine/CVE-2026-23980-Exploit) :  ![starts](https://img.shields.io/github/stars/oscarmine/CVE-2026-23980-Exploit.svg) ![forks](https://img.shields.io/github/forks/oscarmine/CVE-2026-23980-Exploit.svg)


## CVE-2026-23398
perform strict tag validation.

- [https://github.com/zpol/cve-2026-23398-poc](https://github.com/zpol/cve-2026-23398-poc) :  ![starts](https://img.shields.io/github/stars/zpol/cve-2026-23398-poc.svg) ![forks](https://img.shields.io/github/forks/zpol/cve-2026-23398-poc.svg)


## CVE-2026-3288
 A security issue was discovered in ingress-nginx where the `nginx.ingress.kubernetes.io/rewrite-target` Ingress annotation can be used to inject configuration into nginx. This can lead to arbitrary code execution in the context of the ingress-nginx controller, and disclosure of Secrets accessible to the controller. (Note that in the default installation, the controller can access all Secrets cluster-wide.)

- [https://github.com/bvabhishek/CVE-2026-3288-lab](https://github.com/bvabhishek/CVE-2026-3288-lab) :  ![starts](https://img.shields.io/github/stars/bvabhishek/CVE-2026-3288-lab.svg) ![forks](https://img.shields.io/github/forks/bvabhishek/CVE-2026-3288-lab.svg)


## CVE-2026-0740
 The Ninja Forms - File Uploads plugin for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the 'NF_FU_AJAX_Controllers_Uploads::handle_upload' function in all versions up to, and including, 3.3.26. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible. Note: The vulnerability was partially patched in version 3.3.25 and fully patched in version 3.3.27.

- [https://github.com/xShadow-Here/CVE-2026-0740](https://github.com/xShadow-Here/CVE-2026-0740) :  ![starts](https://img.shields.io/github/stars/xShadow-Here/CVE-2026-0740.svg) ![forks](https://img.shields.io/github/forks/xShadow-Here/CVE-2026-0740.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478](https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478) :  ![starts](https://img.shields.io/github/stars/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg) ![forks](https://img.shields.io/github/forks/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)


## CVE-2025-66034
 fontTools is a library for manipulating fonts, written in Python. In versions from 4.33.0 to before 4.60.2, the fonttools varLib (or python3 -m fontTools.varLib) script has an arbitrary file write vulnerability that leads to remote code execution when a malicious .designspace file is processed. The vulnerability affects the main() code path of fontTools.varLib, used by the fonttools varLib CLI and any code that invokes fontTools.varLib.main(). This issue has been patched in version 4.60.2.

- [https://github.com/V0idW1re/HTB-VariaType-Writeup](https://github.com/V0idW1re/HTB-VariaType-Writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/HTB-VariaType-Writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/HTB-VariaType-Writeup.svg)


## CVE-2025-55182
 A pre-authentication remote code execution vulnerability exists in React Server Components versions 19.0.0, 19.1.0, 19.1.1, and 19.2.0 including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints.

- [https://github.com/rix4uni/CVE-2025-55182](https://github.com/rix4uni/CVE-2025-55182) :  ![starts](https://img.shields.io/github/stars/rix4uni/CVE-2025-55182.svg) ![forks](https://img.shields.io/github/forks/rix4uni/CVE-2025-55182.svg)


## CVE-2025-49132
 Pterodactyl is a free, open-source game server management panel. Prior to version 1.11.11, using the /locales/locale.json with the locale and namespace query parameters, a malicious actor is able to execute arbitrary code without being authenticated. With the ability to execute arbitrary code it could be used to gain access to the Panel's server, read credentials from the Panel's config, extract sensitive information from the database, access files of servers managed by the panel, etc. This issue has been patched in version 1.11.11. There are no software workarounds for this vulnerability, but use of an external Web Application Firewall (WAF) could help mitigate this attack.

- [https://github.com/V0idW1re/htb-pterodactyl-writeup](https://github.com/V0idW1re/htb-pterodactyl-writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/htb-pterodactyl-writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/htb-pterodactyl-writeup.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/MKIRAHMET/CVE-2025-29927-PoC](https://github.com/MKIRAHMET/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/MKIRAHMET/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/MKIRAHMET/CVE-2025-29927-PoC.svg)


## CVE-2025-6019
 A Local Privilege Escalation (LPE) vulnerability was found in libblockdev. Generally, the "allow_active" setting in Polkit permits a physically present user to take certain actions based on the session type. Due to the way libblockdev interacts with the udisks daemon, an "allow_active" user on a system may be able escalate to full root privileges on the target host. Normally, udisks mounts user-provided filesystem images with security flags like nosuid and nodev to prevent privilege escalation.  However, a local attacker can create a specially crafted XFS image containing a SUID-root shell, then trick udisks into resizing it. This mounts their malicious filesystem with root privileges, allowing them to execute their SUID-root shell and gain complete control of the system.

- [https://github.com/V0idW1re/htb-pterodactyl-writeup](https://github.com/V0idW1re/htb-pterodactyl-writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/htb-pterodactyl-writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/htb-pterodactyl-writeup.svg)


## CVE-2025-6018
 A Local Privilege Escalation (LPE) vulnerability has been discovered in pam-config within Linux Pluggable Authentication Modules (PAM). This flaw allows an unprivileged local attacker (for example, a user logged in via SSH) to obtain the elevated privileges normally reserved for a physically present, "allow_active" user. The highest risk is that the attacker can then perform all allow_active yes Polkit actions, which are typically restricted to console users, potentially gaining unauthorized control over system configurations, services, or other sensitive operations.

- [https://github.com/V0idW1re/htb-pterodactyl-writeup](https://github.com/V0idW1re/htb-pterodactyl-writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/htb-pterodactyl-writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/htb-pterodactyl-writeup.svg)


## CVE-2024-25082
 Splinefont in FontForge through 20230101 allows command injection via crafted archives or compressed files.

- [https://github.com/V0idW1re/HTB-VariaType-Writeup](https://github.com/V0idW1re/HTB-VariaType-Writeup) :  ![starts](https://img.shields.io/github/stars/V0idW1re/HTB-VariaType-Writeup.svg) ![forks](https://img.shields.io/github/forks/V0idW1re/HTB-VariaType-Writeup.svg)


## CVE-2023-44487
 The HTTP/2 protocol allows a denial of service (server resource consumption) because request cancellation can reset many streams quickly, as exploited in the wild in August through October 2023.

- [https://github.com/TLevente20/HTTP-2-RapidReset-CVE-2023-44487-Testlab](https://github.com/TLevente20/HTTP-2-RapidReset-CVE-2023-44487-Testlab) :  ![starts](https://img.shields.io/github/stars/TLevente20/HTTP-2-RapidReset-CVE-2023-44487-Testlab.svg) ![forks](https://img.shields.io/github/forks/TLevente20/HTTP-2-RapidReset-CVE-2023-44487-Testlab.svg)


## CVE-2023-30258
 Command Injection vulnerability in MagnusSolution magnusbilling 6.x and 7.x allows remote attackers to run arbitrary commands via unauthenticated HTTP request.

- [https://github.com/cyb3rk0ala/THM-MagnusBilling-CVE-2023-30258-Exploit](https://github.com/cyb3rk0ala/THM-MagnusBilling-CVE-2023-30258-Exploit) :  ![starts](https://img.shields.io/github/stars/cyb3rk0ala/THM-MagnusBilling-CVE-2023-30258-Exploit.svg) ![forks](https://img.shields.io/github/forks/cyb3rk0ala/THM-MagnusBilling-CVE-2023-30258-Exploit.svg)


## CVE-2022-3656
 Insufficient data validation in File System in Google Chrome prior to 107.0.5304.62 allowed a remote attacker to bypass file system restrictions via a crafted HTML page. (Chromium security severity: Medium)

- [https://github.com/momika233/CVE-2022-3656](https://github.com/momika233/CVE-2022-3656) :  ![starts](https://img.shields.io/github/stars/momika233/CVE-2022-3656.svg) ![forks](https://img.shields.io/github/forks/momika233/CVE-2022-3656.svg)


## CVE-2022-0847
 A flaw was found in the way the "flags" member of the new pipe buffer structure was lacking proper initialization in copy_page_to_iter_pipe and push_pipe functions in the Linux kernel and could thus contain stale values. An unprivileged local user could use this flaw to write to pages in the page cache backed by read only files and as such escalate their privileges on the system.

- [https://github.com/hackingyseguridad/root](https://github.com/hackingyseguridad/root) :  ![starts](https://img.shields.io/github/stars/hackingyseguridad/root.svg) ![forks](https://img.shields.io/github/forks/hackingyseguridad/root.svg)
- [https://github.com/full-of-stars/cve_2022_0847](https://github.com/full-of-stars/cve_2022_0847) :  ![starts](https://img.shields.io/github/stars/full-of-stars/cve_2022_0847.svg) ![forks](https://img.shields.io/github/forks/full-of-stars/cve_2022_0847.svg)


## CVE-2020-15099
 In TYPO3 CMS greater than or equal to 9.0.0 and less than 9.5.20, and greater than or equal to 10.0.0 and less than 10.4.6, in a case where an attacker manages to generate a valid cryptographic message authentication code (HMAC-SHA1) - either by using a different existing vulnerability or in case the internal encryptionKey was exposed - it is possible to retrieve arbitrary files of a TYPO3 installation. This includes the possibility to fetch typo3conf/LocalConfiguration.php, which again contains the encryptionKey as well as credentials of the database management system being used. In case a database server is directly accessible either via internet or in a shared hosting network, this allows the ability to completely retrieve, manipulate or delete database contents. This includes creating an administration user account - which can be used to trigger remote code execution by injecting custom extensions. This has been patched in versions 9.5.20 and 10.4.6.

- [https://github.com/Dread1ess/CVE-2020-15099](https://github.com/Dread1ess/CVE-2020-15099) :  ![starts](https://img.shields.io/github/stars/Dread1ess/CVE-2020-15099.svg) ![forks](https://img.shields.io/github/forks/Dread1ess/CVE-2020-15099.svg)


## CVE-2020-12446
 The ene.sys driver in G.SKILL Trident Z Lighting Control through 1.00.08 exposes mapping and un-mapping of physical memory, reading and writing to Model Specific Register (MSR) registers, and input from and output to I/O ports to local non-privileged users. This leads to privilege escalation to NT AUTHORITY\SYSTEM.

- [https://github.com/enessakircolak/CVE-2020-12446](https://github.com/enessakircolak/CVE-2020-12446) :  ![starts](https://img.shields.io/github/stars/enessakircolak/CVE-2020-12446.svg) ![forks](https://img.shields.io/github/forks/enessakircolak/CVE-2020-12446.svg)


## CVE-2019-15107
 An issue was discovered in Webmin =1.920. The parameter old in password_change.cgi contains a command injection vulnerability.

- [https://github.com/adampawelczyk/CVE-2019-15107](https://github.com/adampawelczyk/CVE-2019-15107) :  ![starts](https://img.shields.io/github/stars/adampawelczyk/CVE-2019-15107.svg) ![forks](https://img.shields.io/github/forks/adampawelczyk/CVE-2019-15107.svg)

