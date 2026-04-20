# Update 2026-04-20
## CVE-2026-40487
 Postiz is an AI social media scheduling tool. Prior to version 2.21.6, a file upload validation bypass allows any authenticated user to upload arbitrary HTML, SVG, or other executable file types to the server by spoofing the `Content-Type` header. The uploaded files are then served by nginx with a Content-Type derived from their original extension (`text/html`, `image/svg+xml`), enabling Stored Cross-Site Scripting (XSS) in the context of the application's origin. This can lead to session riding, account takeover, and full compromise of other users' accounts. Version 2.21.6 contains a fix.

- [https://github.com/Astaruf/CVE-2026-40487](https://github.com/Astaruf/CVE-2026-40487) :  ![starts](https://img.shields.io/github/stars/Astaruf/CVE-2026-40487.svg) ![forks](https://img.shields.io/github/forks/Astaruf/CVE-2026-40487.svg)


## CVE-2026-39987
 marimo is a reactive Python notebook. Prior to 0.23.0, Marimo has a Pre-Auth RCE vulnerability. The terminal WebSocket endpoint /terminal/ws lacks authentication validation, allowing an unauthenticated attacker to obtain a full PTY shell and execute arbitrary system commands. Unlike other WebSocket endpoints (e.g., /ws) that correctly call validate_auth() for authentication, the /terminal/ws endpoint only checks the running mode and platform support before accepting connections, completely skipping authentication verification. This vulnerability is fixed in 0.23.0.

- [https://github.com/Nxploited/CVE-2026-39987](https://github.com/Nxploited/CVE-2026-39987) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-39987.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-39987.svg)


## CVE-2026-39808
 A improper neutralization of special elements used in an os command ('os command injection') vulnerability in Fortinet FortiSandbox 4.4.0 through 4.4.8 may allow attacker to execute unauthorized code or commands via insert attack vector here

- [https://github.com/0xBlackash/CVE-2026-39808](https://github.com/0xBlackash/CVE-2026-39808) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-39808.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-39808.svg)


## CVE-2026-33032
 Nginx UI is a web user interface for the Nginx web server. In versions 2.3.5 and prior, the nginx-ui MCP (Model Context Protocol) integration exposes two HTTP endpoints: /mcp and /mcp_message. While /mcp requires both IP whitelisting and authentication (AuthRequired() middleware), the /mcp_message endpoint only applies IP whitelisting - and the default IP whitelist is empty, which the middleware treats as "allow all". This means any network attacker can invoke all MCP tools without authentication, including restarting nginx, creating/modifying/deleting nginx configuration files, and triggering automatic config reloads - achieving complete nginx service takeover. At time of publication, there are no publicly available patches.

- [https://github.com/keraattin/CVE-2026-33032](https://github.com/keraattin/CVE-2026-33032) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-33032.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-33032.svg)


## CVE-2026-27542
 Incorrect Privilege Assignment vulnerability in Rymera Web Co Pty Ltd. Woocommerce Wholesale Lead Capture allows Privilege Escalation.This issue affects Woocommerce Wholesale Lead Capture: from n/a through 2.0.3.1.

- [https://github.com/Nxploited/CVE-2026-27542-CVE-2026-27540-](https://github.com/Nxploited/CVE-2026-27542-CVE-2026-27540-) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-27542-CVE-2026-27540-.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-27542-CVE-2026-27540-.svg)


## CVE-2026-27540
 Unrestricted Upload of File with Dangerous Type vulnerability in Rymera Web Co Pty Ltd. Woocommerce Wholesale Lead Capture allows Using Malicious Files.This issue affects Woocommerce Wholesale Lead Capture: from n/a through 2.0.3.1.

- [https://github.com/Nxploited/CVE-2026-27542-CVE-2026-27540-](https://github.com/Nxploited/CVE-2026-27542-CVE-2026-27540-) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-27542-CVE-2026-27540-.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-27542-CVE-2026-27540-.svg)


## CVE-2026-25253
 OpenClaw (aka clawdbot or Moltbot) before 2026.1.29 obtains a gatewayUrl value from a query string and automatically makes a WebSocket connection without prompting, sending a token value.

- [https://github.com/KajzingerAkos/CVE-2026-25253](https://github.com/KajzingerAkos/CVE-2026-25253) :  ![starts](https://img.shields.io/github/stars/KajzingerAkos/CVE-2026-25253.svg) ![forks](https://img.shields.io/github/forks/KajzingerAkos/CVE-2026-25253.svg)
- [https://github.com/Cyber-Warrior-Network/trust-gate-mcp](https://github.com/Cyber-Warrior-Network/trust-gate-mcp) :  ![starts](https://img.shields.io/github/stars/Cyber-Warrior-Network/trust-gate-mcp.svg) ![forks](https://img.shields.io/github/forks/Cyber-Warrior-Network/trust-gate-mcp.svg)


## CVE-2026-25232
 Gogs is an open source self-hosted Git service. Versions 0.13.4 and below have an access control bypass vulnerability which allows any repository collaborator with Write permissions to delete protected branches (including the default branch) by sending a direct POST request, completely bypassing the branch protection mechanism. This vulnerability in the DeleteBranchPost function eenables privilege escalation from Write to Admin level, allowing low-privilege users to perform dangerous operations that should be restricted to administrators only. Although Git Hook layer correctly prevents protected branch deletion via SSH push, the web interface deletion operation does not trigger Git Hooks, resulting in complete bypass of protection mechanisms. In oder to exploit this vulnerability, attackers must have write permissions to the target repository, protected branches configured to the target repository and access to the Gogs web interface. This issue has been fixed in version 0.14.1.

- [https://github.com/H1sok444/CVE-2026-25232-PoC](https://github.com/H1sok444/CVE-2026-25232-PoC) :  ![starts](https://img.shields.io/github/stars/H1sok444/CVE-2026-25232-PoC.svg) ![forks](https://img.shields.io/github/forks/H1sok444/CVE-2026-25232-PoC.svg)


## CVE-2026-24061
 telnetd in GNU Inetutils through 2.7 allows remote authentication bypass via a "-f root" value for the USER environment variable.

- [https://github.com/RStephanH/vuln-deb](https://github.com/RStephanH/vuln-deb) :  ![starts](https://img.shields.io/github/stars/RStephanH/vuln-deb.svg) ![forks](https://img.shields.io/github/forks/RStephanH/vuln-deb.svg)


## CVE-2026-22241
 The Open eClass platform (formerly known as GUnet eClass) is a complete course management system. Prior to version 4.2, an arbitrary file upload vulnerability in the theme import functionality enables an attacker with administrative privileges to upload arbitrary files on the server's file system. The main cause of the issue is that no validation or sanitization of the file's present inside the zip archive. This leads to remote code execution on the web server. Version 4.2 patches the issue.

- [https://github.com/0xBlackash/CVE-2026-22241](https://github.com/0xBlackash/CVE-2026-22241) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-22241.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-22241.svg)


## CVE-2026-4631
 Cockpit's remote login feature passes user-supplied hostnames and usernames from the web interface to the SSH client without validation or sanitization. An attacker with network access to the Cockpit web service can craft a single HTTP request to the login endpoint that injects malicious SSH options or shell commands, achieving code execution on the Cockpit host without valid credentials. The injection occurs during the authentication flow before any credential verification takes place, meaning no login is required to exploit the vulnerability.

- [https://github.com/cyberheartmi9/CVE-2026-4631-cockpit-RCE](https://github.com/cyberheartmi9/CVE-2026-4631-cockpit-RCE) :  ![starts](https://img.shields.io/github/stars/cyberheartmi9/CVE-2026-4631-cockpit-RCE.svg) ![forks](https://img.shields.io/github/forks/cyberheartmi9/CVE-2026-4631-cockpit-RCE.svg)


## CVE-2026-4484
 The Masteriyo LMS plugin for WordPress is vulnerable to Privilege Escalation in all versions up to, and including, 2.1.6. This is due to the plugin allowing a user to update the user role through the 'InstructorsController::prepare_object_for_database' function. This makes it possible for authenticated attackers, with Student-level access and above, to elevate their privileges to that of an administrator.

- [https://github.com/Nxploited/CVE-2026-4484](https://github.com/Nxploited/CVE-2026-4484) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-4484.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-4484.svg)


## CVE-2026-4257
 The Contact Form by Supsystic plugin for WordPress is vulnerable to Server-Side Template Injection (SSTI) leading to Remote Code Execution (RCE) in all versions up to, and including, 1.7.36. This is due to the plugin using the Twig `Twig_Loader_String` template engine without sandboxing, combined with the `cfsPreFill` prefill functionality that allows unauthenticated users to inject arbitrary Twig expressions into form field values via GET parameters. This makes it possible for unauthenticated attackers to execute arbitrary PHP functions and OS commands on the server by leveraging Twig's `registerUndefinedFilterCallback()` method to register arbitrary PHP callbacks.

- [https://github.com/0xgh057r3c0n/CVE-2026-4257](https://github.com/0xgh057r3c0n/CVE-2026-4257) :  ![starts](https://img.shields.io/github/stars/0xgh057r3c0n/CVE-2026-4257.svg) ![forks](https://img.shields.io/github/forks/0xgh057r3c0n/CVE-2026-4257.svg)


## CVE-2026-1937
 The YayMail – WooCommerce Email Customizer plugin for WordPress is vulnerable to unauthorized modification of data that can lead to privilege escalation due to a missing capability check on the `yaymail_import_state` AJAX action in all versions up to, and including, 4.3.2. This makes it possible for authenticated attackers, with Shop Manager-level access and above, to update arbitrary options on the WordPress site. This can be leveraged to update the default role for registration to administrator and enable user registration for attackers to gain administrative user access to a vulnerable site.

- [https://github.com/Nxploited/CVE-2026-1937](https://github.com/Nxploited/CVE-2026-1937) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-1937.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-1937.svg)


## CVE-2026-1492
 The User Registration & Membership – Custom Registration Form Builder, Custom Login Form, User Profile, Content Restriction & Membership Plugin plugin for WordPress is vulnerable to improper privilege management in all versions up to, and including, 5.1.2. This is due to the plugin accepting a user-supplied role during membership registration without properly enforcing a server-side allowlist. This makes it possible for unauthenticated attackers to create administrator accounts by supplying a role value during membership registration.

- [https://github.com/Nxploited/CVE-2026-1492](https://github.com/Nxploited/CVE-2026-1492) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-1492.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-1492.svg)


## CVE-2026-0920
 The LA-Studio Element Kit for Elementor plugin for WordPress is vulnerable to Administrative User Creation in all versions up to, and including, 1.5.6.3. This is due to the 'ajax_register_handle' function not restricting what user roles a user can register with. This makes it possible for unauthenticated attackers to supply the 'lakit_bkrole' parameter during registration and gain administrator access to the site.

- [https://github.com/Nxploited/CVE-2026-0920-](https://github.com/Nxploited/CVE-2026-0920-) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2026-0920-.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2026-0920-.svg)


## CVE-2025-68001
 Unrestricted Upload of File with Dangerous Type vulnerability in garidium g-FFL Checkout g-ffl-checkout allows Upload a Web Shell to a Web Server.This issue affects g-FFL Checkout: from n/a through = 2.1.0.

- [https://github.com/Nxploited/CVE-2025-68001](https://github.com/Nxploited/CVE-2025-68001) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-68001.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-68001.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg)


## CVE-2025-53580
 Incorrect Privilege Assignment vulnerability in quantumcloud Simple Business Directory Pro simple-business-directory-pro allows Privilege Escalation.This issue affects Simple Business Directory Pro: from n/a through  15.6.9.

- [https://github.com/Nxploited/CVE-2025-53580](https://github.com/Nxploited/CVE-2025-53580) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-53580.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-53580.svg)


## CVE-2025-49901
 Authentication Bypass Using an Alternate Path or Channel vulnerability in quantumcloud Simple Link Directory qc-simple-link-directory allows Authentication Abuse.This issue affects Simple Link Directory: from n/a through  14.8.1.

- [https://github.com/Nxploited/CVE-2025-49901](https://github.com/Nxploited/CVE-2025-49901) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-49901.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-49901.svg)


## CVE-2025-29009
 Unrestricted Upload of File with Dangerous Type vulnerability in Webkul Medical Prescription Attachment Plugin for WooCommerce medical-prescription-attachment-plugin-for-woocommerce allows Upload a Web Shell to a Web Server.This issue affects Medical Prescription Attachment Plugin for WooCommerce: from n/a through = 1.2.3.

- [https://github.com/Nxploited/CVE-2025-29009](https://github.com/Nxploited/CVE-2025-29009) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-29009.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-29009.svg)


## CVE-2025-15521
 The Academy LMS – WordPress LMS Plugin for Complete eLearning Solution plugin for WordPress is vulnerable to privilege escalation via account takeover in all versions up to, and including, 3.5.0. This is due to the plugin not properly validating a user's identity prior to updating their password and relying solely on a publicly-exposed nonce for authorization. This makes it possible for unauthenticated attackers to change arbitrary user's password, including administrators, and gain access to their account.

- [https://github.com/Nxploited/CVE-2025-15521](https://github.com/Nxploited/CVE-2025-15521) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-15521.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-15521.svg)


## CVE-2025-15403
 The RegistrationMagic plugin for WordPress is vulnerable to Privilege Escalation in all versions up to, and including, 6.0.7.1. This is due to the 'add_menu' function is accessible via the 'rm_user_exists' AJAX action and allows arbitrary updates to the 'admin_order' setting. This makes it possible for unauthenticated attackers to injecting an empty slug into the order parameter, and manipulate the plugin's menu generation logic, and when the admin menu is subsequently built, the plugin adds 'manage_options' capability for the target role. Note: The vulnerability can only be exploited unauthenticated, but further privilege escalation requires at least a subscriber user.

- [https://github.com/Nxploited/CVE-2025-15403](https://github.com/Nxploited/CVE-2025-15403) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-15403.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-15403.svg)


## CVE-2025-15030
 The User Profile Builder  WordPress plugin before 3.15.2 does not have a proper password reset process, allowing a few unauthenticated requests to reset the password of any user by knowing their username, such as administrator ones, and therefore gain access to their account

- [https://github.com/Nxploited/CVE-2025-15030](https://github.com/Nxploited/CVE-2025-15030) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-15030.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-15030.svg)


## CVE-2025-14364
 The Demo Importer Plus plugin for WordPress is vulnerable to unauthorized modification of data, loss of data, and privilege escalation due to a missing capability check on the Ajax::handle_request() function in all versions up to, and including, 2.0.8. This makes it possible for authenticated attackers, with Subscriber-level access and above, to trigger a full site reset, dropping all database tables except users/usermeta and re-running wp_install(), which also assigns the Administrator role to the attacking subscriber account.

- [https://github.com/Nxploited/CVE-2025-14364](https://github.com/Nxploited/CVE-2025-14364) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-14364.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-14364.svg)


## CVE-2025-13342
 The Frontend Admin by DynamiApps plugin for WordPress is vulnerable to unauthorized modification of arbitrary WordPress options in all versions up to, and including, 3.28.20. This is due to insufficient capability checks and input validation in the ActionOptions::run() save handler. This makes it possible for unauthenticated attackers to modify critical WordPress options such as users_can_register, default_role, and admin_email via submitting crafted form data to public frontend forms.

- [https://github.com/Nxploited/CVE-2025-13342](https://github.com/Nxploited/CVE-2025-13342) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-13342.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-13342.svg)


## CVE-2025-6389
 The Sneeit Framework plugin for WordPress is vulnerable to Remote Code Execution in all versions up to, and including, 8.3 via the sneeit_articles_pagination_callback() function. This is due to the function accepting user input and then passing that through call_user_func(). This makes it possible for unauthenticated attackers to execute code on the server which can be leveraged to inject backdoors or, for example, create new administrative user accounts.

- [https://github.com/Nxploited/CVE-2025-6389](https://github.com/Nxploited/CVE-2025-6389) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-6389.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-6389.svg)


## CVE-2025-5450
 Improper access control in the certificate management component of Ivanti Connect Secure before version 22.7R2.8 and Ivanti Policy Secure before version 22.7R1.5 allows a remote authenticated admin with read-only rights to modify settings that should be restricted.

- [https://github.com/siltyy/cve-2025-54505-fix](https://github.com/siltyy/cve-2025-54505-fix) :  ![starts](https://img.shields.io/github/stars/siltyy/cve-2025-54505-fix.svg) ![forks](https://img.shields.io/github/forks/siltyy/cve-2025-54505-fix.svg)


## CVE-2025-2563
 The User Registration & Membership  WordPress plugin before 4.1.2 does not prevent users to set their account role when the Membership Addon is enabled, leading to a privilege escalation issue and allowing unauthenticated users to gain admin privileges

- [https://github.com/Nxploited/CVE-2025-2563](https://github.com/Nxploited/CVE-2025-2563) :  ![starts](https://img.shields.io/github/stars/Nxploited/CVE-2025-2563.svg) ![forks](https://img.shields.io/github/forks/Nxploited/CVE-2025-2563.svg)


## CVE-2023-24329
 An issue in the urllib.parse component of Python before 3.11.4 allows attackers to bypass blocklisting methods by supplying a URL that starts with blank characters.

- [https://github.com/jithinodattu/CVE-2023-24329-lab](https://github.com/jithinodattu/CVE-2023-24329-lab) :  ![starts](https://img.shields.io/github/stars/jithinodattu/CVE-2023-24329-lab.svg) ![forks](https://img.shields.io/github/forks/jithinodattu/CVE-2023-24329-lab.svg)


## CVE-2021-42278
 Active Directory Domain Services Elevation of Privilege Vulnerability

- [https://github.com/johnson2849/kern](https://github.com/johnson2849/kern) :  ![starts](https://img.shields.io/github/stars/johnson2849/kern.svg) ![forks](https://img.shields.io/github/forks/johnson2849/kern.svg)


## CVE-2021-40449
 Win32k Elevation of Privilege Vulnerability

- [https://github.com/johnson2849/kern](https://github.com/johnson2849/kern) :  ![starts](https://img.shields.io/github/stars/johnson2849/kern.svg) ![forks](https://img.shields.io/github/forks/johnson2849/kern.svg)


## CVE-2021-40444
pstrongUPDATE/strong September 14, 2021: Microsoft has released security updates to address this vulnerability. Please see the Security Updates table for the applicable update for your system. We recommend that you install these updates immediately. Please see the FAQ for important information about which updates are applicable to your system./p

- [https://github.com/johnson2849/kern](https://github.com/johnson2849/kern) :  ![starts](https://img.shields.io/github/stars/johnson2849/kern.svg) ![forks](https://img.shields.io/github/forks/johnson2849/kern.svg)


## CVE-2018-17081
 e107 2.1.9 allows CSRF via e107_admin/wmessage.php?mode=&action=inline&ajax_used=1&id= for changing the title of an arbitrary page.

- [https://github.com/himanshurahi1996/e107_2.1.9_CSRF_POC](https://github.com/himanshurahi1996/e107_2.1.9_CSRF_POC) :  ![starts](https://img.shields.io/github/stars/himanshurahi1996/e107_2.1.9_CSRF_POC.svg) ![forks](https://img.shields.io/github/forks/himanshurahi1996/e107_2.1.9_CSRF_POC.svg)


## CVE-2017-11176
 The mq_notify function in the Linux kernel through 4.11.9 does not set the sock pointer to NULL upon entry into the retry logic. During a user-space close of a Netlink socket, it allows attackers to cause a denial of service (use-after-free) or possibly have unspecified other impact.

- [https://github.com/Cyb3rCr0wCC/cve-2017-11176](https://github.com/Cyb3rCr0wCC/cve-2017-11176) :  ![starts](https://img.shields.io/github/stars/Cyb3rCr0wCC/cve-2017-11176.svg) ![forks](https://img.shields.io/github/forks/Cyb3rCr0wCC/cve-2017-11176.svg)

