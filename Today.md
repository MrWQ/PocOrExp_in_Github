# Update 2026-04-02
## CVE-2026-34227
 Sliver is a command and control framework that uses a custom Wireguard netstack. Prior to version 1.7.4, a single click on a malicious link gives an unauthenticated attacker immediate, silent control over every active C2 session or beacon, capable of exfiltrating all collected target data (e.g. SSH keys, ntds.dit) or destroying the entire compromised infrastructure, entirely through the operator's own browser. This issue has been patched in version 1.7.4.

- [https://github.com/skoveit/CVE-2026-34227](https://github.com/skoveit/CVE-2026-34227) :  ![starts](https://img.shields.io/github/stars/skoveit/CVE-2026-34227.svg) ![forks](https://img.shields.io/github/forks/skoveit/CVE-2026-34227.svg)


## CVE-2026-34200
 Nhost is an open source Firebase alternative with GraphQL. Prior to version 1.41.0, The Nhost CLI MCP server, when explicitly configured to listen on a network port, applies no inbound authentication and does not enforce strict CORS. This allows a malicious website visited on the same machine to issue cross-origin requests to the MCP server and invoke privileged tools using the developer's locally configured credentials. This vulnerability requires two explicit, non-default configuration steps to be exploitable. The default nhost mcp start configuration is not affected. This issue has been patched in version 1.41.0.

- [https://github.com/skoveit/CVE-2026-34200](https://github.com/skoveit/CVE-2026-34200) :  ![starts](https://img.shields.io/github/stars/skoveit/CVE-2026-34200.svg) ![forks](https://img.shields.io/github/forks/skoveit/CVE-2026-34200.svg)


## CVE-2026-34070
 LangChain is a framework for building agents and LLM-powered applications. Prior to version 1.2.22, multiple functions in langchain_core.prompts.loading read files from paths embedded in deserialized config dicts without validating against directory traversal or absolute path injection. When an application passes user-influenced prompt configurations to load_prompt() or load_prompt_from_config(), an attacker can read arbitrary files on the host filesystem, constrained only by file-extension checks (.txt for templates, .json/.yaml for examples). This issue has been patched in version 1.2.22.

- [https://github.com/Rickidevs/CVE-2026-34070](https://github.com/Rickidevs/CVE-2026-34070) :  ![starts](https://img.shields.io/github/stars/Rickidevs/CVE-2026-34070.svg) ![forks](https://img.shields.io/github/forks/Rickidevs/CVE-2026-34070.svg)


## CVE-2026-34036
 Dolibarr is an enterprise resource planning (ERP) and customer relationship management (CRM) software package. In versions 22.0.4 and prior, there is a Local File Inclusion (LFI) vulnerability in the core AJAX endpoint /core/ajax/selectobject.php. By manipulating the objectdesc parameter and exploiting a fail-open logic flaw in the core access control function restrictedArea(), an authenticated user with no specific privileges can read the contents of arbitrary non-PHP files on the server (such as .env, .htaccess, configuration backups, or logs…). At time of publication, there are no publicly available patches.

- [https://github.com/cnf409/CVE-2026-34036](https://github.com/cnf409/CVE-2026-34036) :  ![starts](https://img.shields.io/github/stars/cnf409/CVE-2026-34036.svg) ![forks](https://img.shields.io/github/forks/cnf409/CVE-2026-34036.svg)


## CVE-2026-33634
 Trivy is a security scanner. On March 19, 2026, a threat actor used compromised credentials to publish a malicious Trivy v0.69.4 release, force-push 76 of 77 version tags in `aquasecurity/trivy-action` to credential-stealing malware, and replace all 7 tags in `aquasecurity/setup-trivy` with malicious commits. This incident is a continuation of the supply chain attack that began in late February 2026. Following the initial disclosure on March 1, credential rotation was performed but was not atomic (not all credentials were revoked simultaneously). The attacker could have use a valid token to exfiltrate newly rotated secrets during the rotation window (which lasted a few days). This could have allowed the attacker to retain access and execute the March 19 attack. Affected components include the `aquasecurity/trivy` Go / Container image version 0.69.4, the `aquasecurity/trivy-action` GitHub Action versions 0.0.1 – 0.34.2 (76/77), and the`aquasecurity/setup-trivy` GitHub Action versions 0.2.0 – 0.2.6, prior to the recreation of 0.2.6 with a safe commit. Known safe versions include versions 0.69.2 and 0.69.3 of the Trivy binary, version 0.35.0 of trivy-action, and version 0.2.6 of setup-trivy. Additionally, take other mitigations to ensure the safety of secrets. If there is any possibility that a compromised version ran in one's environment, all secrets accessible to affected pipelines must be treated as exposed and rotated immediately. Check whether one's organization pulled or executed Trivy v0.69.4 from any source. Remove any affected artifacts immediately. Review all workflows using `aquasecurity/trivy-action` or `aquasecurity/setup-trivy`. Those who referenced a version tag rather than a full commit SHA should check workflow run logs from March 19–20, 2026 for signs of compromise. Look for repositories named `tpcp-docs` in one's GitHub organization. The presence of such a repository may indicate that the fallback exfiltration mechanism was triggered and secrets were successfully stolen. Pin GitHub Actions to full, immutable commit SHA hashes, don't use mutable version tags.

- [https://github.com/AshleyT3/docker-socket-risk-demos](https://github.com/AshleyT3/docker-socket-risk-demos) :  ![starts](https://img.shields.io/github/stars/AshleyT3/docker-socket-risk-demos.svg) ![forks](https://img.shields.io/github/forks/AshleyT3/docker-socket-risk-demos.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/EQSTLab/CVE-2026-33017](https://github.com/EQSTLab/CVE-2026-33017) :  ![starts](https://img.shields.io/github/stars/EQSTLab/CVE-2026-33017.svg) ![forks](https://img.shields.io/github/forks/EQSTLab/CVE-2026-33017.svg)


## CVE-2026-32794
Users are recommended to upgrade to version 1.12.0, which fixes the issue.

- [https://github.com/SnailSploit/CVE-2026-32794](https://github.com/SnailSploit/CVE-2026-32794) :  ![starts](https://img.shields.io/github/stars/SnailSploit/CVE-2026-32794.svg) ![forks](https://img.shields.io/github/forks/SnailSploit/CVE-2026-32794.svg)


## CVE-2026-32321
 ClipBucket v5 is an open source video sharing platform. An authenticated time-based blind SQL injection vulnerability exists in ClipBucket prior to 5.5.3 #80 within the `actions/ajax.php` endpoint. Due to insufficient input sanitization of the `userid` parameter, an authenticated attacker can execute arbitrary SQL queries, leading to full database disclosure and potential administrative account takeover. Version 5.5.3 #80 fixes the issue.

- [https://github.com/drkim-dev/CVE-2026-32321](https://github.com/drkim-dev/CVE-2026-32321) :  ![starts](https://img.shields.io/github/stars/drkim-dev/CVE-2026-32321.svg) ![forks](https://img.shields.io/github/forks/drkim-dev/CVE-2026-32321.svg)


## CVE-2026-32096
 Plunk is an open-source email platform built on top of AWS SES. Prior to 0.7.0, a Server-Side Request Forgery (SSRF) vulnerability existed in the SNS webhook handler. An unauthenticated attacker could send a crafted request that caused the server to make an arbitrary outbound HTTP GET request to any host accessible from the server. This vulnerability is fixed in 0.7.0.

- [https://github.com/andrebhu/CVE-2026-32096](https://github.com/andrebhu/CVE-2026-32096) :  ![starts](https://img.shields.io/github/stars/andrebhu/CVE-2026-32096.svg) ![forks](https://img.shields.io/github/forks/andrebhu/CVE-2026-32096.svg)


## CVE-2026-29000
 pac4j-jwt versions prior to 4.5.9, 5.7.9, and 6.3.3 contain an authentication bypass vulnerability in JwtAuthenticator when processing encrypted JWTs that allows remote attackers to forge authentication tokens. Attackers who possess the server's RSA public key can create a JWE-wrapped PlainJWT with arbitrary subject and role claims, bypassing signature verification to authenticate as any user including administrators.

- [https://github.com/ClayOfGilgamesh/CVE-2026-29000](https://github.com/ClayOfGilgamesh/CVE-2026-29000) :  ![starts](https://img.shields.io/github/stars/ClayOfGilgamesh/CVE-2026-29000.svg) ![forks](https://img.shields.io/github/forks/ClayOfGilgamesh/CVE-2026-29000.svg)
- [https://github.com/0xW1LD/CVE-2026-29000](https://github.com/0xW1LD/CVE-2026-29000) :  ![starts](https://img.shields.io/github/stars/0xW1LD/CVE-2026-29000.svg) ![forks](https://img.shields.io/github/forks/0xW1LD/CVE-2026-29000.svg)


## CVE-2026-24061
 telnetd in GNU Inetutils through 2.7 allows remote authentication bypass via a "-f root" value for the USER environment variable.

- [https://github.com/athack-ctf/chall2026-telneted](https://github.com/athack-ctf/chall2026-telneted) :  ![starts](https://img.shields.io/github/stars/athack-ctf/chall2026-telneted.svg) ![forks](https://img.shields.io/github/forks/athack-ctf/chall2026-telneted.svg)


## CVE-2026-22777
 ComfyUI-Manager is an extension designed to enhance the usability of ComfyUI. Prior to versions 3.39.2 and 4.0.5, an attacker can inject special characters into HTTP query parameters to add arbitrary configuration values to the config.ini file. This can lead to security setting tampering or modification of application behavior. This issue has been patched in versions 3.39.2 and 4.0.5.

- [https://github.com/wcnmwcis/CVE-2026-22777](https://github.com/wcnmwcis/CVE-2026-22777) :  ![starts](https://img.shields.io/github/stars/wcnmwcis/CVE-2026-22777.svg) ![forks](https://img.shields.io/github/forks/wcnmwcis/CVE-2026-22777.svg)


## CVE-2026-21717
This vulnerability affects **20.x, 22.x, 24.x, and 25.x**.

- [https://github.com/dajneem23/CVE-2026-21717](https://github.com/dajneem23/CVE-2026-21717) :  ![starts](https://img.shields.io/github/stars/dajneem23/CVE-2026-21717.svg) ![forks](https://img.shields.io/github/forks/dajneem23/CVE-2026-21717.svg)


## CVE-2026-3888
 Local privilege escalation in snapd on Linux allows local attackers to get root privilege by re-creating snap's private /tmp directory when systemd-tmpfiles is configured to automatically clean up this directory. This issue affects Ubuntu 16.04 LTS, 18.04 LTS, 20.04 LTS, 22.04 LTS, and 24.04 LTS.

- [https://github.com/DanielTangnes/CVE-2026-3888](https://github.com/DanielTangnes/CVE-2026-3888) :  ![starts](https://img.shields.io/github/stars/DanielTangnes/CVE-2026-3888.svg) ![forks](https://img.shields.io/github/forks/DanielTangnes/CVE-2026-3888.svg)


## CVE-2026-3055
 Insufficient input validation in NetScaler ADC and NetScaler Gateway when configured as a SAML IDP leading to memory overread

- [https://github.com/fevar54/CVE-2026-3055-Scanner---Herramienta-de-Detecci-n](https://github.com/fevar54/CVE-2026-3055-Scanner---Herramienta-de-Detecci-n) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-3055-Scanner---Herramienta-de-Detecci-n.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-3055-Scanner---Herramienta-de-Detecci-n.svg)
- [https://github.com/fevar54/CVE-2026-3055---Citrix-NetScaler-Memory-Overread-PoC](https://github.com/fevar54/CVE-2026-3055---Citrix-NetScaler-Memory-Overread-PoC) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-3055---Citrix-NetScaler-Memory-Overread-PoC.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-3055---Citrix-NetScaler-Memory-Overread-PoC.svg)


## CVE-2026-2959
 A vulnerability was detected in D-Link DWR-M960 1.01.07. Affected by this vulnerability is the function sub_44E0F8 of the file /boafrm/formNewSchedule. Performing a manipulation of the argument url results in stack-based buffer overflow. Remote exploitation of the attack is possible. The exploit is now public and may be used.

- [https://github.com/padayali-JD/CVE-2026-29598](https://github.com/padayali-JD/CVE-2026-29598) :  ![starts](https://img.shields.io/github/stars/padayali-JD/CVE-2026-29598.svg) ![forks](https://img.shields.io/github/forks/padayali-JD/CVE-2026-29598.svg)


## CVE-2026-0848
 NLTK versions =3.9.2 are vulnerable to arbitrary code execution due to improper input validation in the StanfordSegmenter module. The module dynamically loads external Java .jar files without verification or sandboxing. An attacker can supply or replace the JAR file, enabling the execution of arbitrary Java bytecode at import time. This vulnerability can be exploited through methods such as model poisoning, MITM attacks, or dependency poisoning, leading to remote code execution. The issue arises from the direct execution of the JAR file via subprocess with unvalidated classpath input, allowing malicious classes to execute when loaded by the JVM.

- [https://github.com/fevar54/CVE-2026-0848-Scanner---Herramienta-de-Detecci-n](https://github.com/fevar54/CVE-2026-0848-Scanner---Herramienta-de-Detecci-n) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-0848-Scanner---Herramienta-de-Detecci-n.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-0848-Scanner---Herramienta-de-Detecci-n.svg)
- [https://github.com/fevar54/CVE-2026-0848-PoC-Improper-Input-Validation](https://github.com/fevar54/CVE-2026-0848-PoC-Improper-Input-Validation) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-0848-PoC-Improper-Input-Validation.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-0848-PoC-Improper-Input-Validation.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478](https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478) :  ![starts](https://img.shields.io/github/stars/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg) ![forks](https://img.shields.io/github/forks/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)


## CVE-2025-65482
 An XML External Entity (XXE) vulnerability in opensagres XDocReport v0.9.2 to v2.0.3 allows attackers to execute arbitrary code via uploading a crafted .docx file.

- [https://github.com/AT190510-Cuong/CVE-2025-65482-XXE-](https://github.com/AT190510-Cuong/CVE-2025-65482-XXE-) :  ![starts](https://img.shields.io/github/stars/AT190510-Cuong/CVE-2025-65482-XXE-.svg) ![forks](https://img.shields.io/github/forks/AT190510-Cuong/CVE-2025-65482-XXE-.svg)


## CVE-2025-64087
 A Server-Side Template Injection (SSTI) vulnerability in the FreeMarker component of opensagres XDocReport v1.0.0 to v2.1.0 allows attackers to execute arbitrary code via injecting crafted template expressions.

- [https://github.com/AT190510-Cuong/CVE-2025-64087-SSTI-](https://github.com/AT190510-Cuong/CVE-2025-64087-SSTI-) :  ![starts](https://img.shields.io/github/stars/AT190510-Cuong/CVE-2025-64087-SSTI-.svg) ![forks](https://img.shields.io/github/forks/AT190510-Cuong/CVE-2025-64087-SSTI-.svg)


## CVE-2025-62429
 ClipBucket v5 is an open source video sharing platform. Prior to version 5.5.2 #147, ClipBucket v5 is vulnerable to arbitrary PHP code execution. In /upload/admin_area/actions/update_launch.php, the "type" parameter from a POST request is embedded into PHP tags and executed. Proper sanitization is not performed, and by injecting malicious code an attacker can execute arbitrary PHP code. This allows an attacker to achieve RCE. This issue has been resolved in version 5.5.2 #147.

- [https://github.com/drkim-dev/CVE-2025-62429](https://github.com/drkim-dev/CVE-2025-62429) :  ![starts](https://img.shields.io/github/stars/drkim-dev/CVE-2025-62429.svg) ![forks](https://img.shields.io/github/forks/drkim-dev/CVE-2025-62429.svg)


## CVE-2025-54123
 Hoverfly is an open source API simulation tool. In versions 1.11.3 and prior, the middleware functionality in Hoverfly is vulnerable to command injection vulnerability at `/api/v2/hoverfly/middleware` endpoint due to insufficient validation and sanitization in user input. The vulnerability exists in the middleware management API endpoint `/api/v2/hoverfly/middleware`. This issue is born due to combination of three code level flaws: Insufficient Input Validation in middleware.go line 94-96; Unsafe Command Execution in local_middleware.go line 14-19; and Immediate Execution During Testing in hoverfly_service.go line 173. This allows an attacker to gain remote code execution (RCE) on any system running the vulnerable Hoverfly service. Since the input is directly passed to system commands without proper checks, an attacker can upload a malicious payload or directly execute arbitrary commands (including reverse shells) on the host server with the privileges of the Hoverfly process. Commit 17e60a9bc78826deb4b782dca1c1abd3dbe60d40 in version 1.12.0 disables the set middleware API by default, and subsequent changes to documentation make users aware of the security changes of exposing the set middleware API.

- [https://github.com/davidzzo23/CVE-2025-54123](https://github.com/davidzzo23/CVE-2025-54123) :  ![starts](https://img.shields.io/github/stars/davidzzo23/CVE-2025-54123.svg) ![forks](https://img.shields.io/github/forks/davidzzo23/CVE-2025-54123.svg)


## CVE-2025-33073
 Improper access control in Windows SMB allows an authorized attacker to elevate privileges over a network.

- [https://github.com/EgCupCake/cupntlm-Automated-Exploit-For-CVE-2025-33073-](https://github.com/EgCupCake/cupntlm-Automated-Exploit-For-CVE-2025-33073-) :  ![starts](https://img.shields.io/github/stars/EgCupCake/cupntlm-Automated-Exploit-For-CVE-2025-33073-.svg) ![forks](https://img.shields.io/github/forks/EgCupCake/cupntlm-Automated-Exploit-For-CVE-2025-33073-.svg)


## CVE-2025-6514
 mcp-remote is exposed to OS command injection when connecting to untrusted MCP servers due to crafted input from the authorization_endpoint response URL

- [https://github.com/darshjme/mcp-security-audit](https://github.com/darshjme/mcp-security-audit) :  ![starts](https://img.shields.io/github/stars/darshjme/mcp-security-audit.svg) ![forks](https://img.shields.io/github/forks/darshjme/mcp-security-audit.svg)


## CVE-2024-11680
 ProjectSend versions prior to r1720 are affected by an improper authentication vulnerability. Remote, unauthenticated attackers can exploit this flaw by sending crafted HTTP requests to options.php, enabling unauthorized modification of the application's configuration. Successful exploitation allows attackers to create accounts, upload webshells, and embed malicious JavaScript.

- [https://github.com/qucklecrabik/CVE-2024-11680](https://github.com/qucklecrabik/CVE-2024-11680) :  ![starts](https://img.shields.io/github/stars/qucklecrabik/CVE-2024-11680.svg) ![forks](https://img.shields.io/github/forks/qucklecrabik/CVE-2024-11680.svg)


## CVE-2024-6387
 A security regression (CVE-2006-5051) was discovered in OpenSSH's server (sshd). There is a race condition which can lead sshd to handle some signals in an unsafe manner. An unauthenticated, remote attacker may be able to trigger it by failing to authenticate within a set time period.

- [https://github.com/kaleth4/CVE-2024-6387](https://github.com/kaleth4/CVE-2024-6387) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2024-6387.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2024-6387.svg)


## CVE-2023-3107
 A set of carefully crafted ipv6 packets can trigger an integer overflow in the calculation of a fragment reassembled packet's payload length field. This allows an attacker to trigger a kernel panic, resulting in a denial of service.

- [https://github.com/bugprove/cve-2023-31070](https://github.com/bugprove/cve-2023-31070) :  ![starts](https://img.shields.io/github/stars/bugprove/cve-2023-31070.svg) ![forks](https://img.shields.io/github/forks/bugprove/cve-2023-31070.svg)


## CVE-2022-46364
 A SSRF vulnerability in parsing the href attribute of XOP:Include in MTOM requests in versions of Apache CXF before 3.5.5 and 3.4.10 allows an attacker to perform SSRF style attacks on webservices that take at least one parameter of any type. 

- [https://github.com/0xmid00/CVE-2022-46364-poc](https://github.com/0xmid00/CVE-2022-46364-poc) :  ![starts](https://img.shields.io/github/stars/0xmid00/CVE-2022-46364-poc.svg) ![forks](https://img.shields.io/github/forks/0xmid00/CVE-2022-46364-poc.svg)


## CVE-2022-40684
 An authentication bypass using an alternate path or channel [CWE-288] in Fortinet FortiOS version 7.2.0 through 7.2.1 and 7.0.0 through 7.0.6, FortiProxy version 7.2.0 and version 7.0.0 through 7.0.6 and FortiSwitchManager version 7.2.0 and 7.0.0 allows an unauthenticated atttacker to perform operations on the administrative interface via specially crafted HTTP or HTTPS requests.

- [https://github.com/pintukumar-sutradhar/fortigate-cve-2022-40684-tool](https://github.com/pintukumar-sutradhar/fortigate-cve-2022-40684-tool) :  ![starts](https://img.shields.io/github/stars/pintukumar-sutradhar/fortigate-cve-2022-40684-tool.svg) ![forks](https://img.shields.io/github/forks/pintukumar-sutradhar/fortigate-cve-2022-40684-tool.svg)


## CVE-2022-30190
Please see the MSRC Blog Entry for important information about steps you can take to protect your system from this vulnerability.

- [https://github.com/abbarhissarh/FollinaXploit](https://github.com/abbarhissarh/FollinaXploit) :  ![starts](https://img.shields.io/github/stars/abbarhissarh/FollinaXploit.svg) ![forks](https://img.shields.io/github/forks/abbarhissarh/FollinaXploit.svg)


## CVE-2022-26133
 SharedSecretClusterAuthenticator in Atlassian Bitbucket Data Center versions 5.14.0 and later before 7.6.14, 7.7.0 and later prior to 7.17.6, 7.18.0 and later prior to 7.18.4, 7.19.0 and later prior to 7.19.4, and 7.20.0 allow a remote, unauthenticated attacker to execute arbitrary code via Java deserialization.

- [https://github.com/abbarhissarh/CVE-2022-26133](https://github.com/abbarhissarh/CVE-2022-26133) :  ![starts](https://img.shields.io/github/stars/abbarhissarh/CVE-2022-26133.svg) ![forks](https://img.shields.io/github/forks/abbarhissarh/CVE-2022-26133.svg)


## CVE-2022-24124
 The query API in Casdoor before 1.13.1 has a SQL injection vulnerability related to the field and value parameters, as demonstrated by api/get-organizations.

- [https://github.com/abbarhissarh/CVE-2022-24124](https://github.com/abbarhissarh/CVE-2022-24124) :  ![starts](https://img.shields.io/github/stars/abbarhissarh/CVE-2022-24124.svg) ![forks](https://img.shields.io/github/forks/abbarhissarh/CVE-2022-24124.svg)


## CVE-2021-25076
 The WP User Frontend WordPress plugin before 3.5.26 does not validate and escape the status parameter before using it in a SQL statement in the Subscribers dashboard, leading to an SQL injection. Due to the lack of sanitisation and escaping, this could also lead to Reflected Cross-Site Scripting

- [https://github.com/abbarhissarh/CVE-2021-25076](https://github.com/abbarhissarh/CVE-2021-25076) :  ![starts](https://img.shields.io/github/stars/abbarhissarh/CVE-2021-25076.svg) ![forks](https://img.shields.io/github/forks/abbarhissarh/CVE-2021-25076.svg)


## CVE-2021-3156
 Sudo before 1.9.5p2 contains an off-by-one error that can result in a heap-based buffer overflow, which allows privilege escalation to root via "sudoedit -s" and a command-line argument that ends with a single backslash character.

- [https://github.com/r4v1nduu/CVE-2021-3156](https://github.com/r4v1nduu/CVE-2021-3156) :  ![starts](https://img.shields.io/github/stars/r4v1nduu/CVE-2021-3156.svg) ![forks](https://img.shields.io/github/forks/r4v1nduu/CVE-2021-3156.svg)


## CVE-2020-29607
 A file upload restriction bypass vulnerability in Pluck CMS before 4.7.13 allows an admin privileged user to gain access in the host through the "manage files" functionality, which may result in remote code execution.

- [https://github.com/abbarhissarh/CVE-2020-29607](https://github.com/abbarhissarh/CVE-2020-29607) :  ![starts](https://img.shields.io/github/stars/abbarhissarh/CVE-2020-29607.svg) ![forks](https://img.shields.io/github/forks/abbarhissarh/CVE-2020-29607.svg)


## CVE-2020-2551
 Vulnerability in the Oracle WebLogic Server product of Oracle Fusion Middleware (component: WLS Core Components). Supported versions that are affected are 10.3.6.0.0, 12.1.3.0.0, 12.2.1.3.0 and 12.2.1.4.0. Easily exploitable vulnerability allows unauthenticated attacker with network access via IIOP to compromise Oracle WebLogic Server. Successful attacks of this vulnerability can result in takeover of Oracle WebLogic Server. CVSS 3.0 Base Score 9.8 (Confidentiality, Integrity and Availability impacts). CVSS Vector: (CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H).

- [https://github.com/abbarhissarh/CVE-Exploit](https://github.com/abbarhissarh/CVE-Exploit) :  ![starts](https://img.shields.io/github/stars/abbarhissarh/CVE-Exploit.svg) ![forks](https://img.shields.io/github/forks/abbarhissarh/CVE-Exploit.svg)

