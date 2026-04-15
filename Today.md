# Update 2026-04-15
## CVE-2026-40175
 Axios is a promise based HTTP client for the browser and Node.js. Prior to 1.15.0, the Axios library is vulnerable to a specific "Gadget" attack chain that allows Prototype Pollution in any third-party dependency to be escalated into Remote Code Execution (RCE) or Full Cloud Compromise (via AWS IMDSv2 bypass). This vulnerability is fixed in 1.15.0.

- [https://github.com/kengzzzz/CVE-2026-40175](https://github.com/kengzzzz/CVE-2026-40175) :  ![starts](https://img.shields.io/github/stars/kengzzzz/CVE-2026-40175.svg) ![forks](https://img.shields.io/github/forks/kengzzzz/CVE-2026-40175.svg)


## CVE-2026-39987
 marimo is a reactive Python notebook. Prior to 0.23.0, Marimo has a Pre-Auth RCE vulnerability. The terminal WebSocket endpoint /terminal/ws lacks authentication validation, allowing an unauthenticated attacker to obtain a full PTY shell and execute arbitrary system commands. Unlike other WebSocket endpoints (e.g., /ws) that correctly call validate_auth() for authentication, the /terminal/ws endpoint only checks the running mode and platform support before accepting connections, completely skipping authentication verification. This vulnerability is fixed in 0.23.0.

- [https://github.com/mki9/CVE-2026-39987_exploit](https://github.com/mki9/CVE-2026-39987_exploit) :  ![starts](https://img.shields.io/github/stars/mki9/CVE-2026-39987_exploit.svg) ![forks](https://img.shields.io/github/forks/mki9/CVE-2026-39987_exploit.svg)
- [https://github.com/fevar54/marimo_CVE-2026-39987_RCE_PoC](https://github.com/fevar54/marimo_CVE-2026-39987_RCE_PoC) :  ![starts](https://img.shields.io/github/stars/fevar54/marimo_CVE-2026-39987_RCE_PoC.svg) ![forks](https://img.shields.io/github/forks/fevar54/marimo_CVE-2026-39987_RCE_PoC.svg)


## CVE-2026-35616
 A improper access control vulnerability in Fortinet FortiClientEMS 7.4.5 through 7.4.6 may allow an unauthenticated attacker to execute unauthorized code or commands via crafted requests.

- [https://github.com/keraattin/CVE-2026-35616](https://github.com/keraattin/CVE-2026-35616) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-35616.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-35616.svg)


## CVE-2026-34621
 Acrobat Reader versions 24.001.30356, 26.001.21367 and earlier are affected by an Improperly Controlled Modification of Object Prototype Attributes ('Prototype Pollution') vulnerability that could result in arbitrary code execution in the context of the current user. Exploitation of this issue requires user interaction in that a victim must open a malicious file.

- [https://github.com/eduardorossi84/CVE-2026-34621-POC](https://github.com/eduardorossi84/CVE-2026-34621-POC) :  ![starts](https://img.shields.io/github/stars/eduardorossi84/CVE-2026-34621-POC.svg) ![forks](https://img.shields.io/github/forks/eduardorossi84/CVE-2026-34621-POC.svg)
- [https://github.com/ercihan/CVE-2026-34621](https://github.com/ercihan/CVE-2026-34621) :  ![starts](https://img.shields.io/github/stars/ercihan/CVE-2026-34621.svg) ![forks](https://img.shields.io/github/forks/ercihan/CVE-2026-34621.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/Spydomain/CVE-2026-33017-lab](https://github.com/Spydomain/CVE-2026-33017-lab) :  ![starts](https://img.shields.io/github/stars/Spydomain/CVE-2026-33017-lab.svg) ![forks](https://img.shields.io/github/forks/Spydomain/CVE-2026-33017-lab.svg)


## CVE-2026-31283
 In Totara LMS v19.1.5 and before, the forgot password API does not implement rate limiting for the target email address. which can be used for an Email Bombing attack.

- [https://github.com/saykino/CVE-2026-31283](https://github.com/saykino/CVE-2026-31283) :  ![starts](https://img.shields.io/github/stars/saykino/CVE-2026-31283.svg) ![forks](https://img.shields.io/github/forks/saykino/CVE-2026-31283.svg)


## CVE-2026-31282
 Totara LMS v19.1.5 and before is vulnerable to Incorrect Access Control. The login page code can be manipulated to reveal the login form. An attacker can chain that with missing rate-limit on the login form to launch a brute force attack.

- [https://github.com/saykino/CVE-2026-31282](https://github.com/saykino/CVE-2026-31282) :  ![starts](https://img.shields.io/github/stars/saykino/CVE-2026-31282.svg) ![forks](https://img.shields.io/github/forks/saykino/CVE-2026-31282.svg)


## CVE-2026-31281
 Totara LMS v19.1.5 and before is vulnerable to HTLM Injection. An attacker can inject malicious HTLM code in a message and send it to all the users in the application, resulting in executing the code and may lead to session hijacking and executing commands on the victim's browser.

- [https://github.com/saykino/CVE-2026-31281](https://github.com/saykino/CVE-2026-31281) :  ![starts](https://img.shields.io/github/stars/saykino/CVE-2026-31281.svg) ![forks](https://img.shields.io/github/forks/saykino/CVE-2026-31281.svg)


## CVE-2026-31280
 An issue in the Bluetooth RFCOMM service of Parani M10 Motorcycle Intercom v2.1.3 allows unauthorized attackers to cause a Denial of Service (DoS) via supplying crafted RFCOMM frames.

- [https://github.com/CipherX1802/CVE-2026-31280-Insecure-Bluetooth-RFCOMM-Leading-to-Device-Crash-in-Parani-M10-Intercom](https://github.com/CipherX1802/CVE-2026-31280-Insecure-Bluetooth-RFCOMM-Leading-to-Device-Crash-in-Parani-M10-Intercom) :  ![starts](https://img.shields.io/github/stars/CipherX1802/CVE-2026-31280-Insecure-Bluetooth-RFCOMM-Leading-to-Device-Crash-in-Parani-M10-Intercom.svg) ![forks](https://img.shields.io/github/forks/CipherX1802/CVE-2026-31280-Insecure-Bluetooth-RFCOMM-Leading-to-Device-Crash-in-Parani-M10-Intercom.svg)


## CVE-2026-31048
 An issue in the codepickle/code protocol of Pyro v3.x allows attackers to execute arbitrary code via supplying a crafted pickled string message.

- [https://github.com/Sif-0x01/security-advisories](https://github.com/Sif-0x01/security-advisories) :  ![starts](https://img.shields.io/github/stars/Sif-0x01/security-advisories.svg) ![forks](https://img.shields.io/github/forks/Sif-0x01/security-advisories.svg)


## CVE-2026-29955
 The `/registercrd` endpoint in KubePlus 4.14 in the kubeconfiggenerator component is vulnerable to command injection. The component uses `subprocess.Popen()` with `shell=True` parameter to execute shell commands, and the user-supplied `chartName` parameter is directly concatenated into the command string without any sanitization or validation. An attacker can inject arbitrary shell commands by crafting a malicious `chartName` parameter value.

- [https://github.com/b0b0haha/CVE-2026-29955](https://github.com/b0b0haha/CVE-2026-29955) :  ![starts](https://img.shields.io/github/stars/b0b0haha/CVE-2026-29955.svg) ![forks](https://img.shields.io/github/forks/b0b0haha/CVE-2026-29955.svg)


## CVE-2026-29628
 A stack overflow in the experimental/tinyobj_loader_opt.h file of tinyobjloader commit d56555b allows attackers to cause a Denial of Service (DoS) via supplying a crafted .mtl file.

- [https://github.com/kiyochii/CVE-2026-29628](https://github.com/kiyochii/CVE-2026-29628) :  ![starts](https://img.shields.io/github/stars/kiyochii/CVE-2026-29628.svg) ![forks](https://img.shields.io/github/forks/kiyochii/CVE-2026-29628.svg)


## CVE-2026-25769
 Wazuh is a free and open source platform used for threat prevention, detection, and response. Versions 4.0.0 through 4.14.2 have a Remote Code Execution (RCE) vulnerability due to Deserialization of Untrusted Data). All Wazuh deployments using cluster mode (master/worker architecture) and any organization with a compromised worker node (e.g., through initial access, insider threat, or supply chain attack) are impacted. An attacker who gains access to a worker node (through any means) can achieve full RCE on the master node with root privileges. Version 4.14.3 fixes the issue.

- [https://github.com/0xBlackash/CVE-2026-25769](https://github.com/0xBlackash/CVE-2026-25769) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-25769.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-25769.svg)


## CVE-2026-6201
 A vulnerability was identified in CodeAstro Online Job Portal 1.0. The impacted element is an unknown function of the file /jobs/job-delete.php of the component Delete Job Posting Handler. Such manipulation of the argument ID leads to improper access controls. The attack can be launched remotely. The exploit is publicly available and might be used.

- [https://github.com/Xmyronn/CVE-2026-6201-IDOR](https://github.com/Xmyronn/CVE-2026-6201-IDOR) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-6201-IDOR.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-6201-IDOR.svg)


## CVE-2026-6184
 A weakness has been identified in code-projects Simple Content Management System 1.0. This affects an unknown part of the file /web/admin/welcome.php. Executing a manipulation of the argument News Title can lead to cross site scripting. The attack can be executed remotely. The exploit has been made available to the public and could be used for attacks.

- [https://github.com/Xmyronn/CVE-2026-6184-stored-XSS](https://github.com/Xmyronn/CVE-2026-6184-stored-XSS) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-6184-stored-XSS.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-6184-stored-XSS.svg)


## CVE-2026-6183
 A security flaw has been discovered in code-projects Simple Content Management System 1.0. Affected by this issue is some unknown functionality of the file /web/index.php. Performing a manipulation of the argument ID results in sql injection. Remote exploitation of the attack is possible. The exploit has been released to the public and may be used for attacks.

- [https://github.com/Xmyronn/CVE-2026-6183-SQLI](https://github.com/Xmyronn/CVE-2026-6183-SQLI) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-6183-SQLI.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-6183-SQLI.svg)


## CVE-2026-6182
 A vulnerability was identified in code-projects Simple Content Management System 1.0. Affected by this vulnerability is an unknown functionality of the file /web/admin/login.php. Such manipulation of the argument User leads to sql injection. The attack may be launched remotely. The exploit is publicly available and might be used.

- [https://github.com/Xmyronn/CVE-2026-6182-SQLI-auth](https://github.com/Xmyronn/CVE-2026-6182-SQLI-auth) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-6182-SQLI-auth.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-6182-SQLI-auth.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478](https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478) :  ![starts](https://img.shields.io/github/stars/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg) ![forks](https://img.shields.io/github/forks/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)


## CVE-2025-59528
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5, Flowise is vulnerable to remote code execution. The CustomMCP node allows users to input configuration settings for connecting to an external MCP server. This node parses the user-provided mcpServerConfig string to build the MCP server configuration. However, during this process, it executes JavaScript code without any security validation. Specifically, inside the convertToValidJSONString function, user input is directly passed to the Function() constructor, which evaluates and executes the input as JavaScript code. Since this runs with full Node.js runtime privileges, it can access dangerous modules such as child_process and fs. This issue has been patched in version 3.0.6.

- [https://github.com/kartik2005221/CVE-2025-58434-AND-59528-POC](https://github.com/kartik2005221/CVE-2025-58434-AND-59528-POC) :  ![starts](https://img.shields.io/github/stars/kartik2005221/CVE-2025-58434-AND-59528-POC.svg) ![forks](https://img.shields.io/github/forks/kartik2005221/CVE-2025-58434-AND-59528-POC.svg)
- [https://github.com/vanhari/CVE-2025-59528](https://github.com/vanhari/CVE-2025-59528) :  ![starts](https://img.shields.io/github/stars/vanhari/CVE-2025-59528.svg) ![forks](https://img.shields.io/github/forks/vanhari/CVE-2025-59528.svg)
- [https://github.com/UsifAraby/CVE-2025-59528-POC](https://github.com/UsifAraby/CVE-2025-59528-POC) :  ![starts](https://img.shields.io/github/stars/UsifAraby/CVE-2025-59528-POC.svg) ![forks](https://img.shields.io/github/forks/UsifAraby/CVE-2025-59528-POC.svg)


## CVE-2025-59213
 Improper neutralization of special elements used in an sql command ('sql injection') in Microsoft Configuration Manager allows an unauthorized attacker to elevate privileges over an adjacent network.

- [https://github.com/synacktiv/CVE-2025-59213](https://github.com/synacktiv/CVE-2025-59213) :  ![starts](https://img.shields.io/github/stars/synacktiv/CVE-2025-59213.svg) ![forks](https://img.shields.io/github/forks/synacktiv/CVE-2025-59213.svg)


## CVE-2025-55320
 Improper neutralization of special elements used in an sql command ('sql injection') in Microsoft Configuration Manager allows an authorized attacker to elevate privileges over an adjacent network.

- [https://github.com/synacktiv/CVE-2025-55320](https://github.com/synacktiv/CVE-2025-55320) :  ![starts](https://img.shields.io/github/stars/synacktiv/CVE-2025-55320.svg) ![forks](https://img.shields.io/github/forks/synacktiv/CVE-2025-55320.svg)


## CVE-2025-54416
 tj-actions/branch-names is a Github actions repository that contains workflows to retrieve branch or tag names with support for all events. In versions 8.2.1 and below, a critical vulnerability has been identified in the tj-actions/branch-names' GitHub Action workflow which allows arbitrary command execution in downstream workflows. This issue arises due to inconsistent input sanitization and unescaped output, enabling malicious actors to exploit specially crafted branch names or tags. While internal sanitization mechanisms have been implemented, the action outputs remain vulnerable, exposing consuming workflows to significant security risks. This is fixed in version 9.0.0

- [https://github.com/HexborneStudio/atlas-tj-actions-poc](https://github.com/HexborneStudio/atlas-tj-actions-poc) :  ![starts](https://img.shields.io/github/stars/HexborneStudio/atlas-tj-actions-poc.svg) ![forks](https://img.shields.io/github/forks/HexborneStudio/atlas-tj-actions-poc.svg)


## CVE-2025-37899
be in the smb2_sess_setup function which makes use of sess-user.

- [https://github.com/ccss17/o3_finds_cve-2025-37899](https://github.com/ccss17/o3_finds_cve-2025-37899) :  ![starts](https://img.shields.io/github/stars/ccss17/o3_finds_cve-2025-37899.svg) ![forks](https://img.shields.io/github/forks/ccss17/o3_finds_cve-2025-37899.svg)


## CVE-2025-23266
 NVIDIA Container Toolkit for all platforms contains a vulnerability in some hooks used to initialize the container, where an attacker could execute arbitrary code with elevated permissions. A successful exploit of this vulnerability might lead to escalation of privileges, data tampering, information disclosure, and denial of service.

- [https://github.com/ForeverLX/security-research](https://github.com/ForeverLX/security-research) :  ![starts](https://img.shields.io/github/stars/ForeverLX/security-research.svg) ![forks](https://img.shields.io/github/forks/ForeverLX/security-research.svg)


## CVE-2025-8110
 Improper Symbolic link handling in the PutContents API in Gogs allows Local Execution of Code.

- [https://github.com/popyue/CVE-2025-8110](https://github.com/popyue/CVE-2025-8110) :  ![starts](https://img.shields.io/github/stars/popyue/CVE-2025-8110.svg) ![forks](https://img.shields.io/github/forks/popyue/CVE-2025-8110.svg)


## CVE-2024-45337
 Applications and libraries which misuse connection.serverAuthenticate (via callback field ServerConfig.PublicKeyCallback) may be susceptible to an authorization bypass. The documentation for ServerConfig.PublicKeyCallback says that "A call to this function does not guarantee that the key offered is in fact used to authenticate." Specifically, the SSH protocol allows clients to inquire about whether a public key is acceptable before proving control of the corresponding private key. PublicKeyCallback may be called with multiple keys, and the order in which the keys were provided cannot be used to infer which key the client successfully authenticated with, if any. Some applications, which store the key(s) passed to PublicKeyCallback (or derived information) and make security relevant determinations based on it once the connection is established, may make incorrect assumptions. For example, an attacker may send public keys A and B, and then authenticate with A. PublicKeyCallback would be called only twice, first with A and then with B. A vulnerable application may then make authorization decisions based on key B for which the attacker does not actually control the private key. Since this API is widely misused, as a partial mitigation golang.org/x/cry...@v0.31.0 enforces the property that, when successfully authenticating via public key, the last key passed to ServerConfig.PublicKeyCallback will be the key used to authenticate the connection. PublicKeyCallback will now be called multiple times with the same key, if necessary. Note that the client may still not control the last key passed to PublicKeyCallback if the connection is then authenticated with a different method, such as PasswordCallback, KeyboardInteractiveCallback, or NoClientAuth. Users should be using the Extensions field of the Permissions return value from the various authentication callbacks to record data associated with the authentication attempt instead of referencing external state. Once the connection is established the state corresponding to the successful authentication attempt can be retrieved via the ServerConn.Permissions field. Note that some third-party libraries misuse the Permissions type by sharing it across authentication attempts; users of third-party libraries should refer to the relevant projects for guidance.

- [https://github.com/Backline-playground/gogs](https://github.com/Backline-playground/gogs) :  ![starts](https://img.shields.io/github/stars/Backline-playground/gogs.svg) ![forks](https://img.shields.io/github/forks/Backline-playground/gogs.svg)


## CVE-2023-30367
 Multi-Remote Next Generation Connection Manager (mRemoteNG) is free software that enables users to store and manage multi-protocol connection configurations to remotely connect to systems. mRemoteNG configuration files can be stored in an encrypted state on disk. mRemoteNG version = v1.76.20 and = 1.77.3-dev loads configuration files in plain text into memory (after decrypting them if necessary) at application start-up, even if no connection has been established yet. This allows attackers to access contents of configuration files in plain text through a memory dump and thus compromise user credentials when no custom password encryption key has been set. This also bypasses the connection configuration file encryption setting by dumping already decrypted configurations from memory.

- [https://github.com/S1lkys/CVE-2023-30367-mRemoteNG-password-dumper](https://github.com/S1lkys/CVE-2023-30367-mRemoteNG-password-dumper) :  ![starts](https://img.shields.io/github/stars/S1lkys/CVE-2023-30367-mRemoteNG-password-dumper.svg) ![forks](https://img.shields.io/github/forks/S1lkys/CVE-2023-30367-mRemoteNG-password-dumper.svg)


## CVE-2023-29357
 Microsoft SharePoint Server Elevation of Privilege Vulnerability

- [https://github.com/DonVorrin/CVE-2023-29357](https://github.com/DonVorrin/CVE-2023-29357) :  ![starts](https://img.shields.io/github/stars/DonVorrin/CVE-2023-29357.svg) ![forks](https://img.shields.io/github/forks/DonVorrin/CVE-2023-29357.svg)


## CVE-2023-6972
 The Backup Migration plugin for WordPress is vulnerable to Path Traversal in all versions up to, and including, 1.3.9 via the 'content-backups' and 'content-name', 'content-manifest', or 'content-bmitmp' and 'content-identy' HTTP headers. This makes it possible for unauthenticated attackers to delete arbitrary files, including the wp-config.php file, which can make site takeover and remote code execution possible.

- [https://github.com/0x00phantom-hat/CVE-2023-6972-Exploit-Arbitrary-File-Deletion](https://github.com/0x00phantom-hat/CVE-2023-6972-Exploit-Arbitrary-File-Deletion) :  ![starts](https://img.shields.io/github/stars/0x00phantom-hat/CVE-2023-6972-Exploit-Arbitrary-File-Deletion.svg) ![forks](https://img.shields.io/github/forks/0x00phantom-hat/CVE-2023-6972-Exploit-Arbitrary-File-Deletion.svg)


## CVE-2023-6553
 The Backup Migration plugin for WordPress is vulnerable to Remote Code Execution in all versions up to, and including, 1.3.7 via the /includes/backup-heart.php file. This is due to an attacker being able to control the values passed to an include, and subsequently leverage that to achieve remote code execution. This makes it possible for unauthenticated attackers to easily execute code on the server.

- [https://github.com/0x00phantom-hat/CVE-2023-6553-RCE-Exploit](https://github.com/0x00phantom-hat/CVE-2023-6553-RCE-Exploit) :  ![starts](https://img.shields.io/github/stars/0x00phantom-hat/CVE-2023-6553-RCE-Exploit.svg) ![forks](https://img.shields.io/github/forks/0x00phantom-hat/CVE-2023-6553-RCE-Exploit.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/Taldrid1/cve-2021-41773](https://github.com/Taldrid1/cve-2021-41773) :  ![starts](https://img.shields.io/github/stars/Taldrid1/cve-2021-41773.svg) ![forks](https://img.shields.io/github/forks/Taldrid1/cve-2021-41773.svg)


## CVE-2021-22986
 On BIG-IP versions 16.0.x before 16.0.1.1, 15.1.x before 15.1.2.1, 14.1.x before 14.1.4, 13.1.x before 13.1.3.6, and 12.1.x before 12.1.5.3 amd BIG-IQ 7.1.0.x before 7.1.0.3 and 7.0.0.x before 7.0.0.2, the iControl REST interface has an unauthenticated remote command execution vulnerability. Note: Software versions which have reached End of Software Development (EoSD) are not evaluated.

- [https://github.com/whatheheckisthis/BigIP-iControl-RCE-Research](https://github.com/whatheheckisthis/BigIP-iControl-RCE-Research) :  ![starts](https://img.shields.io/github/stars/whatheheckisthis/BigIP-iControl-RCE-Research.svg) ![forks](https://img.shields.io/github/forks/whatheheckisthis/BigIP-iControl-RCE-Research.svg)


## CVE-2020-6864
 ZTE E8820V3 router product is impacted by an information leak vulnerability. Attackers could use this vulnerability to to gain wireless passwords. After obtaining the wireless password, the attacker could collect information and attack the router.

- [https://github.com/gigachadusers/cve-2020-6864](https://github.com/gigachadusers/cve-2020-6864) :  ![starts](https://img.shields.io/github/stars/gigachadusers/cve-2020-6864.svg) ![forks](https://img.shields.io/github/forks/gigachadusers/cve-2020-6864.svg)


## CVE-2020-0796
 A remote code execution vulnerability exists in the way that the Microsoft Server Message Block 3.1.1 (SMBv3) protocol handles certain requests, aka 'Windows SMBv3 Client/Server Remote Code Execution Vulnerability'.

- [https://github.com/adrielni7651/smb-adtech-platform](https://github.com/adrielni7651/smb-adtech-platform) :  ![starts](https://img.shields.io/github/stars/adrielni7651/smb-adtech-platform.svg) ![forks](https://img.shields.io/github/forks/adrielni7651/smb-adtech-platform.svg)


## CVE-2006-3392
 Webmin before 1.290 and Usermin before 1.220 calls the simplify_path function before decoding HTML, which allows remote attackers to read arbitrary files, as demonstrated using "..%01" sequences, which bypass the removal of "../" sequences before bytes such as "%01" are removed from the filename.  NOTE: This is a different issue than CVE-2006-3274.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)

