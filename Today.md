# Update 2026-04-27
## CVE-2026-41651
3. Late flag read at execution time (lines 2273–2277): The scheduler's idle callback reads cached_transaction_flags at dispatch time, not at authorization time. If flags were overwritten between authorization and execution, the backend sees the attacker's flags.

- [https://github.com/dinosn/pack2theroot-lab](https://github.com/dinosn/pack2theroot-lab) :  ![starts](https://img.shields.io/github/stars/dinosn/pack2theroot-lab.svg) ![forks](https://img.shields.io/github/forks/dinosn/pack2theroot-lab.svg)


## CVE-2026-41177
 Squidex is an open source headless content management system and content management hub. Prior to version 7.23.0, the Squidex Restore API is vulnerable to Blind Server-Side Request Forgery (SSRF). The application fails to validate the URI scheme of the user-supplied `Url` parameter, allowing the use of the `file://` protocol. This allows an authenticated administrator to force the backend server to interact with the local filesystem, which can lead to Local File Interaction (LFI) and potential disclosure of sensitive system information through side-channel analysis of internal logs. Version 7.23.0 contains a fix.

- [https://github.com/TurkiOS/CVE-2026-41177-Squidex-CMS](https://github.com/TurkiOS/CVE-2026-41177-Squidex-CMS) :  ![starts](https://img.shields.io/github/stars/TurkiOS/CVE-2026-41177-Squidex-CMS.svg) ![forks](https://img.shields.io/github/forks/TurkiOS/CVE-2026-41177-Squidex-CMS.svg)


## CVE-2026-39987
 marimo is a reactive Python notebook. Prior to 0.23.0, Marimo has a Pre-Auth RCE vulnerability. The terminal WebSocket endpoint /terminal/ws lacks authentication validation, allowing an unauthenticated attacker to obtain a full PTY shell and execute arbitrary system commands. Unlike other WebSocket endpoints (e.g., /ws) that correctly call validate_auth() for authentication, the /terminal/ws endpoint only checks the running mode and platform support before accepting connections, completely skipping authentication verification. This vulnerability is fixed in 0.23.0.

- [https://github.com/h3raklez/CVE-2026-39987](https://github.com/h3raklez/CVE-2026-39987) :  ![starts](https://img.shields.io/github/stars/h3raklez/CVE-2026-39987.svg) ![forks](https://img.shields.io/github/forks/h3raklez/CVE-2026-39987.svg)


## CVE-2026-22038
 AutoGPT is a platform that allows users to create, deploy, and manage continuous artificial intelligence agents that automate complex workflows. Prior to autogpt-platform-beta-v0.6.46, the AutoGPT platform's Stagehand integration blocks log API keys and authentication secrets in plaintext using logger.info() statements. This occurs in three separate block implementations (StagehandObserveBlock, StagehandActBlock, and StagehandExtractBlock) where the code explicitly calls api_key.get_secret_value() and logs the result. This issue has been patched in autogpt-platform-beta-v0.6.46.

- [https://github.com/sivaadityacoder/CVE-2026-22038](https://github.com/sivaadityacoder/CVE-2026-22038) :  ![starts](https://img.shields.io/github/stars/sivaadityacoder/CVE-2026-22038.svg) ![forks](https://img.shields.io/github/forks/sivaadityacoder/CVE-2026-22038.svg)


## CVE-2026-6356
 A vulnerability in the web application allows standard users to escalate their privileges to those of a super administrator through parameter manipulation, enabling them to access and modify sensitive information.

- [https://github.com/Penguinsecq/CVE-2026-6355](https://github.com/Penguinsecq/CVE-2026-6355) :  ![starts](https://img.shields.io/github/stars/Penguinsecq/CVE-2026-6355.svg) ![forks](https://img.shields.io/github/forks/Penguinsecq/CVE-2026-6355.svg)


## CVE-2026-3844
 The Breeze Cache plugin for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the 'fetch_gravatar_from_remote' function in all versions up to, and including, 2.4.4. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible. The vulnerability can only be exploited if "Host Files Locally - Gravatars" is enabled, which is disabled by default.

- [https://github.com/dinosn/CVE-2026-3844](https://github.com/dinosn/CVE-2026-3844) :  ![starts](https://img.shields.io/github/stars/dinosn/CVE-2026-3844.svg) ![forks](https://img.shields.io/github/forks/dinosn/CVE-2026-3844.svg)


## CVE-2026-3269
 A flaw has been found in psi-probe PSI Probe up to 5.3.0. The impacted element is the function handleRequestInternal of the file psi-probe-core/src/main/java/psiprobe/controllers/sessions/ExpireSessionsController.java of the component Session Handler. Executing a manipulation can lead to denial of service. The attack can be launched remotely. The exploit has been published and may be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/TurkiOS/cve-2026-32699-facturascripts-nick-bypass](https://github.com/TurkiOS/cve-2026-32699-facturascripts-nick-bypass) :  ![starts](https://img.shields.io/github/stars/TurkiOS/cve-2026-32699-facturascripts-nick-bypass.svg) ![forks](https://img.shields.io/github/forks/TurkiOS/cve-2026-32699-facturascripts-nick-bypass.svg)


## CVE-2026-2184
 A vulnerability was detected in Great Developers Certificate Generation System up to 97171bb0e5e22e52eacf4e4fa81773e5f3cffb73. This vulnerability affects unknown code of the file /restructured/csv.php. The manipulation of the argument photo results in os command injection. The attack can be executed remotely. This product implements a rolling release for ongoing delivery, which means version information for affected or updated releases is unavailable. The code repository of the project has not been active for many years.

- [https://github.com/blaxkmiradev/CVE-2026-21847-Hardcoded-AES-Encryption-Key-in-DPDC-Customer-Portal](https://github.com/blaxkmiradev/CVE-2026-21847-Hardcoded-AES-Encryption-Key-in-DPDC-Customer-Portal) :  ![starts](https://img.shields.io/github/stars/blaxkmiradev/CVE-2026-21847-Hardcoded-AES-Encryption-Key-in-DPDC-Customer-Portal.svg) ![forks](https://img.shields.io/github/forks/blaxkmiradev/CVE-2026-21847-Hardcoded-AES-Encryption-Key-in-DPDC-Customer-Portal.svg)


## CVE-2026-1729
 The AdForest theme for WordPress is vulnerable to authentication bypass in all versions up to, and including, 6.0.12. This is due to the plugin not properly verifying a user's identity prior to authenticating them through the 'sb_login_user_with_otp_fun' function. This makes it possible for unauthenticated attackers to log in as arbitrary users, including administrators.

- [https://github.com/ninjazan420/CVE-2026-1729-PoC-AdForest-WordPress-Authentication-Bypass](https://github.com/ninjazan420/CVE-2026-1729-PoC-AdForest-WordPress-Authentication-Bypass) :  ![starts](https://img.shields.io/github/stars/ninjazan420/CVE-2026-1729-PoC-AdForest-WordPress-Authentication-Bypass.svg) ![forks](https://img.shields.io/github/forks/ninjazan420/CVE-2026-1729-PoC-AdForest-WordPress-Authentication-Bypass.svg)


## CVE-2026-1529
 A flaw was found in Keycloak. An attacker can exploit this vulnerability by modifying the organization ID and target email within a legitimate invitation token's JSON Web Token (JWT) payload. This lack of cryptographic signature verification allows the attacker to successfully self-register into an unauthorized organization, leading to unauthorized access.

- [https://github.com/ninjazan420/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation](https://github.com/ninjazan420/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation) :  ![starts](https://img.shields.io/github/stars/ninjazan420/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation.svg) ![forks](https://img.shields.io/github/forks/ninjazan420/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation.svg)


## CVE-2026-0740
 The Ninja Forms - File Uploads plugin for WordPress is vulnerable to arbitrary file uploads due to missing file type validation in the 'NF_FU_AJAX_Controllers_Uploads::handle_upload' function in all versions up to, and including, 3.3.26. This makes it possible for unauthenticated attackers to upload arbitrary files on the affected site's server which may make remote code execution possible. Note: The vulnerability was partially patched in version 3.3.25 and fully patched in version 3.3.27.

- [https://github.com/murrez/CVE-2026-0740](https://github.com/murrez/CVE-2026-0740) :  ![starts](https://img.shields.io/github/stars/murrez/CVE-2026-0740.svg) ![forks](https://img.shields.io/github/forks/murrez/CVE-2026-0740.svg)


## CVE-2025-68621
 Trilium Notes is an open-source, cross-platform hierarchical note taking application with focus on building large personal knowledge bases.  Prior to 0.101.0, a critical timing attack vulnerability in Trilium's sync authentication endpoint allows unauthenticated remote attackers to recover HMAC authentication hashes byte-by-byte through statistical timing analysis. This enables complete authentication bypass without password knowledge, granting full read/write access to victim's knowledge base. This vulnerability is fixed in 0.101.0.

- [https://github.com/sivaadityacoder/CVE-2025-68621](https://github.com/sivaadityacoder/CVE-2025-68621) :  ![starts](https://img.shields.io/github/stars/sivaadityacoder/CVE-2025-68621.svg) ![forks](https://img.shields.io/github/forks/sivaadityacoder/CVE-2025-68621.svg)


## CVE-2025-67147
 Multiple SQL Injection vulnerabilities exist in amansuryawanshi Gym-Management-System-PHP 1.0 via the 'name', 'email', and 'comment' parameters in (1) submit_contact.php, the 'username' and 'pass_key' parameters in (2) secure_login.php, and the 'login_id', 'pwfield', and 'login_key' parameters in (3) change_s_pwd.php. An unauthenticated or authenticated attacker can exploit these issues to bypass authentication, execute arbitrary SQL commands, modify database records, delete data, or escalate privileges to administrator level.

- [https://github.com/sivaadityacoder/CVE-2025-67146-CVE-2025-67147](https://github.com/sivaadityacoder/CVE-2025-67146-CVE-2025-67147) :  ![starts](https://img.shields.io/github/stars/sivaadityacoder/CVE-2025-67146-CVE-2025-67147.svg) ![forks](https://img.shields.io/github/forks/sivaadityacoder/CVE-2025-67146-CVE-2025-67147.svg)


## CVE-2025-67146
 Multiple SQL Injection vulnerabilities exist in AbhishekMali21 GYM-MANAGEMENT-SYSTEM 1.0 via the 'name' parameter in (1) member_search.php, (2) trainer_search.php, and (3) gym_search.php, and via the 'id' parameter in (4) payment_search.php. An unauthenticated remote attacker can exploit these issues to inject malicious SQL commands, leading to unauthorized data extraction, authentication bypass, or modification of database contents.

- [https://github.com/sivaadityacoder/CVE-2025-67146-CVE-2025-67147](https://github.com/sivaadityacoder/CVE-2025-67146-CVE-2025-67147) :  ![starts](https://img.shields.io/github/stars/sivaadityacoder/CVE-2025-67146-CVE-2025-67147.svg) ![forks](https://img.shields.io/github/forks/sivaadityacoder/CVE-2025-67146-CVE-2025-67147.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)


## CVE-2025-54313
 eslint-config-prettier 8.10.1, 9.1.1, 10.1.6, and 10.1.7 has embedded malicious code for a supply chain compromise. Installing an affected package executes an install.js file that launches the node-gyp.dll malware on Windows.

- [https://github.com/Paspke/scavenger_scanner](https://github.com/Paspke/scavenger_scanner) :  ![starts](https://img.shields.io/github/stars/Paspke/scavenger_scanner.svg) ![forks](https://img.shields.io/github/forks/Paspke/scavenger_scanner.svg)


## CVE-2025-53770
Microsoft is preparing and fully testing a comprehensive update to address this vulnerability.  In the meantime, please make sure that the mitigation provided in this CVE documentation is in place so that you are protected from exploitation.

- [https://github.com/0xisfet/CVE-2025-53770-Scanner](https://github.com/0xisfet/CVE-2025-53770-Scanner) :  ![starts](https://img.shields.io/github/stars/0xisfet/CVE-2025-53770-Scanner.svg) ![forks](https://img.shields.io/github/forks/0xisfet/CVE-2025-53770-Scanner.svg)


## CVE-2025-52691
 Successful exploitation of the vulnerability could allow an unauthenticated attacker to upload arbitrary files to any location on the mail server, potentially enabling remote code execution.

- [https://github.com/ninjazan420/CVE-2025-52691-PoC-SmarterMail-authentication-bypass-exploit-WT-2026-0001](https://github.com/ninjazan420/CVE-2025-52691-PoC-SmarterMail-authentication-bypass-exploit-WT-2026-0001) :  ![starts](https://img.shields.io/github/stars/ninjazan420/CVE-2025-52691-PoC-SmarterMail-authentication-bypass-exploit-WT-2026-0001.svg) ![forks](https://img.shields.io/github/forks/ninjazan420/CVE-2025-52691-PoC-SmarterMail-authentication-bypass-exploit-WT-2026-0001.svg)


## CVE-2025-27407
 graphql-ruby is a Ruby implementation of GraphQL. Starting in version 1.11.5 and prior to versions 1.11.8, 1.12.25, 1.13.24, 2.0.32, 2.1.14, 2.2.17, and 2.3.21, loading a malicious schema definition in `GraphQL::Schema.from_introspection` (or `GraphQL::Schema::Loader.load`) can result in remote code execution. Any system which loads a schema by JSON from an untrusted source is vulnerable, including those that use GraphQL::Client to load external schemas via GraphQL introspection. Versions 1.11.8, 1.12.25, 1.13.24, 2.0.32, 2.1.14, 2.2.17, and 2.3.21 contain a patch for the issue.

- [https://github.com/LoGGGG2402/CVE-2025-27407](https://github.com/LoGGGG2402/CVE-2025-27407) :  ![starts](https://img.shields.io/github/stars/LoGGGG2402/CVE-2025-27407.svg) ![forks](https://img.shields.io/github/forks/LoGGGG2402/CVE-2025-27407.svg)


## CVE-2025-25279
 Mattermost versions 10.4.x = 10.4.1, 9.11.x = 9.11.7, 10.3.x = 10.3.2, 10.2.x = 10.2.2 fail to properly validate board blocks when importing boards which allows an attacker could read any arbitrary file on the system via importing and exporting a specially crafted import archive in Boards.

- [https://github.com/AbokorMAHAMMADMOUSSE/CVE-2025-25279-Mattermost-Path-Traversal](https://github.com/AbokorMAHAMMADMOUSSE/CVE-2025-25279-Mattermost-Path-Traversal) :  ![starts](https://img.shields.io/github/stars/AbokorMAHAMMADMOUSSE/CVE-2025-25279-Mattermost-Path-Traversal.svg) ![forks](https://img.shields.io/github/forks/AbokorMAHAMMADMOUSSE/CVE-2025-25279-Mattermost-Path-Traversal.svg)


## CVE-2025-2304
When a user wishes to change his password, the 'updated_ajax' method of the UsersController is called. The vulnerability stems from the use of the dangerous permit! method, which allows all parameters to pass through without any filtering.

- [https://github.com/Jeanback1/CVE-2025-2304-exploit](https://github.com/Jeanback1/CVE-2025-2304-exploit) :  ![starts](https://img.shields.io/github/stars/Jeanback1/CVE-2025-2304-exploit.svg) ![forks](https://img.shields.io/github/forks/Jeanback1/CVE-2025-2304-exploit.svg)


## CVE-2024-21413
 Microsoft Outlook Remote Code Execution Vulnerability

- [https://github.com/bhatbhupendra/Moniker-Link--CVE-2024-21413-](https://github.com/bhatbhupendra/Moniker-Link--CVE-2024-21413-) :  ![starts](https://img.shields.io/github/stars/bhatbhupendra/Moniker-Link--CVE-2024-21413-.svg) ![forks](https://img.shields.io/github/forks/bhatbhupendra/Moniker-Link--CVE-2024-21413-.svg)


## CVE-2024-3273
 ** UNSUPPORTED WHEN ASSIGNED ** A vulnerability, which was classified as critical, was found in D-Link DNS-320L, DNS-325, DNS-327L and DNS-340L up to 20240403. Affected is an unknown function of the file /cgi-bin/nas_sharing.cgi of the component HTTP GET Request Handler. The manipulation of the argument system leads to command injection. It is possible to launch the attack remotely. The exploit has been disclosed to the public and may be used. The identifier of this vulnerability is VDB-259284. NOTE: This vulnerability only affects products that are no longer supported by the maintainer. NOTE: Vendor was contacted early and confirmed immediately that the product is end-of-life. It should be retired and replaced.

- [https://github.com/askhatov21/CP3418_BestPracticesCybersecurity_OTANATA_Project](https://github.com/askhatov21/CP3418_BestPracticesCybersecurity_OTANATA_Project) :  ![starts](https://img.shields.io/github/stars/askhatov21/CP3418_BestPracticesCybersecurity_OTANATA_Project.svg) ![forks](https://img.shields.io/github/forks/askhatov21/CP3418_BestPracticesCybersecurity_OTANATA_Project.svg)


## CVE-2023-32629
 Local privilege escalation vulnerability in Ubuntu Kernels overlayfs ovl_copy_up_meta_inode_data skip permission checks when calling ovl_do_setxattr on Ubuntu kernels

- [https://github.com/h3raklez/CVE-2023-32629](https://github.com/h3raklez/CVE-2023-32629) :  ![starts](https://img.shields.io/github/stars/h3raklez/CVE-2023-32629.svg) ![forks](https://img.shields.io/github/forks/h3raklez/CVE-2023-32629.svg)


## CVE-2019-9053
 An issue was discovered in CMS Made Simple 2.2.8. It is possible with the News module, through a crafted URL, to achieve unauthenticated blind time-based SQL injection via the m1_idlist parameter.

- [https://github.com/killukeren/-CVE-2019-9053](https://github.com/killukeren/-CVE-2019-9053) :  ![starts](https://img.shields.io/github/stars/killukeren/-CVE-2019-9053.svg) ![forks](https://img.shields.io/github/forks/killukeren/-CVE-2019-9053.svg)


## CVE-2018-14009
 Codiad through 2.8.4 allows Remote Code Execution, a different vulnerability than CVE-2017-11366 and CVE-2017-15689.

- [https://github.com/lolameroo/Codiad-CVE-2018-14009](https://github.com/lolameroo/Codiad-CVE-2018-14009) :  ![starts](https://img.shields.io/github/stars/lolameroo/Codiad-CVE-2018-14009.svg) ![forks](https://img.shields.io/github/forks/lolameroo/Codiad-CVE-2018-14009.svg)


## CVE-2017-11882
 Microsoft Office 2007 Service Pack 3, Microsoft Office 2010 Service Pack 2, Microsoft Office 2013 Service Pack 1, and Microsoft Office 2016 allow an attacker to run arbitrary code in the context of the current user by failing to properly handle objects in memory, aka "Microsoft Office Memory Corruption Vulnerability". This CVE ID is unique from CVE-2017-11884.

- [https://github.com/DONKEY0xSHOT/CVE-2017-11882-Blocker](https://github.com/DONKEY0xSHOT/CVE-2017-11882-Blocker) :  ![starts](https://img.shields.io/github/stars/DONKEY0xSHOT/CVE-2017-11882-Blocker.svg) ![forks](https://img.shields.io/github/forks/DONKEY0xSHOT/CVE-2017-11882-Blocker.svg)


## CVE-2017-11366
 components/filemanager/class.filemanager.php in Codiad before 2.8.4 is vulnerable to remote command execution because shell commands can be embedded in parameter values, as demonstrated by search_file_type.

- [https://github.com/lolameroo/Codiad-CVE-2018-14009](https://github.com/lolameroo/Codiad-CVE-2018-14009) :  ![starts](https://img.shields.io/github/stars/lolameroo/Codiad-CVE-2018-14009.svg) ![forks](https://img.shields.io/github/forks/lolameroo/Codiad-CVE-2018-14009.svg)


## CVE-2002-1120
 Buffer overflow in Savant Web Server 3.1 and earlier allows remote attackers to execute arbitrary code via a long HTTP GET request.

- [https://github.com/TheMalwareGuardian/CVE-2002-1120](https://github.com/TheMalwareGuardian/CVE-2002-1120) :  ![starts](https://img.shields.io/github/stars/TheMalwareGuardian/CVE-2002-1120.svg) ![forks](https://img.shields.io/github/forks/TheMalwareGuardian/CVE-2002-1120.svg)


## CVE-2002-0936
 The Java Server Pages (JSP) engine in Tomcat allows web page owners to cause a denial of service (engine crash) on the web server via a JSP page that calls WPrinterJob().pageSetup(null,null).

- [https://github.com/om4rsallam/Full-Attack-Lifecycle-Simulation-on-Metasploitable](https://github.com/om4rsallam/Full-Attack-Lifecycle-Simulation-on-Metasploitable) :  ![starts](https://img.shields.io/github/stars/om4rsallam/Full-Attack-Lifecycle-Simulation-on-Metasploitable.svg) ![forks](https://img.shields.io/github/forks/om4rsallam/Full-Attack-Lifecycle-Simulation-on-Metasploitable.svg)


## CVE-2002-0082
 The dbm and shm session cache code in mod_ssl before 2.8.7-1.3.23, and Apache-SSL before 1.3.22+1.46, does not properly initialize memory using the i2d_SSL_SESSION function, which allows remote attackers to use a buffer overflow to execute arbitrary code via a large client certificate that is signed by a trusted Certificate Authority (CA), which produces a large serialized session.

- [https://github.com/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation](https://github.com/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation) :  ![starts](https://img.shields.io/github/stars/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation.svg) ![forks](https://img.shields.io/github/forks/anilkashyap01/Binary-Exploitation-and-Kernel-Escalation.svg)

