# Update 2026-04-16
## CVE-2026-40175
 Axios is a promise based HTTP client for the browser and Node.js. Prior to 1.15.0 and 0.3.1, the Axios library is vulnerable to a specific "Gadget" attack chain that allows Prototype Pollution in any third-party dependency to be escalated into Remote Code Execution (RCE) or Full Cloud Compromise (via AWS IMDSv2 bypass). This vulnerability is fixed in 1.15.0 and 0.3.1.

- [https://github.com/surri/audit-axios](https://github.com/surri/audit-axios) :  ![starts](https://img.shields.io/github/stars/surri/audit-axios.svg) ![forks](https://img.shields.io/github/forks/surri/audit-axios.svg)
- [https://github.com/LeeKangHyun/axios-security-guide](https://github.com/LeeKangHyun/axios-security-guide) :  ![starts](https://img.shields.io/github/stars/LeeKangHyun/axios-security-guide.svg) ![forks](https://img.shields.io/github/forks/LeeKangHyun/axios-security-guide.svg)


## CVE-2026-35585
 File Browser is a file managing interface for uploading, deleting, previewing, renaming, and editing files within a specified directory. From 2.0.0 through 2.63.1, the hook system in File Browser — which executes administrator-defined shell commands on file events such as upload, rename, and delete — is vulnerable to OS command injection. Variable substitution for values like $FILE and $USERNAME is performed via os.Expand without sanitization. An attacker with file write permission can craft a malicious filename containing shell metacharacters, causing the server to execute arbitrary OS commands when the hook fires. This results in Remote Code Execution (RCE). This feature has been disabled by default for all installations from v2.33.8 onwards, including for existent installations.

- [https://github.com/Saku0512/CVE-2026-35585-poc](https://github.com/Saku0512/CVE-2026-35585-poc) :  ![starts](https://img.shields.io/github/stars/Saku0512/CVE-2026-35585-poc.svg) ![forks](https://img.shields.io/github/forks/Saku0512/CVE-2026-35585-poc.svg)


## CVE-2026-35584
 FreeScout is a free help desk and shared inbox built with PHP's Laravel framework. Prior to 1.8.212, the endpoint GET /thread/read/{conversation_id}/{thread_id} does not require authentication and does not validate whether the given thread_id belongs to the given conversation_id. This allows any unauthenticated attacker to mark any thread as read by passing arbitrary IDs, enumerate valid thread IDs via HTTP response codes (200 vs 404), and manipulate opened_at timestamps across conversations (IDOR). This vulnerability is fixed in 1.8.212.

- [https://github.com/spoo1k/CVE-2026-35584](https://github.com/spoo1k/CVE-2026-35584) :  ![starts](https://img.shields.io/github/stars/spoo1k/CVE-2026-35584.svg) ![forks](https://img.shields.io/github/forks/spoo1k/CVE-2026-35584.svg)


## CVE-2026-35517
 FTLDNS (pihole-FTL) provides an interactive API and also generates statistics for Pi-hole's Web interface. From 6.0 to before 6.6, the Pi-hole FTL engine contains a Remote Code Execution (RCE) vulnerability in the upstream DNS servers configuration parameter (dns.upstreams). This vulnerability allows an authenticated attacker to inject arbitrary dnsmasq configuration directives through newline characters, ultimately achieving command execution on the underlying system. This vulnerability is fixed in 6.6.

- [https://github.com/keraattin/CVE-2026-35517](https://github.com/keraattin/CVE-2026-35517) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-35517.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-35517.svg)


## CVE-2026-34621
 Acrobat Reader versions 24.001.30356, 26.001.21367 and earlier are affected by an Improperly Controlled Modification of Object Prototype Attributes ('Prototype Pollution') vulnerability that could result in arbitrary code execution in the context of the current user. Exploitation of this issue requires user interaction in that a victim must open a malicious file.

- [https://github.com/KeulenR01/Remediate-AdobeAcrobat-CVE-2026-34621](https://github.com/KeulenR01/Remediate-AdobeAcrobat-CVE-2026-34621) :  ![starts](https://img.shields.io/github/stars/KeulenR01/Remediate-AdobeAcrobat-CVE-2026-34621.svg) ![forks](https://img.shields.io/github/forks/KeulenR01/Remediate-AdobeAcrobat-CVE-2026-34621.svg)


## CVE-2026-34197
Users are recommended to upgrade to version 5.19.4 or 6.2.3, which fixes the issue

- [https://github.com/keraattin/CVE-2026-34197](https://github.com/keraattin/CVE-2026-34197) :  ![starts](https://img.shields.io/github/stars/keraattin/CVE-2026-34197.svg) ![forks](https://img.shields.io/github/forks/keraattin/CVE-2026-34197.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/Spydomain/CVE-2026-33017-langflow-lab](https://github.com/Spydomain/CVE-2026-33017-langflow-lab) :  ![starts](https://img.shields.io/github/stars/Spydomain/CVE-2026-33017-langflow-lab.svg) ![forks](https://img.shields.io/github/forks/Spydomain/CVE-2026-33017-langflow-lab.svg)


## CVE-2026-30480
 A Local File Inclusion (LFI) vulnerability in the NFSen module (nfsen.inc.php) of LibreNMS 22.11.0-23-gd091788f2 allows authenticated attackers to include arbitrary PHP files from the server filesystem via path traversal sequences in the nfsen parameter.

- [https://github.com/parlakbarann/CVE-2026-30480](https://github.com/parlakbarann/CVE-2026-30480) :  ![starts](https://img.shields.io/github/stars/parlakbarann/CVE-2026-30480.svg) ![forks](https://img.shields.io/github/forks/parlakbarann/CVE-2026-30480.svg)


## CVE-2026-22692
 October is a Content Management System (CMS) and web platform. Versions prior to 3.7.13 and versions 4.0.0 through 4.1.4 contain a sandbox bypass vulnerability in the optional Twig safe mode feature (CMS_SAFE_MODE). Certain methods on the collect() helper were not properly restricted, allowing authenticated users with template editing permissions to bypass sandbox protections. Exploitation requires authenticated backend access with CMS template editing permissions and only affects installations with CMS_SAFE_MODE enabled (disabled by default). This issue has been fixed in versions 3.7.13 and 4.1.5. To workaround this issue, users can disable CMS_SAFE_MODE if untrusted template editing is not required, and restrict CMS template editing permissions to fully trusted administrators only.

- [https://github.com/lukasz-rybak/CVE-2026-22692](https://github.com/lukasz-rybak/CVE-2026-22692) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-22692.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-22692.svg)


## CVE-2026-6227
 The BackWPup plugin for WordPress is vulnerable to Local File Inclusion via the `block_name` parameter of the `/wp-json/backwpup/v1/getblock` REST endpoint in all versions up to, and including, 5.6.6 due to a non-recursive `str_replace()` sanitization of path traversal sequences. This makes it possible for authenticated attackers, with Administrator-level access and above, to include arbitrary PHP files on the server via crafted traversal sequences (e.g., `....//`), which can be leveraged to read sensitive files such as `wp-config.php` or achieve remote code execution in certain configurations. Administrators have the ability to grant individual users permission to handle backups, which may then allow lower-level users to exploit this vulnerability.

- [https://github.com/Pixel-DefaultBR/CVE-2026-6227](https://github.com/Pixel-DefaultBR/CVE-2026-6227) :  ![starts](https://img.shields.io/github/stars/Pixel-DefaultBR/CVE-2026-6227.svg) ![forks](https://img.shields.io/github/forks/Pixel-DefaultBR/CVE-2026-6227.svg)


## CVE-2026-6042
 A security flaw has been discovered in musl libc up to 1.2.6. Affected is the function iconv of the file src/locale/iconv.c of the component GB18030 4-byte Decoder. Performing a manipulation results in inefficient algorithmic complexity. The attack must be initiated from a local position. To fix this issue, it is recommended to deploy a patch.

- [https://github.com/jensnesten/CVE-2026-6042-PoC](https://github.com/jensnesten/CVE-2026-6042-PoC) :  ![starts](https://img.shields.io/github/stars/jensnesten/CVE-2026-6042-PoC.svg) ![forks](https://img.shields.io/github/forks/jensnesten/CVE-2026-6042-PoC.svg)


## CVE-2025-69993
 Leaflet versions up to and including 1.9.4 are vulnerable to Cross-Site Scripting (XSS) via the bindPopup() method. This method renders user-supplied input as raw HTML without sanitization, allowing attackers to inject arbitrary JavaScript code through event handler attributes (e.g., img src=x onerror="alert('XSS')"). When a victim views an affected map popup, the malicious script executes in the context of the victim's browser session.

- [https://github.com/PierfrancescoConti/leaflet-cve-2025-69993](https://github.com/PierfrancescoConti/leaflet-cve-2025-69993) :  ![starts](https://img.shields.io/github/stars/PierfrancescoConti/leaflet-cve-2025-69993.svg) ![forks](https://img.shields.io/github/forks/PierfrancescoConti/leaflet-cve-2025-69993.svg)


## CVE-2025-68613
 n8n is an open source workflow automation platform. Versions starting with 0.211.0 and prior to 1.120.4, 1.121.1, and 1.122.0 contain a critical Remote Code Execution (RCE) vulnerability in their workflow expression evaluation system. Under certain conditions, expressions supplied by authenticated users during workflow configuration may be evaluated in an execution context that is not sufficiently isolated from the underlying runtime. An authenticated attacker could abuse this behavior to execute arbitrary code with the privileges of the n8n process. Successful exploitation may lead to full compromise of the affected instance, including unauthorized access to sensitive data, modification of workflows, and execution of system-level operations. This issue has been fixed in versions 1.120.4, 1.121.1, and 1.122.0. Users are strongly advised to upgrade to a patched version, which introduces additional safeguards to restrict expression evaluation. If upgrading is not immediately possible, administrators should consider the following temporary mitigations: Limit workflow creation and editing permissions to fully trusted users only; and/or deploy n8n in a hardened environment with restricted operating system privileges and network access to reduce the impact of potential exploitation. These workarounds do not fully eliminate the risk and should only be used as short-term measures.

- [https://github.com/canpilayda/n8n-RCE-CVE-2025-68613](https://github.com/canpilayda/n8n-RCE-CVE-2025-68613) :  ![starts](https://img.shields.io/github/stars/canpilayda/n8n-RCE-CVE-2025-68613.svg) ![forks](https://img.shields.io/github/forks/canpilayda/n8n-RCE-CVE-2025-68613.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/ahmed-dev-op/CVE-2025-55182](https://github.com/ahmed-dev-op/CVE-2025-55182) :  ![starts](https://img.shields.io/github/stars/ahmed-dev-op/CVE-2025-55182.svg) ![forks](https://img.shields.io/github/forks/ahmed-dev-op/CVE-2025-55182.svg)


## CVE-2025-59528
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5, Flowise is vulnerable to remote code execution. The CustomMCP node allows users to input configuration settings for connecting to an external MCP server. This node parses the user-provided mcpServerConfig string to build the MCP server configuration. However, during this process, it executes JavaScript code without any security validation. Specifically, inside the convertToValidJSONString function, user input is directly passed to the Function() constructor, which evaluates and executes the input as JavaScript code. Since this runs with full Node.js runtime privileges, it can access dangerous modules such as child_process and fs. This issue has been patched in version 3.0.6.

- [https://github.com/CVETeam/FlowiseAI-Critical-KillChain](https://github.com/CVETeam/FlowiseAI-Critical-KillChain) :  ![starts](https://img.shields.io/github/stars/CVETeam/FlowiseAI-Critical-KillChain.svg) ![forks](https://img.shields.io/github/forks/CVETeam/FlowiseAI-Critical-KillChain.svg)


## CVE-2025-58434
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5 and earlier, the `forgot-password` endpoint in Flowise returns sensitive information including a valid password reset `tempToken` without authentication or verification. This enables any attacker to generate a reset token for arbitrary users and directly reset their password, leading to a complete account takeover (ATO). This vulnerability applies to both the cloud service (`cloud.flowiseai.com`) and self-hosted/local Flowise deployments that expose the same API. Commit 9e178d68873eb876073846433a596590d3d9c863 in version 3.0.6 secures password reset endpoints. Several recommended remediation steps are available. Do not return reset tokens or sensitive account details in API responses. Tokens must only be delivered securely via the registered email channel. Ensure `forgot-password` responds with a generic success message regardless of input, to avoid user enumeration. Require strong validation of the `tempToken` (e.g., single-use, short expiry, tied to request origin, validated against email delivery). Apply the same fixes to both cloud and self-hosted/local deployments. Log and monitor password reset requests for suspicious activity. Consider multi-factor verification for sensitive accounts.

- [https://github.com/CVETeam/FlowiseAI-Critical-KillChain](https://github.com/CVETeam/FlowiseAI-Critical-KillChain) :  ![starts](https://img.shields.io/github/stars/CVETeam/FlowiseAI-Critical-KillChain.svg) ![forks](https://img.shields.io/github/forks/CVETeam/FlowiseAI-Critical-KillChain.svg)


## CVE-2025-50565
 Doubo ERP 1.0 has an SQL injection vulnerability due to a lack of filtering of user input, which can be remotely initiated by an attacker.

- [https://github.com/m0b1u3/CVE-2025-50565](https://github.com/m0b1u3/CVE-2025-50565) :  ![starts](https://img.shields.io/github/stars/m0b1u3/CVE-2025-50565.svg) ![forks](https://img.shields.io/github/forks/m0b1u3/CVE-2025-50565.svg)


## CVE-2025-48561
 In multiple locations, there is a possible way to access data displayed on the screen due to side channel information disclosure. This could lead to local information disclosure with no additional execution privileges needed. User interaction is not needed for exploitation.

- [https://github.com/thanhvan205/Pixnapping-Key-Exfiltration](https://github.com/thanhvan205/Pixnapping-Key-Exfiltration) :  ![starts](https://img.shields.io/github/stars/thanhvan205/Pixnapping-Key-Exfiltration.svg) ![forks](https://img.shields.io/github/forks/thanhvan205/Pixnapping-Key-Exfiltration.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927](https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/sn1p3rt3s7/NextJS_CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/sn1p3rt3s7/NextJS_CVE-2025-29927.svg)


## CVE-2025-24000
 Authentication Bypass Using an Alternate Path or Channel vulnerability in Saad Iqbal Post SMTP post-smtp allows Authentication Bypass.This issue affects Post SMTP: from n/a through = 3.2.0.

- [https://github.com/bsdrip/CVE-2025-24000-exploit](https://github.com/bsdrip/CVE-2025-24000-exploit) :  ![starts](https://img.shields.io/github/stars/bsdrip/CVE-2025-24000-exploit.svg) ![forks](https://img.shields.io/github/forks/bsdrip/CVE-2025-24000-exploit.svg)


## CVE-2025-13595
 The CIBELES AI plugin for WordPress is vulnerable to arbitrary file uploads due to missing capability check in the 'actualizador_git.php' file in all versions up to, and including, 1.10.8. This makes it possible for unauthenticated attackers to download arbitrary GitHub repositories and overwrite plugin files on the affected site's server which may make remote code execution possible.

- [https://github.com/d0n601/CVE-2025-13595](https://github.com/d0n601/CVE-2025-13595) :  ![starts](https://img.shields.io/github/stars/d0n601/CVE-2025-13595.svg) ![forks](https://img.shields.io/github/forks/d0n601/CVE-2025-13595.svg)


## CVE-2025-13159
 The Flo Forms – Easy Drag & Drop Form Builder plugin for WordPress is vulnerable to Stored Cross-Site Scripting via SVG file uploads in all versions up to, and including, 1.0.43. This is due to the plugin allowing SVG file uploads via an unauthenticated AJAX endpoint (`flo_form_submit`) without proper file content validation. This makes it possible for unauthenticated attackers to upload malicious SVG files containing JavaScript that executes when an administrator views the uploaded file in the WordPress admin interface, leading to potential full site compromise.

- [https://github.com/MooseLoveti/Flo-Forms-CVE-Report](https://github.com/MooseLoveti/Flo-Forms-CVE-Report) :  ![starts](https://img.shields.io/github/stars/MooseLoveti/Flo-Forms-CVE-Report.svg) ![forks](https://img.shields.io/github/forks/MooseLoveti/Flo-Forms-CVE-Report.svg)


## CVE-2025-8110
 Improper Symbolic link handling in the PutContents API in Gogs allows Local Execution of Code.

- [https://github.com/NetsecBandit/CVE-2025-8110-Exploit](https://github.com/NetsecBandit/CVE-2025-8110-Exploit) :  ![starts](https://img.shields.io/github/stars/NetsecBandit/CVE-2025-8110-Exploit.svg) ![forks](https://img.shields.io/github/forks/NetsecBandit/CVE-2025-8110-Exploit.svg)


## CVE-2024-25381
 There is a Stored XSS Vulnerability in Emlog Pro 2.2.8 Article Publishing, due to non-filtering of quoted content.

- [https://github.com/m0b1u3/CVE-2024-25381](https://github.com/m0b1u3/CVE-2024-25381) :  ![starts](https://img.shields.io/github/stars/m0b1u3/CVE-2024-25381.svg) ![forks](https://img.shields.io/github/forks/m0b1u3/CVE-2024-25381.svg)


## CVE-2024-21413
 Microsoft Outlook Remote Code Execution Vulnerability

- [https://github.com/FathanahHidayati/https-github.com-xaitax-CVE-2024-21413-Microsoft-Outlook-Remote-Code-Execution-Vulnerability](https://github.com/FathanahHidayati/https-github.com-xaitax-CVE-2024-21413-Microsoft-Outlook-Remote-Code-Execution-Vulnerability) :  ![starts](https://img.shields.io/github/stars/FathanahHidayati/https-github.com-xaitax-CVE-2024-21413-Microsoft-Outlook-Remote-Code-Execution-Vulnerability.svg) ![forks](https://img.shields.io/github/forks/FathanahHidayati/https-github.com-xaitax-CVE-2024-21413-Microsoft-Outlook-Remote-Code-Execution-Vulnerability.svg)


## CVE-2021-22986
 On BIG-IP versions 16.0.x before 16.0.1.1, 15.1.x before 15.1.2.1, 14.1.x before 14.1.4, 13.1.x before 13.1.3.6, and 12.1.x before 12.1.5.3 amd BIG-IQ 7.1.0.x before 7.1.0.3 and 7.0.0.x before 7.0.0.2, the iControl REST interface has an unauthenticated remote command execution vulnerability. Note: Software versions which have reached End of Software Development (EoSD) are not evaluated.

- [https://github.com/whatheheckisthis/Canonical-Extension-CVE-2021-22986](https://github.com/whatheheckisthis/Canonical-Extension-CVE-2021-22986) :  ![starts](https://img.shields.io/github/stars/whatheheckisthis/Canonical-Extension-CVE-2021-22986.svg) ![forks](https://img.shields.io/github/forks/whatheheckisthis/Canonical-Extension-CVE-2021-22986.svg)


## CVE-2020-9715
 Adobe Acrobat and Reader versions 2020.009.20074 and earlier, 2020.001.30002, 2017.011.30171 and earlier, and 2015.006.30523 and earlier have an use-after-free vulnerability. Successful exploitation could lead to arbitrary code execution .

- [https://github.com/f8al/PoC-CVE-2020-9715](https://github.com/f8al/PoC-CVE-2020-9715) :  ![starts](https://img.shields.io/github/stars/f8al/PoC-CVE-2020-9715.svg) ![forks](https://img.shields.io/github/forks/f8al/PoC-CVE-2020-9715.svg)


## CVE-2020-3580
 Multiple vulnerabilities in the web services interface of Cisco Adaptive Security Appliance (ASA) Software and Cisco Firepower Threat Defense (FTD) Software could allow an unauthenticated, remote attacker to conduct cross-site scripting (XSS) attacks against a user of the web services interface of an affected device. The vulnerabilities are due to insufficient validation of user-supplied input by the web services interface of an affected device. An attacker could exploit these vulnerabilities by persuading a user of the interface to click a crafted link. A successful exploit could allow the attacker to execute arbitrary script code in the context of the interface or allow the attacker to access sensitive, browser-based information. Note: These vulnerabilities affect only specific AnyConnect and WebVPN configurations. For more information, see the Vulnerable Products section.

- [https://github.com/brittle-finance685/XSS-HUNTER](https://github.com/brittle-finance685/XSS-HUNTER) :  ![starts](https://img.shields.io/github/stars/brittle-finance685/XSS-HUNTER.svg) ![forks](https://img.shields.io/github/forks/brittle-finance685/XSS-HUNTER.svg)


## CVE-2019-15707
 An improper access control vulnerability in FortiMail admin webUI 6.2.0, 6.0.0 to 6.0.6, 5.4.10 and below may allow administrators to perform system backup config download they should not be authorized for.

- [https://github.com/cristianovisk/CVE-2019-15707](https://github.com/cristianovisk/CVE-2019-15707) :  ![starts](https://img.shields.io/github/stars/cristianovisk/CVE-2019-15707.svg) ![forks](https://img.shields.io/github/forks/cristianovisk/CVE-2019-15707.svg)


## CVE-2019-1951
 A vulnerability in the packet filtering features of Cisco SD-WAN Solution could allow an unauthenticated, remote attacker to bypass L3 and L4 traffic filters. The vulnerability is due to improper traffic filtering conditions on an affected device. An attacker could exploit this vulnerability by crafting a malicious TCP packet with specific characteristics and sending it to a target device. A successful exploit could allow the attacker to bypass the L3 and L4 traffic filters and inject an arbitrary packet in the network.

- [https://github.com/jra89/CVE-2019-19511](https://github.com/jra89/CVE-2019-19511) :  ![starts](https://img.shields.io/github/stars/jra89/CVE-2019-19511.svg) ![forks](https://img.shields.io/github/forks/jra89/CVE-2019-19511.svg)


## CVE-2018-1288
 In Apache Kafka 0.9.0.0 to 0.9.0.1, 0.10.0.0 to 0.10.2.1, 0.11.0.0 to 0.11.0.2, and 1.0.0, authenticated Kafka users may perform action reserved for the Broker via a manually created fetch request interfering with data replication, resulting in data loss.

- [https://github.com/joegallagher4/CVE-2018-1288-](https://github.com/joegallagher4/CVE-2018-1288-) :  ![starts](https://img.shields.io/github/stars/joegallagher4/CVE-2018-1288-.svg) ![forks](https://img.shields.io/github/forks/joegallagher4/CVE-2018-1288-.svg)


## CVE-2018-1099
 DNS rebinding vulnerability found in etcd 3.3.1 and earlier. An attacker can control his DNS records to direct to localhost, and trick the browser into sending requests to localhost (or any other address).

- [https://github.com/nicolastsk/cve-2018-10993](https://github.com/nicolastsk/cve-2018-10993) :  ![starts](https://img.shields.io/github/stars/nicolastsk/cve-2018-10993.svg) ![forks](https://img.shields.io/github/forks/nicolastsk/cve-2018-10993.svg)


## CVE-2008-2992
 Stack-based buffer overflow in Adobe Acrobat and Reader 8.1.2 and earlier allows remote attackers to execute arbitrary code via a PDF file that calls the util.printf JavaScript function with a crafted format string argument, a related issue to CVE-2008-1104.

- [https://github.com/Jonas-Holmberg/CVE-2008-2992](https://github.com/Jonas-Holmberg/CVE-2008-2992) :  ![starts](https://img.shields.io/github/stars/Jonas-Holmberg/CVE-2008-2992.svg) ![forks](https://img.shields.io/github/forks/Jonas-Holmberg/CVE-2008-2992.svg)

