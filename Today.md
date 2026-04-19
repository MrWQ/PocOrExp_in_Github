# Update 2026-04-19
## CVE-2026-40261
 Composer is a dependency manager for PHP. Versions 1.0 through 2.2.26 and 2.3 through 2.9.5 contain a command injection vulnerability in the Perforce::syncCodeBase() method, which appends the $sourceReference parameter to a shell command without proper escaping, and additionally in the Perforce::generateP4Command() method as in GHSA-wg36-wvj6-r67p / CVE-2026-40176, which interpolates user-supplied Perforce connection parameters (port, user, client) from the source url field without proper escaping. An attacker can inject arbitrary commands through crafted source reference or source url values containing shell metacharacters, even if Perforce is not installed. Unlike CVE-2026-40176, the source reference and url are provided as part of package metadata, meaning any compromised or malicious Composer repository can serve package metadata declaring perforce as a source type with malicious values. This vulnerability is exploitable when installing or updating dependencies from source, including the default behavior when installing dev-prefixed versions. This issue has been fixed in Composer 2.2.27 (2.2 LTS) and 2.9.6 (mainline). If developers are unable to immediately update, they can avoid installing dependencies from source by using --prefer-dist or the preferred-install: dist config setting, and only use trusted Composer repositories as a workaround.

