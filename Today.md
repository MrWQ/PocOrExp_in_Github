# Update 2026-03-25
## CVE-2026-24516
 A command injection vulnerability exists in DigitalOcean Droplet Agent through 1.3.2. The troubleshooting actioner component (internal/troubleshooting/actioner/actioner.go) processes metadata from the metadata service endpoint and executes commands specified in the TroubleshootingAgent.Requesting array without adequate input validation. While the code validates that artifacts exist in the validInvestigationArtifacts map, it fails to sanitize the actual command content after the "command:" prefix. This allows an attacker who can control metadata responses to inject and execute arbitrary OS commands with root privileges. The attack is triggered by sending a TCP packet with specific sequence numbers to the SSH port, which causes the agent to fetch metadata from http://169.254.169.254/metadata/v1.json. The vulnerability affects the command execution flow in internal/troubleshooting/actioner/actioner.go (insufficient validation), internal/troubleshooting/command/exec.go (direct exec.CommandContext call), and internal/troubleshooting/command/command.go (command parsing without sanitization). This can lead to complete system compromise, data exfiltration, privilege escalation, and potential lateral movement across cloud infrastructure.

- [https://github.com/poxsky/CVE-2026-24516-DigitalOcean-RCE](https://github.com/poxsky/CVE-2026-24516-DigitalOcean-RCE) :  ![starts](https://img.shields.io/github/stars/poxsky/CVE-2026-24516-DigitalOcean-RCE.svg) ![forks](https://img.shields.io/github/forks/poxsky/CVE-2026-24516-DigitalOcean-RCE.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/FrenzisRed/CVE-2026-23744](https://github.com/FrenzisRed/CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/FrenzisRed/CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/FrenzisRed/CVE-2026-23744.svg)
- [https://github.com/fckoo/mcpjaminspector-unauth-rce](https://github.com/fckoo/mcpjaminspector-unauth-rce) :  ![starts](https://img.shields.io/github/stars/fckoo/mcpjaminspector-unauth-rce.svg) ![forks](https://img.shields.io/github/forks/fckoo/mcpjaminspector-unauth-rce.svg)


## CVE-2026-23520
 Arcane provides modern docker management. Prior to 1.13.0, Arcane has a command injection in the updater service. Arcane’s updater service supported lifecycle labels com.getarcaneapp.arcane.lifecycle.pre-update and com.getarcaneapp.arcane.lifecycle.post-update that allowed defining a command to run before or after a container update. The label value is passed directly to /bin/sh -c without sanitization or validation. Because any authenticated user (not limited to administrators) can create projects through the API, an attacker can create a project that specifies one of these lifecycle labels with a malicious command. When an administrator later triggers a container update (either manually or via scheduled update checks), Arcane reads the lifecycle label and executes its value as a shell command inside the container. This vulnerability is fixed in 1.13.0.

- [https://github.com/cypher-21/CVE-2026-23520](https://github.com/cypher-21/CVE-2026-23520) :  ![starts](https://img.shields.io/github/stars/cypher-21/CVE-2026-23520.svg) ![forks](https://img.shields.io/github/forks/cypher-21/CVE-2026-23520.svg)


## CVE-2026-3888
 Local privilege escalation in snapd on Linux allows local attackers to get root privilege by re-creating snap's private /tmp directory when systemd-tmpfiles is configured to automatically clean up this directory. This issue affects Ubuntu 16.04 LTS, 18.04 LTS, 20.04 LTS, 22.04 LTS, and 24.04 LTS.

- [https://github.com/nomaisthere/CVE-2026-3888](https://github.com/nomaisthere/CVE-2026-3888) :  ![starts](https://img.shields.io/github/stars/nomaisthere/CVE-2026-3888.svg) ![forks](https://img.shields.io/github/forks/nomaisthere/CVE-2026-3888.svg)
- [https://github.com/TheCyberGeek/CVE-2026-3888-snap-confine-systemd-tmpfiles-LPE](https://github.com/TheCyberGeek/CVE-2026-3888-snap-confine-systemd-tmpfiles-LPE) :  ![starts](https://img.shields.io/github/stars/TheCyberGeek/CVE-2026-3888-snap-confine-systemd-tmpfiles-LPE.svg) ![forks](https://img.shields.io/github/forks/TheCyberGeek/CVE-2026-3888-snap-confine-systemd-tmpfiles-LPE.svg)


## CVE-2026-3587
 An unauthenticated remote attacker can exploit a hidden function in the CLI prompt to escape the restricted interface and gain root access to the underlying Linux based OS, leading to full compromise of the device.

- [https://github.com/z3r0h3ro/cve-2026-3587-poc](https://github.com/z3r0h3ro/cve-2026-3587-poc) :  ![starts](https://img.shields.io/github/stars/z3r0h3ro/cve-2026-3587-poc.svg) ![forks](https://img.shields.io/github/forks/z3r0h3ro/cve-2026-3587-poc.svg)


## CVE-2026-3288
 A security issue was discovered in ingress-nginx where the `nginx.ingress.kubernetes.io/rewrite-target` Ingress annotation can be used to inject configuration into nginx. This can lead to arbitrary code execution in the context of the ingress-nginx controller, and disclosure of Secrets accessible to the controller. (Note that in the default installation, the controller can access all Secrets cluster-wide.)

- [https://github.com/SnailSploit/CVE-2026-32885](https://github.com/SnailSploit/CVE-2026-32885) :  ![starts](https://img.shields.io/github/stars/SnailSploit/CVE-2026-32885.svg) ![forks](https://img.shields.io/github/forks/SnailSploit/CVE-2026-32885.svg)


## CVE-2026-3049
 A vulnerability was detected in horilla-opensource horilla up to 1.0.2. This issue affects the function get of the file horilla_generics/global_search.py of the component Query Parameter Handler. The manipulation of the argument prev_url results in open redirect. The attack can be executed remotely. The exploit is now public and may be used. Upgrading to version 1.0.3 is capable of addressing this issue. The patch is identified as 730b5a44ff060916780c44a4bdbc8ced70a2cd27. The affected component should be upgraded.

- [https://github.com/Mehdi-Ben-Hamou/CVE-2026-30498](https://github.com/Mehdi-Ben-Hamou/CVE-2026-30498) :  ![starts](https://img.shields.io/github/stars/Mehdi-Ben-Hamou/CVE-2026-30498.svg) ![forks](https://img.shields.io/github/forks/Mehdi-Ben-Hamou/CVE-2026-30498.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)


## CVE-2025-66398
 Signal K Server is a server application that runs on a central hub in a boat. Prior to version 2.19.0, an unauthenticated attacker can pollute the internal state (`restoreFilePath`) of the server via the `/skServer/validateBackup` endpoint. This allows the attacker to hijack the administrator's "Restore" functionality to overwrite critical server configuration files (e.g., `security.json`, `package.json`), leading to account takeover and Remote Code Execution (RCE). Version 2.19.0 patches this vulnerability.

- [https://github.com/showy-headteacher114/cve-2025-66398](https://github.com/showy-headteacher114/cve-2025-66398) :  ![starts](https://img.shields.io/github/stars/showy-headteacher114/cve-2025-66398.svg) ![forks](https://img.shields.io/github/forks/showy-headteacher114/cve-2025-66398.svg)


## CVE-2025-53770
Microsoft is preparing and fully testing a comprehensive update to address this vulnerability.  In the meantime, please make sure that the mitigation provided in this CVE documentation is in place so that you are protected from exploitation.

- [https://github.com/gmh5225/ZeroPoint](https://github.com/gmh5225/ZeroPoint) :  ![starts](https://img.shields.io/github/stars/gmh5225/ZeroPoint.svg) ![forks](https://img.shields.io/github/forks/gmh5225/ZeroPoint.svg)


## CVE-2025-52204
 A Cross-Site Scripting (XSS) vulnerability exists in Znuny::ITSM 6.5.x in the customer.pl endpoint via the OTRSCustomerInterface parameter

- [https://github.com/j0qq3r/CVE-2025-52204](https://github.com/j0qq3r/CVE-2025-52204) :  ![starts](https://img.shields.io/github/stars/j0qq3r/CVE-2025-52204.svg) ![forks](https://img.shields.io/github/forks/j0qq3r/CVE-2025-52204.svg)


## CVE-2025-49132
 Pterodactyl is a free, open-source game server management panel. Prior to version 1.11.11, using the /locales/locale.json with the locale and namespace query parameters, a malicious actor is able to execute arbitrary code without being authenticated. With the ability to execute arbitrary code it could be used to gain access to the Panel's server, read credentials from the Panel's config, extract sensitive information from the database, access files of servers managed by the panel, etc. This issue has been patched in version 1.11.11. There are no software workarounds for this vulnerability, but use of an external Web Application Firewall (WAF) could help mitigate this attack.

- [https://github.com/nik123-py/CVE-2025-49132_HTB_SEASON10](https://github.com/nik123-py/CVE-2025-49132_HTB_SEASON10) :  ![starts](https://img.shields.io/github/stars/nik123-py/CVE-2025-49132_HTB_SEASON10.svg) ![forks](https://img.shields.io/github/forks/nik123-py/CVE-2025-49132_HTB_SEASON10.svg)


## CVE-2025-34096
 A stack-based buffer overflow vulnerability exists in Easy File Sharing HTTP Server version 7.2. The flaw is triggered when a crafted POST request is sent to the /sendemail.ghp endpoint containing an overly long Email parameter. The application fails to properly validate the length of this field, resulting in a memory corruption condition. An unauthenticated remote attacker can exploit this to execute arbitrary code with the privileges of the server process.

- [https://github.com/TheMalwareGuardian/CVE-2025-34096](https://github.com/TheMalwareGuardian/CVE-2025-34096) :  ![starts](https://img.shields.io/github/stars/TheMalwareGuardian/CVE-2025-34096.svg) ![forks](https://img.shields.io/github/forks/TheMalwareGuardian/CVE-2025-34096.svg)


## CVE-2025-25200
 Koa is expressive middleware for Node.js using ES2017 async functions. Prior to versions 0.21.2, 1.7.1, 2.15.4, and 3.0.0-alpha.3, Koa uses an evil regex to parse the `X-Forwarded-Proto` and `X-Forwarded-Host` HTTP headers. This can be exploited to carry out a Denial-of-Service attack. Versions 0.21.2, 1.7.1, 2.15.4, and 3.0.0-alpha.3 fix the issue.

- [https://github.com/dwictor0/PoC-CVE-2025-25200](https://github.com/dwictor0/PoC-CVE-2025-25200) :  ![starts](https://img.shields.io/github/stars/dwictor0/PoC-CVE-2025-25200.svg) ![forks](https://img.shields.io/github/forks/dwictor0/PoC-CVE-2025-25200.svg)


## CVE-2025-24893
 XWiki Platform is a generic wiki platform offering runtime services for applications built on top of it. Any guest can perform arbitrary remote code execution through a request to `SolrSearch`. This impacts the confidentiality, integrity and availability of the whole XWiki installation. To reproduce on an instance, without being logged in, go to `host/xwiki/bin/get/Main/SolrSearch?media=rss&text=%7D%7D%7D%7B%7Basync%20async%3Dfalse%7D%7D%7B%7Bgroovy%7D%7Dprintln%28"Hello%20from"%20%2B%20"%20search%20text%3A"%20%2B%20%2823%20%2B%2019%29%29%7B%7B%2Fgroovy%7D%7D%7B%7B%2Fasync%7D%7D%20`. If there is an output, and the title of the RSS feed contains `Hello from search text:42`, then the instance is vulnerable. This vulnerability has been patched in XWiki 15.10.11, 16.4.1 and 16.5.0RC1. Users are advised to upgrade. Users unable to upgrade may edit `Main.SolrSearchMacros` in `SolrSearchMacros.xml` on line 955 to match the `rawResponse` macro in `macros.vm#L2824` with a content type of `application/xml`, instead of simply outputting the content of the feed.

- [https://github.com/gmh5225/CVE-2025-24893-RCE-PoC](https://github.com/gmh5225/CVE-2025-24893-RCE-PoC) :  ![starts](https://img.shields.io/github/stars/gmh5225/CVE-2025-24893-RCE-PoC.svg) ![forks](https://img.shields.io/github/forks/gmh5225/CVE-2025-24893-RCE-PoC.svg)


## CVE-2025-12137
 The Import WP – Export and Import CSV and XML files to WordPress plugin for WordPress is vulnerable to Arbitrary File Read in all versions up to, and including, 2.14.16. This is due to the plugin's REST API endpoint accepting arbitrary absolute file paths without proper validation in the 'attach_file()' function when handling 'file_local' actions. This makes it possible for authenticated attackers, with administrator-level access and above, to read arbitrary files on the server's filesystem, including sensitive configuration files and system files via the 'local_url' parameter.

- [https://github.com/jFriedli/CVE-2025-12137](https://github.com/jFriedli/CVE-2025-12137) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-12137.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-12137.svg)


## CVE-2025-12028
 The IndieAuth plugin for WordPress is vulnerable to Cross-Site Request Forgery in all versions up to, and including, 4.5.4. This is due to missing nonce verification on the `login_form_indieauth()` function and the authorization endpoint at wp-login.php?action=indieauth. This makes it possible for unauthenticated attackers to force authenticated users to approve OAuth authorization requests for attacker-controlled applications via a forged request granted they can trick a user into performing an action such as clicking on a link or visiting a malicious page while logged in. The attacker can then exchange the stolen authorization code for an access token, effectively taking over the victim's account with the granted scopes (create, update, delete).

- [https://github.com/jFriedli/CVE-2025-12028](https://github.com/jFriedli/CVE-2025-12028) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-12028.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-12028.svg)


## CVE-2025-11988
 The Crypto plugin for WordPress is vulnerable to unauthorized manipulation of data in all versions up to, and including, 2.22. This is due to the plugin registering an unauthenticated AJAX action (wp_ajax_nopriv_crypto_connect_ajax_process) that allows calling the crypto_delete_json method with only a publicly-available nonce check. This makes it possible for unauthenticated attackers to delete specific JSON files matching the pattern *_pending.json within the wp-content/uploads/yak/ directory, causing data loss and denial of service for plugin workflows that rely on these artifacts.

- [https://github.com/jFriedli/CVE-2025-11988](https://github.com/jFriedli/CVE-2025-11988) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-11988.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-11988.svg)


## CVE-2025-11986
 The Crypto plugin for WordPress is vulnerable to Information exposure in all versions up to, and including, 2.22. This is due to the plugin registering an unauthenticated AJAX action (wp_ajax_nopriv_crypto_connect_ajax_process) that allows calling the register and savenft methods with only a publicly-available nonce check and no wallet signature verification. This makes it possible for unauthenticated attackers to set a site-wide global authentication state via a single transient, bypassing all access controls for ALL visitors to the site. The impact is complete bypass of [crypto-block] shortcode restrictions and page-level access controls, affecting all site visitors for one hour, plus the ability to inject arbitrary data into the plugin's custom_users table.

- [https://github.com/jFriedli/CVE-2025-11986](https://github.com/jFriedli/CVE-2025-11986) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-11986.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-11986.svg)


## CVE-2025-11973
 The 简数采集器 plugin for WordPress is vulnerable to Arbitrary File Read in all versions up to, and including, 2.6.3 via the __kds_flag functionality that imports featured images. This makes it possible for authenticated attackers, with Adminstrator-level access and above, to read the contents of arbitrary files on the server, which can contain sensitive information.

- [https://github.com/jFriedli/CVE-2025-11973](https://github.com/jFriedli/CVE-2025-11973) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-11973.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-11973.svg)


## CVE-2025-11771
 The Cryptocurrency (Token), Launchpad (Presale), ICO & IDO, Airdrop by TokenICO plugin for WordPress is vulnerable to unauthenticated and unauthorized modification of data due to missing authentication and capability checks on the 'createSaleRecord' function in all versions up to, and including, 2.4.6. This makes it possible for unauthenticated attackers to manipulate presales counters.

- [https://github.com/jFriedli/CVE-2025-11771](https://github.com/jFriedli/CVE-2025-11771) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-11771.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-11771.svg)


## CVE-2025-11627
 The Site Checkup Debug AI Troubleshooting with Wizard and Tips for Each Issue plugin for WordPress is vulnerable to log file poisoning in all versions up to, and including, 1.47. This makes it possible for unauthenticated attackers to insert arbitrary content into log files, and potentially cause denial of service via disk space exhaustion.

- [https://github.com/jFriedli/CVE-2025-11627](https://github.com/jFriedli/CVE-2025-11627) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-11627.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-11627.svg)


## CVE-2025-11177
 The External Login plugin for WordPress is vulnerable to SQL Injection via the 'log' parameter in all versions up to, and including, 1.11.2 due to insufficient escaping on the user supplied parameter and lack of sufficient preparation on the existing SQL query.  This makes it possible for unauthenticated attackers to append additional SQL queries into already existing queries that can be used to extract sensitive information from the database when a PostgreSQL or MSSQL database is configured as the external authentication database.

- [https://github.com/jFriedli/CVE-2025-11177](https://github.com/jFriedli/CVE-2025-11177) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-11177.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-11177.svg)


## CVE-2025-10658
 The SupportCandy – Helpdesk & Customer Support Ticket System plugin for WordPress is vulnerable to Authentication Bypass in all versions up to, and including, 3.3.7. This is due to missing rate limiting on the OTP verification for guest login. This makes it possible for unauthenticated attackers to bypass authentication and gain unauthorized access to customer support tickets by brute forcing the 6-digit OTP code.

- [https://github.com/jFriedli/CVE-2025-10658](https://github.com/jFriedli/CVE-2025-10658) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-10658.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-10658.svg)


## CVE-2025-10307
 The Backuply – Backup, Restore, Migrate and Clone plugin for WordPress is vulnerable to arbitrary file deletion due to insufficient file path validation in the delete backup functionality in all versions up to, and including, 1.4.8. This makes it possible for authenticated attackers, with Administrator-level access and above, to delete arbitrary files on the server, which can easily lead to remote code execution when the right file is deleted (such as wp-config.php).

- [https://github.com/jFriedli/CVE-2025-10307](https://github.com/jFriedli/CVE-2025-10307) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-10307.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-10307.svg)


## CVE-2025-10294
 The OwnID Passwordless Login plugin for WordPress is vulnerable to Authentication Bypass in all versions up to, and including, 1.3.4. This is due to the plugin not properly checking if the ownid_shared_secret value is empty prior to authenticating a user via JWT. This makes it possible for unauthenticated attackers to log in as other users, including administrators, on instances where the plugin has not been fully configured yet.

- [https://github.com/jFriedli/CVE-2025-10294](https://github.com/jFriedli/CVE-2025-10294) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-10294.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-10294.svg)


## CVE-2025-9967
 The Orion SMS OTP Verification plugin for WordPress is vulnerable to privilege escalation via account takeover in all versions up to, and including, 1.1.7. This is due to the plugin not properly validating a user's identity prior to updating their password. This makes it possible for unauthenticated attackers to change arbitrary user's password to a one-time password if the attacker knows the user's phone number

- [https://github.com/jFriedli/CVE-2025-9967](https://github.com/jFriedli/CVE-2025-9967) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-9967.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-9967.svg)


## CVE-2025-9485
 The OAuth Single Sign On – SSO (OAuth Client) plugin for WordPress is vulnerable to Improper Verification of Cryptographic Signature in versions up to, and including, 6.26.12. This is due to the plugin performing unsafe JWT token processing without verification or validation in the `get_resource_owner_from_id_token` function. This makes it possible for unauthenticated attackers to bypass authentication and gain access to any existing user account - including administrators in certain configurations - or to create arbitrary subscriber-level accounts.

- [https://github.com/jFriedli/CVE-2025-9485](https://github.com/jFriedli/CVE-2025-9485) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-9485.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-9485.svg)


## CVE-2025-9172
 The Vibes plugin for WordPress is vulnerable to time-based SQL Injection via the ‘resource’ parameter in all versions up to, and including, 2.2.0 due to insufficient escaping on the user supplied parameter and lack of sufficient preparation on the existing SQL query.  This makes it possible for unauthenticated attackers to append additional SQL queries into already existing queries that can be used to extract sensitive information from the database.

- [https://github.com/jFriedli/CVE-2025-9172](https://github.com/jFriedli/CVE-2025-9172) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-9172.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-9172.svg)


## CVE-2025-9074
This can lead to execution of a wide range of privileged commands to the engine API, including controlling other containers, creating new ones, managing images etc. In some circumstances (e.g. Docker Desktop for Windows with WSL backend) it also allows mounting the host drive with the same privileges as the user running Docker Desktop.

- [https://github.com/rocket-panda/CVE-2025-9074](https://github.com/rocket-panda/CVE-2025-9074) :  ![starts](https://img.shields.io/github/stars/rocket-panda/CVE-2025-9074.svg) ![forks](https://img.shields.io/github/forks/rocket-panda/CVE-2025-9074.svg)


## CVE-2025-6792
 The One to one user Chat by WPGuppy plugin for WordPress is vulnerable to unauthorized access of data due to a missing capability check on the /wp-json/guppylite/v2/channel-authorize rest endpoint in all versions up to, and including, 1.1.4. This makes it possible for unauthenticated attackers to intercept and view private chat messages between users.

- [https://github.com/jFriedli/CVE-2025-6792](https://github.com/jFriedli/CVE-2025-6792) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-6792.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-6792.svg)


## CVE-2025-6783
 The GoZen Forms plugin for WordPress is vulnerable to SQL Injection via the 'forms-id' parameter of the emdedSc() function in all versions up to, and including, 1.1.5 due to insufficient escaping on the user supplied parameter and lack of sufficient preparation on the existing SQL query.  This makes it possible for unauthenticated attackers to append additional SQL queries into already existing queries that can be used to extract sensitive information from the database.

- [https://github.com/jFriedli/CVE-2025-6783](https://github.com/jFriedli/CVE-2025-6783) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-6783.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-6783.svg)


## CVE-2025-6782
 The GoZen Forms plugin for WordPress is vulnerable to SQL Injection via the 'forms-id' parameter of the dirGZActiveForm() function in all versions up to, and including, 1.1.5 due to insufficient escaping on the user supplied parameter and lack of sufficient preparation on the existing SQL query.  This makes it possible for unauthenticated attackers to append additional SQL queries into already existing queries that can be used to extract sensitive information from the database.

- [https://github.com/jFriedli/CVE-2025-6782](https://github.com/jFriedli/CVE-2025-6782) :  ![starts](https://img.shields.io/github/stars/jFriedli/CVE-2025-6782.svg) ![forks](https://img.shields.io/github/forks/jFriedli/CVE-2025-6782.svg)


## CVE-2025-6002
 An unrestricted file upload vulnerability exists in the Product Image section of the VirtueMart backend. Authenticated attackers can upload files with arbitrary extensions, including executable or malicious files, potentially leading to remote code execution or other security impacts depending on server configuration.

- [https://github.com/schn1tzelme1ster/CVE-2025-6002](https://github.com/schn1tzelme1ster/CVE-2025-6002) :  ![starts](https://img.shields.io/github/stars/schn1tzelme1ster/CVE-2025-6002.svg) ![forks](https://img.shields.io/github/forks/schn1tzelme1ster/CVE-2025-6002.svg)


## CVE-2024-46879
 A Reflected Cross-Site Scripting (XSS) vulnerability exists in the POST request data zipPath of tiki-admin_system.php in Tiki version 21.2. This vulnerability allows attackers to execute arbitrary JavaScript code via a crafted payload, leading to potential access to sensitive information or unauthorized actions.

- [https://github.com/ColdFusionX/CVE-2024-46879-TikiCMS-XSS](https://github.com/ColdFusionX/CVE-2024-46879-TikiCMS-XSS) :  ![starts](https://img.shields.io/github/stars/ColdFusionX/CVE-2024-46879-TikiCMS-XSS.svg) ![forks](https://img.shields.io/github/forks/ColdFusionX/CVE-2024-46879-TikiCMS-XSS.svg)


## CVE-2024-46878
 A Cross-Site Scripting (XSS) vulnerability exists in the page parameter of tiki-editpage.php in Tiki version 26.3 and earlier. This vulnerability allows attackers to execute arbitrary JavaScript code via a crafted payload, leading to potential access to sensitive information or unauthorized actions.

- [https://github.com/ColdFusionX/CVE-2024-46878-TikiCMS-XSS](https://github.com/ColdFusionX/CVE-2024-46878-TikiCMS-XSS) :  ![starts](https://img.shields.io/github/stars/ColdFusionX/CVE-2024-46878-TikiCMS-XSS.svg) ![forks](https://img.shields.io/github/forks/ColdFusionX/CVE-2024-46878-TikiCMS-XSS.svg)


## CVE-2024-5134
 A vulnerability was found in SourceCodester Electricity Consumption Monitoring Tool 1.0. It has been declared as critical. This vulnerability affects unknown code of the file /endpoint/delete-bill.php. The manipulation of the argument bill leads to sql injection. The attack can be initiated remotely. The exploit has been disclosed to the public and may be used. VDB-265210 is the identifier assigned to this vulnerability.

- [https://github.com/victorGoeman/CVE-2024-51347](https://github.com/victorGoeman/CVE-2024-51347) :  ![starts](https://img.shields.io/github/stars/victorGoeman/CVE-2024-51347.svg) ![forks](https://img.shields.io/github/forks/victorGoeman/CVE-2024-51347.svg)
- [https://github.com/victorGoeman/CVE-2024-51348](https://github.com/victorGoeman/CVE-2024-51348) :  ![starts](https://img.shields.io/github/stars/victorGoeman/CVE-2024-51348.svg) ![forks](https://img.shields.io/github/forks/victorGoeman/CVE-2024-51348.svg)
- [https://github.com/victorGoeman/CVE-2024-51346](https://github.com/victorGoeman/CVE-2024-51346) :  ![starts](https://img.shields.io/github/stars/victorGoeman/CVE-2024-51346.svg) ![forks](https://img.shields.io/github/forks/victorGoeman/CVE-2024-51346.svg)


## CVE-2024-2473
 The WPS Hide Login plugin for WordPress is vulnerable to Login Page Disclosure in all versions up to, and including, 1.9.15.2. This is due to a bypass that is created when the 'action=postpass' parameter is supplied. This makes it possible for attackers to easily discover any login page that may have been hidden by the plugin.

- [https://github.com/M4xSec/CVE-2024-2473](https://github.com/M4xSec/CVE-2024-2473) :  ![starts](https://img.shields.io/github/stars/M4xSec/CVE-2024-2473.svg) ![forks](https://img.shields.io/github/forks/M4xSec/CVE-2024-2473.svg)


## CVE-2023-32784
 In KeePass 2.x before 2.54, it is possible to recover the cleartext master password from a memory dump, even when a workspace is locked or no longer running. The memory dump can be a KeePass process dump, swap file (pagefile.sys), hibernation file (hiberfil.sys), or RAM dump of the entire system. The first character cannot be recovered. In 2.54, there is different API usage and/or random string insertion for mitigation.

- [https://github.com/super-oof/keepass2-password-finder](https://github.com/super-oof/keepass2-password-finder) :  ![starts](https://img.shields.io/github/stars/super-oof/keepass2-password-finder.svg) ![forks](https://img.shields.io/github/forks/super-oof/keepass2-password-finder.svg)


## CVE-2022-36804
 Multiple API endpoints in Atlassian Bitbucket Server and Data Center 7.0.0 before version 7.6.17, from version 7.7.0 before version 7.17.10, from version 7.18.0 before version 7.21.4, from version 8.0.0 before version 8.0.3, from version 8.1.0 before version 8.1.3, and from version 8.2.0 before version 8.2.2, and from version 8.3.0 before 8.3.1 allows remote attackers with read permissions to a public or private Bitbucket repository to execute arbitrary code by sending a malicious HTTP request. This vulnerability was reported via our Bug Bounty Program by TheGrandPew.

- [https://github.com/JohanGabrielson/bitbucket-test](https://github.com/JohanGabrielson/bitbucket-test) :  ![starts](https://img.shields.io/github/stars/JohanGabrielson/bitbucket-test.svg) ![forks](https://img.shields.io/github/forks/JohanGabrielson/bitbucket-test.svg)


## CVE-2021-33044
 The identity authentication bypass vulnerability found in some Dahua products during the login process. Attackers can bypass device identity authentication by constructing malicious data packets.

- [https://github.com/eagle-nett/DAHUA_AUTH-BYPASS-CVE-2021-33044](https://github.com/eagle-nett/DAHUA_AUTH-BYPASS-CVE-2021-33044) :  ![starts](https://img.shields.io/github/stars/eagle-nett/DAHUA_AUTH-BYPASS-CVE-2021-33044.svg) ![forks](https://img.shields.io/github/forks/eagle-nett/DAHUA_AUTH-BYPASS-CVE-2021-33044.svg)


## CVE-2017-14980
 Buffer overflow in Sync Breeze Enterprise 10.0.28 allows remote attackers to have unspecified impact via a long username parameter to /login.

- [https://github.com/TheMalwareGuardian/CVE-2017-14980](https://github.com/TheMalwareGuardian/CVE-2017-14980) :  ![starts](https://img.shields.io/github/stars/TheMalwareGuardian/CVE-2017-14980.svg) ![forks](https://img.shields.io/github/forks/TheMalwareGuardian/CVE-2017-14980.svg)


## CVE-2015-8522
 Buffer overflow in the server in IBM Tivoli Storage Manager FastBack 5.5.x and 6.x before 6.1.12.2 allows remote attackers to execute arbitrary code via a crafted command, a different vulnerability than CVE-2015-8519, CVE-2015-8520, and CVE-2015-8521.

- [https://github.com/damariion/CVE-2015-8522](https://github.com/damariion/CVE-2015-8522) :  ![starts](https://img.shields.io/github/stars/damariion/CVE-2015-8522.svg) ![forks](https://img.shields.io/github/forks/damariion/CVE-2015-8522.svg)


## CVE-2014-0160
 The (1) TLS and (2) DTLS implementations in OpenSSL 1.0.1 before 1.0.1g do not properly handle Heartbeat Extension packets, which allows remote attackers to obtain sensitive information from process memory via crafted packets that trigger a buffer over-read, as demonstrated by reading private keys, related to d1_both.c and t1_lib.c, aka the Heartbleed bug.

- [https://github.com/Ryo-Soikutsu/Heartbleed](https://github.com/Ryo-Soikutsu/Heartbleed) :  ![starts](https://img.shields.io/github/stars/Ryo-Soikutsu/Heartbleed.svg) ![forks](https://img.shields.io/github/forks/Ryo-Soikutsu/Heartbleed.svg)


## CVE-2012-5958
 Stack-based buffer overflow in the unique_service_name function in ssdp/ssdp_server.c in the SSDP parser in the portable SDK for UPnP Devices (aka libupnp, formerly the Intel SDK for UPnP devices) before 1.6.18 allows remote attackers to execute arbitrary code via a UDP packet with a crafted string that is not properly handled after a certain pointer subtraction.

- [https://github.com/hmrumman777-beep/NetAudit-IoT](https://github.com/hmrumman777-beep/NetAudit-IoT) :  ![starts](https://img.shields.io/github/stars/hmrumman777-beep/NetAudit-IoT.svg) ![forks](https://img.shields.io/github/forks/hmrumman777-beep/NetAudit-IoT.svg)