- [https://github.com/daptheHuman/cve-2026-40176-cve-2026-40261](https://github.com/daptheHuman/cve-2026-40176-cve-2026-40261) :  ![starts](https://img.shields.io/github/stars/daptheHuman/cve-2026-40176-cve-2026-40261.svg) ![forks](https://img.shields.io/github/forks/daptheHuman/cve-2026-40176-cve-2026-40261.svg)


## CVE-2026-40176
 Composer is a dependency manager for PHP. Versions 1.0 through 2.2.26 and 2.3 through 2.9.5 contain a command injection vulnerability in the Perforce::generateP4Command() method, which constructs shell commands by interpolating user-supplied Perforce connection parameters (port, user, client) without proper escaping. An attacker can inject arbitrary commands through these values in a malicious composer.json declaring a Perforce VCS repository, leading to command execution in the context of the user running Composer, even if Perforce is not installed. VCS repositories are only loaded from the root composer.json or the composer config directory, so this cannot be exploited through composer.json files of packages installed as dependencies. Users are at risk if they run Composer commands on untrusted projects with attacker-supplied composer.json files. This issue has been fixed in Composer 2.2.27 (2.2 LTS) and 2.9.6 (mainline).

- [https://github.com/daptheHuman/cve-2026-40176-cve-2026-40261](https://github.com/daptheHuman/cve-2026-40176-cve-2026-40261) :  ![starts](https://img.shields.io/github/stars/daptheHuman/cve-2026-40176-cve-2026-40261.svg) ![forks](https://img.shields.io/github/forks/daptheHuman/cve-2026-40176-cve-2026-40261.svg)


## CVE-2026-40175
 Axios is a promise based HTTP client for the browser and Node.js. Prior to 1.15.0 and 0.3.1, the Axios library is vulnerable to a specific "Gadget" attack chain that allows Prototype Pollution in any third-party dependency to be escalated into Remote Code Execution (RCE) or Full Cloud Compromise (via AWS IMDSv2 bypass). This vulnerability is fixed in 1.15.0 and 0.3.1.

- [https://github.com/pjt3591oo/CVE-2026-40175-poc](https://github.com/pjt3591oo/CVE-2026-40175-poc) :  ![starts](https://img.shields.io/github/stars/pjt3591oo/CVE-2026-40175-poc.svg) ![forks](https://img.shields.io/github/forks/pjt3591oo/CVE-2026-40175-poc.svg)


## CVE-2026-39842
 OpenRemote is an open-source IoT platform. Versions 1.21.0 and below contain two interrelated expression injection vulnerabilities in the rules engine that allow arbitrary code execution on the server. The JavaScript rules engine executes user-supplied scripts via Nashorn's ScriptEngine.eval() without sandboxing, class filtering, or access restrictions, and the authorization check in RulesResourceImpl only restricts Groovy rules to superusers while leaving JavaScript rules unrestricted for any user with the write:rules role. Additionally, the Groovy rules engine has a GroovyDenyAllFilter security filter that is defined but never registered, as the registration code is commented out, rendering the SandboxTransformer ineffective for superuser-created Groovy rules. A non-superuser attacker with the write:rules role can create JavaScript rulesets that execute with full JVM access, enabling remote code execution as root, arbitrary file read, environment variable theft including database credentials, and complete multi-tenant isolation bypass to access data across all realms. This issue has been fixed in version 1.22.0.

- [https://github.com/keraattin/CVE-2026-39842](https://github.com/keraattin/CVE-2026-39842) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-39842.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-39842.svg)


## CVE-2026-37749
 A SQL injection vulnerability in CodeAstro Simple Attendance Management System v1.0 allows remote unauthenticated attackers to bypass authentication via the username parameter in index.php.

- [https://github.com/menevarad007/CVE-2026-37749](https://github.com/menevarad007/CVE-2026-37749) :  ![starts](https://img.shields.io/github/stars/menevarad007/CVE-2026-37749.svg) ![forks](https://img.shields.io/github/forks/menevarad007/CVE-2026-37749.svg)


## CVE-2026-34621
 Acrobat Reader versions 24.001.30356, 26.001.21367 and earlier are affected by an Improperly Controlled Modification of Object Prototype Attributes ('Prototype Pollution') vulnerability that could result in arbitrary code execution in the context of the current user. Exploitation of this issue requires user interaction in that a victim must open a malicious file.

- [https://github.com/ercihan/CVE-2026-34621_PDF_SAMPLE](https://github.com/ercihan/CVE-2026-34621_PDF_SAMPLE) :  ![starts](https://img.shields.io/github/stars/ercihan/CVE-2026-34621_PDF_SAMPLE.svg) ![forks](https://img.shields.io/github/forks/ercihan/CVE-2026-34621_PDF_SAMPLE.svg)


## CVE-2026-33825
 Insufficient granularity of access control in Microsoft Defender allows an authorized attacker to elevate privileges locally.

- [https://github.com/Letlaka/redsun-bluehammer-undefend-detection-pack](https://github.com/Letlaka/redsun-bluehammer-undefend-detection-pack) :  ![starts](https://img.shields.io/github/stars/Letlaka/redsun-bluehammer-undefend-detection-pack.svg) ![forks](https://img.shields.io/github/forks/Letlaka/redsun-bluehammer-undefend-detection-pack.svg)


## CVE-2026-33671
 Picomatch is a glob matcher written JavaScript. Versions prior to 4.0.4, 3.0.2, and 2.3.2 are vulnerable to Regular Expression Denial of Service (ReDoS) when processing crafted extglob patterns. Certain patterns using extglob quantifiers such as `+()` and `*()`, especially when combined with overlapping alternatives or nested extglobs, are compiled into regular expressions that can exhibit catastrophic backtracking on non-matching input. Applications are impacted when they allow untrusted users to supply glob patterns that are passed to `picomatch` for compilation or matching. In those cases, an attacker can cause excessive CPU consumption and block the Node.js event loop, resulting in a denial of service. Applications that only use trusted, developer-controlled glob patterns are much less likely to be exposed in a security-relevant way. This issue is fixed in picomatch 4.0.4, 3.0.2 and 2.3.2. Users should upgrade to one of these versions or later, depending on their supported release line. If upgrading is not immediately possible, avoid passing untrusted glob patterns to `picomatch`. Possible mitigations include disabling extglob support for untrusted patterns by using `noextglob: true`, rejecting or sanitizing patterns containing nested extglobs or extglob quantifiers such as `+()` and `*()`, enforcing strict allowlists for accepted pattern syntax, running matching in an isolated worker or separate process with time and resource limits, and applying application-level request throttling and input validation for any endpoint that accepts glob patterns.

- [https://github.com/BeLazy167/next-picomatch-cve-repro](https://github.com/BeLazy167/next-picomatch-cve-repro) :  ![starts](https://img.shields.io/github/stars/BeLazy167/next-picomatch-cve-repro.svg) ![forks](https://img.shields.io/github/forks/BeLazy167/next-picomatch-cve-repro.svg)


## CVE-2026-33032
 Nginx UI is a web user interface for the Nginx web server. In versions 2.3.5 and prior, the nginx-ui MCP (Model Context Protocol) integration exposes two HTTP endpoints: /mcp and /mcp_message. While /mcp requires both IP whitelisting and authentication (AuthRequired() middleware), the /mcp_message endpoint only applies IP whitelisting - and the default IP whitelist is empty, which the middleware treats as "allow all". This means any network attacker can invoke all MCP tools without authentication, including restarting nginx, creating/modifying/deleting nginx configuration files, and triggering automatic config reloads - achieving complete nginx service takeover. At time of publication, there are no publicly available patches.

- [https://github.com/Shreda/CVE-2026-33032-nginx-ui-vuln-lab](https://github.com/Shreda/CVE-2026-33032-nginx-ui-vuln-lab) :  ![starts](https://img.shields.io/github/stars/Shreda/CVE-2026-33032-nginx-ui-vuln-lab.svg) ![forks](https://img.shields.io/github/forks/Shreda/CVE-2026-33032-nginx-ui-vuln-lab.svg)


## CVE-2026-29000
 pac4j-jwt versions prior to 4.5.9, 5.7.9, and 6.3.3 contain an authentication bypass vulnerability in JwtAuthenticator when processing encrypted JWTs that allows remote attackers to forge authentication tokens. Attackers who possess the server's RSA public key can create a JWE-wrapped PlainJWT with arbitrary subject and role claims, bypassing signature verification to authenticate as any user including administrators.

- [https://github.com/cipher1x1/CVE-2026-29000](https://github.com/cipher1x1/CVE-2026-29000) :  ![starts](https://img.shields.io/github/stars/cipher1x1/CVE-2026-29000.svg) ![forks](https://img.shields.io/github/forks/cipher1x1/CVE-2026-29000.svg)


## CVE-2026-26980
 Ghost is a Node.js content management system. Versions 3.24.0 through 6.19.0 allow unauthenticated attackers to perform arbitrary reads from the database. This issue has been fixed in version 6.19.1.

- [https://github.com/dinosn/ghost-cve-2026-26980](https://github.com/dinosn/ghost-cve-2026-26980) :  ![starts](https://img.shields.io/github/stars/dinosn/ghost-cve-2026-26980.svg) ![forks](https://img.shields.io/github/forks/dinosn/ghost-cve-2026-26980.svg)


## CVE-2026-23500
 Dolibarr is an enterprise resource planning (ERP) and customer relationship management (CRM) software package. In versions prior to 23.0.0 , the ODT to PDF conversion process in odf.php concatenates the MAIN_ODT_AS_PDF configuration constant directly into a shell command passed to exec() without sanitization. An authenticated administrator can inject arbitrary OS commands via this constant using command separators, achieving remote code execution as the web server user when any ODT template is generated. This issue has been fixed in version 23.0.0.

- [https://github.com/lukasz-rybak/CVE-2026-23500](https://github.com/lukasz-rybak/CVE-2026-23500) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-23500.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-23500.svg)


## CVE-2026-2631
 The Datalogics Ecommerce Delivery  WordPress plugin before 2.6.60 exposes an unauthenticated REST endpoint that allows any remote user to modify the option `datalogics_token` without verification. This token is subsequently used for authentication in a protected endpoint that allows users to perform arbitrary WordPress `update_option()` operations. Attackers can use this to enable registartion and to set the default role as Administrator.

- [https://github.com/AnggaTechI/Mass-Scanner-CVE-2026-2631](https://github.com/AnggaTechI/Mass-Scanner-CVE-2026-2631) :  ![starts](https://img.shields.io/github/stars/AnggaTechI/Mass-Scanner-CVE-2026-2631.svg) ![forks](https://img.shields.io/github/forks/AnggaTechI/Mass-Scanner-CVE-2026-2631.svg)


## CVE-2026-1555
 The WebStack theme for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the io_img_upload() function in all versions up to, and including, 1.2024. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/Nxploited/CVE-2026-1555](https://github.com/Nxploited/CVE-2026-1555) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-1555.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-1555.svg)


## CVE-2026-1492
 The User Registration & Membership – Custom Registration Form Builder, Custom Login Form, User Profile, Content Restriction & Membership Plugin plugin for WordPress is vulnerable to improper privilege management in all versions up to, and including, 5.1.2. This is due to the plugin accepting a user-supplied role during membership registration without properly enforcing a server-side allowlist. This makes it possible for unauthenticated attackers to create administrator accounts by supplying a role value during membership registration.

- [https://github.com/imad-z1/CVE-2026-1492-POC](https://github.com/imad-z1/CVE-2026-1492-POC) :  ![starts](https://img.shields.io/github/stars/imad-z1/CVE-2026-1492-POC.svg) ![forks](https://img.shields.io/github/forks/imad-z1/CVE-2026-1492-POC.svg)


## CVE-2026-1405
 The Slider Future plugin for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the 'slider_future_handle_image_upload' function in all versions up to, and including, 1.0.5. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible.

- [https://github.com/AnggaTechI/Mass-Scanner-CVE-2026-1405](https://github.com/AnggaTechI/Mass-Scanner-CVE-2026-1405) :  ![starts](https://img.shields.io/github/stars/AnggaTechI/Mass-Scanner-CVE-2026-1405.svg) ![forks](https://img.shields.io/github/forks/AnggaTechI/Mass-Scanner-CVE-2026-1405.svg)


## CVE-2026-0740
 The Ninja Forms - File Uploads plugin for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the 'NF_FU_AJAX_Controllers_Uploads::handle_upload' function in all versions up to, and including, 3.3.26. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible. Note: The vulnerability was partially patched in version 3.3.25 and fully patched in version 3.3.27.

- [https://github.com/0xgh057r3c0n/CVE-2026-0740](https://github.com/0xgh057r3c0n/CVE-2026-0740) :  ![starts](https://img.shields.io/github/stars/0xgh057r3c0n/CVE-2026-0740.svg) ![forks](https://img.shields.io/github/forks/0xgh057r3c0n/CVE-2026-0740.svg)


## CVE-2025-70795
 STProcessMonitor 11.11.4.0, part of the Safetica Application suite, allows an admin-privileged user to send crafted IOCTL requests to terminate processes that are protected through a third-party implementation. This is caused by insufficient caller validation in the driver's IOCTL handler, enabling unauthorized processes to perform those actions in kernel space. Successful exploitation can lead to denial of service by disrupting critical third-party services or applications. Unauthorized processes load the driver and send a crafted IOCTL request (0xB822200C) to terminate processes protected by a third-party implementation. This action exploits insufficient caller validation in the driver's IOCTL handler, allowing unauthorized processes to perform termination operations in kernel space. Successful exploitation can lead to denial of service by disrupting critical third-party services or applications.

- [https://github.com/ANYLNK/STProcessMonitorBYOVD](https://github.com/ANYLNK/STProcessMonitorBYOVD) :  ![starts](https://img.shields.io/github/stars/ANYLNK/STProcessMonitorBYOVD.svg) ![forks](https://img.shields.io/github/forks/ANYLNK/STProcessMonitorBYOVD.svg)
- [https://github.com/wutang700/STProcessMonitorBYOVD](https://github.com/wutang700/STProcessMonitorBYOVD) :  ![starts](https://img.shields.io/github/stars/wutang700/STProcessMonitorBYOVD.svg) ![forks](https://img.shields.io/github/forks/wutang700/STProcessMonitorBYOVD.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-55182
 A pre-authentication remote code execution vulnerability exists in React Server Components versions 19.0.0, 19.1.0, 19.1.1, and 19.2.0 including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints.

- [https://github.com/rubensuxo-eh/react2shell-exploit](https://github.com/rubensuxo-eh/react2shell-exploit) :  ![starts](https://img.shields.io/github/stars/rubensuxo-eh/react2shell-exploit.svg) ![forks](https://img.shields.io/github/forks/rubensuxo-eh/react2shell-exploit.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927](https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/sn1p3rt3s7/NextJS_CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/sn1p3rt3s7/NextJS_CVE-2025-29927.svg)


## CVE-2025-20282
This vulnerability is due a lack of file validation checks that would prevent uploaded files from being placed in privileged directories on an affected system. An attacker could exploit this vulnerability by uploading a crafted file to the affected device. A successful exploit could allow the attacker to store malicious files on the affected system and then execute arbitrary code or obtain root privileges on the system.

- [https://github.com/biggerbangg/cve-2025-20282](https://github.com/biggerbangg/cve-2025-20282) :  ![starts](https://img.shields.io/github/stars/biggerbangg/cve-2025-20282.svg) ![forks](https://img.shields.io/github/forks/biggerbangg/cve-2025-20282.svg)


## CVE-2025-7771
 ThrottleStop.sys, a legitimate driver, exposes two IOCTL interfaces that allow arbitrary read and write access to physical memory via the MmMapIoSpace function. This insecure implementation can be exploited by a malicious user-mode application to patch the running Windows kernel and invoke arbitrary kernel functions with ring-0 privileges. The vulnerability enables local attackers to execute arbitrary code in kernel context, resulting in privilege escalation and potential follow-on attacks, such as disabling security software or bypassing kernel-level protections. ThrottleStop.sys version 3.0.0.0 and possibly others are affected. Apply updates per vendor instructions.

- [https://github.com/D4rkks/CVE-2025-7771-Vulnerability-Exploration](https://github.com/D4rkks/CVE-2025-7771-Vulnerability-Exploration) :  ![starts](https://img.shields.io/github/stars/D4rkks/CVE-2025-7771-Vulnerability-Exploration.svg) ![forks](https://img.shields.io/github/forks/D4rkks/CVE-2025-7771-Vulnerability-Exploration.svg)


## CVE-2025-6695
 A vulnerability was found in LabRedesCefetRJ WeGIA 3.4.0 and classified as problematic. This issue affects some unknown processing of the file /html/matPat/adicionar_categoria.php of the component Additional Categoria. The manipulation of the argument Insira a nova categoria leads to cross site scripting. The attack may be initiated remotely. The exploit has been disclosed to the public and may be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/DBmonster19/CVE-2025-66954](https://github.com/DBmonster19/CVE-2025-66954) :  ![starts](https://img.shields.io/github/stars/DBmonster19/CVE-2025-66954.svg) ![forks](https://img.shields.io/github/forks/DBmonster19/CVE-2025-66954.svg)


## CVE-2025-4322
 The Motors theme for WordPress is vulnerable to privilege escalation via account takeover in all versions up to, and including, 5.6.67. This is due to the theme not properly validating a user's identity prior to updating their password. This makes it possible for unauthenticated attackers to change arbitrary user passwords, including those of administrators, and leverage that to gain access to their account.

- [https://github.com/zedeq/WP-CVE-2025-4322---Scan](https://github.com/zedeq/WP-CVE-2025-4322---Scan) :  ![starts](https://img.shields.io/github/stars/zedeq/WP-CVE-2025-4322---Scan.svg) ![forks](https://img.shields.io/github/forks/zedeq/WP-CVE-2025-4322---Scan.svg)


## CVE-2024-45496
 A flaw was found in OpenShift. This issue occurs due to the misuse of elevated privileges in the OpenShift Container Platform's build process. During the build initialization step, the git-clone container is run with a privileged security context, allowing unrestricted access to the node. An attacker with developer-level access can provide a crafted .gitconfig file containing commands executed during the cloning process, leading to arbitrary command execution on the worker node. An attacker running code in a privileged container could escalate their permissions on the node running the container.

- [https://github.com/biggerbangg/cve-2024-45496](https://github.com/biggerbangg/cve-2024-45496) :  ![starts](https://img.shields.io/github/stars/biggerbangg/cve-2024-45496.svg) ![forks](https://img.shields.io/github/forks/biggerbangg/cve-2024-45496.svg)


## CVE-2024-7387
 A flaw was found in openshift/builder. This vulnerability allows command injection via path traversal, where a malicious user can execute arbitrary commands on the OpenShift node running the builder container. When using the “Docker” strategy, executable files inside the privileged build container can be overridden using the `spec.source.secrets.secret.destinationDir` attribute of the `BuildConfig` definition. An attacker running code in a privileged container could escalate their permissions on the node running the container.

- [https://github.com/biggerbangg/cve-2024-7387](https://github.com/biggerbangg/cve-2024-7387) :  ![starts](https://img.shields.io/github/stars/biggerbangg/cve-2024-7387.svg) ![forks](https://img.shields.io/github/forks/biggerbangg/cve-2024-7387.svg)


## CVE-2023-27163
 request-baskets up to v1.2.1 was discovered to contain a Server-Side Request Forgery (SSRF) via the component /api/baskets/{name}. This vulnerability allows attackers to access network resources and sensitive information via a crafted API request.

- [https://github.com/tombstoneghost/htb-sau-exploit-chain](https://github.com/tombstoneghost/htb-sau-exploit-chain) :  ![starts](https://img.shields.io/github/stars/tombstoneghost/htb-sau-exploit-chain.svg) ![forks](https://img.shields.io/github/forks/tombstoneghost/htb-sau-exploit-chain.svg)


## CVE-2021-25337
 Improper access control in clipboard service in Samsung mobile devices prior to SMR Mar-2021 Release 1 allows untrusted applications to read or write certain local files.

- [https://github.com/CrisZalSa/JustALampNothingElse](https://github.com/CrisZalSa/JustALampNothingElse) :  ![starts](https://img.shields.io/github/stars/CrisZalSa/JustALampNothingElse.svg) ![forks](https://img.shields.io/github/forks/CrisZalSa/JustALampNothingElse.svg)


## CVE-2021-3560
 It was found that polkit could be tricked into bypassing the credential checks for D-Bus requests, elevating the privileges of the requestor to the root user. This flaw could be used by an unprivileged local attacker to, for example, create a new local administrator. The highest threat from this vulnerability is to data confidentiality and integrity as well as system availability.

- [https://github.com/yutasato88/CVE-2021-3560-PolkitPrivilegeEsclation](https://github.com/yutasato88/CVE-2021-3560-PolkitPrivilegeEsclation) :  ![starts](https://img.shields.io/github/stars/yutasato88/CVE-2021-3560-PolkitPrivilegeEsclation.svg) ![forks](https://img.shields.io/github/forks/yutasato88/CVE-2021-3560-PolkitPrivilegeEsclation.svg)


## CVE-2019-9053
 An issue was discovered in CMS Made Simple 2.2.8. It is possible with the News module, through a crafted URL, to achieve unauthenticated blind time-based SQL injection via the m1_idlist parameter.

- [https://github.com/coolkiee/CVE-2019-9053](https://github.com/coolkiee/CVE-2019-9053) :  ![starts](https://img.shields.io/github/stars/coolkiee/CVE-2019-9053.svg) ![forks](https://img.shields.io/github/forks/coolkiee/CVE-2019-9053.svg)


## CVE-2007-2447
 The MS-RPC functionality in smbd in Samba 3.0.0 through 3.0.25rc3 allows remote attackers to execute arbitrary commands via shell metacharacters involving the (1) SamrChangePassword function, when the "username map script" smb.conf option is enabled, and allows remote authenticated users to execute commands via shell metacharacters involving other MS-RPC functions in the (2) remote printer and (3) file share management.

- [https://github.com/Daviddoctor/Samba-CVE-2007-2447-Exploit-Username-Map-Script](https://github.com/Daviddoctor/Samba-CVE-2007-2447-Exploit-Username-Map-Script) :  ![starts](https://img.shields.io/github/stars/Daviddoctor/Samba-CVE-2007-2447-Exploit-Username-Map-Script.svg) ![forks](https://img.shields.io/github/forks/Daviddoctor/Samba-CVE-2007-2447-Exploit-Username-Map-Script.svg)

