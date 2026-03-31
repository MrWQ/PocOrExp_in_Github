# Update 2026-03-31
## CVE-2026-34005
 In Sofia on Xiongmai DVR/NVR (AHB7008T-MH-V2 and NBD7024H-P) 4.03.R11 devices, root OS command injection can occur via shell metacharacters in the HostName value via an authenticated DVRIP protocol (TCP port 34567) request to the NetWork.NetCommon configuration handler, because system() is used.

- [https://github.com/uky007/CVE-2026-34005](https://github.com/uky007/CVE-2026-34005) :  ![starts](https://img.shields.io/github/stars/uky007/CVE-2026-34005.svg) ![forks](https://img.shields.io/github/forks/uky007/CVE-2026-34005.svg)


## CVE-2026-33634
 Trivy is a security scanner. On March 19, 2026, a threat actor used compromised credentials to publish a malicious Trivy v0.69.4 release, force-push 76 of 77 version tags in `aquasecurity/trivy-action` to credential-stealing malware, and replace all 7 tags in `aquasecurity/setup-trivy` with malicious commits. This incident is a continuation of the supply chain attack that began in late February 2026. Following the initial disclosure on March 1, credential rotation was performed but was not atomic (not all credentials were revoked simultaneously). The attacker could have use a valid token to exfiltrate newly rotated secrets during the rotation window (which lasted a few days). This could have allowed the attacker to retain access and execute the March 19 attack. Affected components include the `aquasecurity/trivy` Go / Container image version 0.69.4, the `aquasecurity/trivy-action` GitHub Action versions 0.0.1 – 0.34.2 (76/77), and the`aquasecurity/setup-trivy` GitHub Action versions 0.2.0 – 0.2.6, prior to the recreation of 0.2.6 with a safe commit. Known safe versions include versions 0.69.2 and 0.69.3 of the Trivy binary, version 0.35.0 of trivy-action, and version 0.2.6 of setup-trivy. Additionally, take other mitigations to ensure the safety of secrets. If there is any possibility that a compromised version ran in one's environment, all secrets accessible to affected pipelines must be treated as exposed and rotated immediately. Check whether one's organization pulled or executed Trivy v0.69.4 from any source. Remove any affected artifacts immediately. Review all workflows using `aquasecurity/trivy-action` or `aquasecurity/setup-trivy`. Those who referenced a version tag rather than a full commit SHA should check workflow run logs from March 19–20, 2026 for signs of compromise. Look for repositories named `tpcp-docs` in one's GitHub organization. The presence of such a repository may indicate that the fallback exfiltration mechanism was triggered and secrets were successfully stolen. Pin GitHub Actions to full, immutable commit SHA hashes, don't use mutable version tags.

- [https://github.com/Unit221B/teampcp-tools](https://github.com/Unit221B/teampcp-tools) :  ![starts](https://img.shields.io/github/stars/Unit221B/teampcp-tools.svg) ![forks](https://img.shields.io/github/forks/Unit221B/teampcp-tools.svg)


## CVE-2026-33340
 LoLLMs WEBUI provides the Web user interface for Lord of Large Language and Multi modal Systems. A critical Server-Side Request Forgery (SSRF) vulnerability has been identified in all known existing versions of `lollms-webui`. The `@router.post("/api/proxy")` endpoint allows unauthenticated attackers to force the server into making arbitrary GET requests. This can be exploited to access internal services, scan local networks, or exfiltrate sensitive cloud metadata (e.g., AWS/GCP IAM tokens). As of time of publication, no known patched versions are available.

- [https://github.com/regaan/CVE-2026-33340](https://github.com/regaan/CVE-2026-33340) :  ![starts](https://img.shields.io/github/stars/regaan/CVE-2026-33340.svg) ![forks](https://img.shields.io/github/forks/regaan/CVE-2026-33340.svg)


## CVE-2026-32015
 OpenClaw versions 2026.1.21 prior to 2026.2.19 contain a path hijacking vulnerability in tools.exec.safeBins that allows attackers to bypass allowlist checks by controlling process PATH resolution. Attackers who can influence the gateway process PATH or launch environment can execute trojan binaries with allowlisted names, such as jq, circumventing executable validation controls.

- [https://github.com/hargabyte/cve-scanner](https://github.com/hargabyte/cve-scanner) :  ![starts](https://img.shields.io/github/stars/hargabyte/cve-scanner.svg) ![forks](https://img.shields.io/github/forks/hargabyte/cve-scanner.svg)


## CVE-2026-32013
 OpenClaw versions prior to 2026.2.25 contain a symlink traversal vulnerability in the agents.files.get and agents.files.set methods that allows reading and writing files outside the agent workspace. Attackers can exploit symlinked allowlisted files to access arbitrary host files within gateway process permissions, potentially enabling code execution through file overwrite attacks.

- [https://github.com/hargabyte/cve-scanner](https://github.com/hargabyte/cve-scanner) :  ![starts](https://img.shields.io/github/stars/hargabyte/cve-scanner.svg) ![forks](https://img.shields.io/github/forks/hargabyte/cve-scanner.svg)


## CVE-2026-26980
 Ghost is a Node.js content management system. Versions 3.24.0 through 6.19.0 allow unauthenticated attackers to perform arbitrary reads from the database. This issue has been fixed in version 6.19.1.

- [https://github.com/vognik/CVE-2026-26980](https://github.com/vognik/CVE-2026-26980) :  ![starts](https://img.shields.io/github/stars/vognik/CVE-2026-26980.svg) ![forks](https://img.shields.io/github/forks/vognik/CVE-2026-26980.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/CyLock11/CVE-2026-23744](https://github.com/CyLock11/CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/CyLock11/CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/CyLock11/CVE-2026-23744.svg)
- [https://github.com/z4yd3/PoC-CVE-2026-23744](https://github.com/z4yd3/PoC-CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/z4yd3/PoC-CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/z4yd3/PoC-CVE-2026-23744.svg)


## CVE-2026-22813
 OpenCode is an open source AI coding agent. The markdown renderer used for LLM responses will insert arbitrary HTML into the DOM. There is no sanitization with DOMPurify or even a CSP on the web interface to prevent JavaScript execution via HTML injection. This means controlling the LLM response for a chat session gets JavaScript execution on the http://localhost:4096 origin. This vulnerability is fixed in 1.1.10.

- [https://github.com/HodgeLuke/ai-agent-security-research](https://github.com/HodgeLuke/ai-agent-security-research) :  ![starts](https://img.shields.io/github/stars/HodgeLuke/ai-agent-security-research.svg) ![forks](https://img.shields.io/github/forks/HodgeLuke/ai-agent-security-research.svg)


## CVE-2026-22812
 OpenCode is an open source AI coding agent. Prior to 1.0.216, OpenCode automatically starts an unauthenticated HTTP server that allows any local process (or any website via permissive CORS) to execute arbitrary shell commands with the user's privileges. This vulnerability is fixed in 1.0.216.

- [https://github.com/HodgeLuke/ai-agent-security-research](https://github.com/HodgeLuke/ai-agent-security-research) :  ![starts](https://img.shields.io/github/stars/HodgeLuke/ai-agent-security-research.svg) ![forks](https://img.shields.io/github/forks/HodgeLuke/ai-agent-security-research.svg)


## CVE-2026-3055
 Insufficient input validation in NetScaler ADC and NetScaler Gateway when configured as a SAML IDP leading to memory overread

- [https://github.com/0xBlackash/CVE-2026-3055](https://github.com/0xBlackash/CVE-2026-3055) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-3055.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-3055.svg)


## CVE-2026-0897
 Allocation of Resources Without Limits or Throttling in the HDF5 weight loading component in Google Keras 3.0.0 through 3.13.0 on all platforms allows a remote attacker to cause a Denial of Service (DoS) through memory exhaustion and a crash of the Python interpreter via a crafted .keras archive containing a valid model.weights.h5 file whose dataset declares an extremely large shape.

- [https://github.com/HyperPS/CVE-2026-0897](https://github.com/HyperPS/CVE-2026-0897) :  ![starts](https://img.shields.io/github/stars/HyperPS/CVE-2026-0897.svg) ![forks](https://img.shields.io/github/forks/HyperPS/CVE-2026-0897.svg)


## CVE-2026-0848
 NLTK versions =3.9.2 are vulnerable to arbitrary code execution due to improper input validation in the StanfordSegmenter module. The module dynamically loads external Java .jar files without verification or sandboxing. An attacker can supply or replace the JAR file, enabling the execution of arbitrary Java bytecode at import time. This vulnerability can be exploited through methods such as model poisoning, MITM attacks, or dependency poisoning, leading to remote code execution. The issue arises from the direct execution of the JAR file via subprocess with unvalidated classpath input, allowing malicious classes to execute when loaded by the JVM.

- [https://github.com/HyperPS/CVE-2026-0848](https://github.com/HyperPS/CVE-2026-0848) :  ![starts](https://img.shields.io/github/stars/HyperPS/CVE-2026-0848.svg) ![forks](https://img.shields.io/github/forks/HyperPS/CVE-2026-0848.svg)


## CVE-2026-0847
 A vulnerability in NLTK versions up to and including 3.9.2 allows arbitrary file read via path traversal in multiple CorpusReader classes, including WordListCorpusReader, TaggedCorpusReader, and BracketParseCorpusReader. These classes fail to properly sanitize or validate file paths, enabling attackers to traverse directories and access sensitive files on the server. This issue is particularly critical in scenarios where user-controlled file inputs are processed, such as in machine learning APIs, chatbots, or NLP pipelines. Exploitation of this vulnerability can lead to unauthorized access to sensitive files, including system files, SSH private keys, and API tokens, and may potentially escalate to remote code execution when combined with other vulnerabilities.

- [https://github.com/HyperPS/CVE-2026-0847](https://github.com/HyperPS/CVE-2026-0847) :  ![starts](https://img.shields.io/github/stars/HyperPS/CVE-2026-0847.svg) ![forks](https://img.shields.io/github/forks/HyperPS/CVE-2026-0847.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)


## CVE-2025-61246
 indieka900 online-shopping-system-php 1.0 is vulnerable to SQL Injection in master/review_action.php via the proId parameter.

- [https://github.com/hackergovind/CVE-2025-61246](https://github.com/hackergovind/CVE-2025-61246) :  ![starts](https://img.shields.io/github/stars/hackergovind/CVE-2025-61246.svg) ![forks](https://img.shields.io/github/forks/hackergovind/CVE-2025-61246.svg)


## CVE-2025-60709
 Out-of-bounds read in Windows Common Log File System Driver allows an authorized attacker to elevate privileges locally.

- [https://github.com/ByteCodeSecure/CVE-2025-60709](https://github.com/ByteCodeSecure/CVE-2025-60709) :  ![starts](https://img.shields.io/github/stars/ByteCodeSecure/CVE-2025-60709.svg) ![forks](https://img.shields.io/github/forks/ByteCodeSecure/CVE-2025-60709.svg)


## CVE-2025-55182
 A pre-authentication remote code execution vulnerability exists in React Server Components versions 19.0.0, 19.1.0, 19.1.1, and 19.2.0 including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints.

- [https://github.com/Rat5ak/CVE-2025-55182-React2Shell-RCE-POC](https://github.com/Rat5ak/CVE-2025-55182-React2Shell-RCE-POC) :  ![starts](https://img.shields.io/github/stars/Rat5ak/CVE-2025-55182-React2Shell-RCE-POC.svg) ![forks](https://img.shields.io/github/forks/Rat5ak/CVE-2025-55182-React2Shell-RCE-POC.svg)


## CVE-2025-54123
 Hoverfly is an open source API simulation tool. In versions 1.11.3 and prior, the middleware functionality in Hoverfly is vulnerable to command injection vulnerability at `/api/v2/hoverfly/middleware` endpoint due to insufficient validation and sanitization in user input. The vulnerability exists in the middleware management API endpoint `/api/v2/hoverfly/middleware`. This issue is born due to combination of three code level flaws: Insufficient Input Validation in middleware.go line 94-96; Unsafe Command Execution in local_middleware.go line 14-19; and Immediate Execution During Testing in hoverfly_service.go line 173. This allows an attacker to gain remote code execution (RCE) on any system running the vulnerable Hoverfly service. Since the input is directly passed to system commands without proper checks, an attacker can upload a malicious payload or directly execute arbitrary commands (including reverse shells) on the host server with the privileges of the Hoverfly process. Commit 17e60a9bc78826deb4b782dca1c1abd3dbe60d40 in version 1.12.0 disables the set middleware API by default, and subsequent changes to documentation make users aware of the security changes of exposing the set middleware API.

- [https://github.com/tristanqtn/CVE-2025-54123](https://github.com/tristanqtn/CVE-2025-54123) :  ![starts](https://img.shields.io/github/stars/tristanqtn/CVE-2025-54123.svg) ![forks](https://img.shields.io/github/forks/tristanqtn/CVE-2025-54123.svg)


## CVE-2025-23419
Note: Software versions which have reached End of Technical Support (EoTS) are not evaluated.

- [https://github.com/xitexploiter96-dot/CVE-2025-23419](https://github.com/xitexploiter96-dot/CVE-2025-23419) :  ![starts](https://img.shields.io/github/stars/xitexploiter96-dot/CVE-2025-23419.svg) ![forks](https://img.shields.io/github/forks/xitexploiter96-dot/CVE-2025-23419.svg)


## CVE-2025-23209
 Craft is a flexible, user-friendly CMS for creating custom digital experiences on the web and beyond. This is an remote code execution (RCE) vulnerability that affects Craft 4 and 5 installs where your security key has already been compromised. Anyone running an unpatched version of Craft with a compromised security key is affected. This vulnerability has been patched in Craft 5.5.8 and 4.13.8. Users who cannot update to a patched version, should rotate their security keys and ensure their privacy to help migitgate the issue.

- [https://github.com/farid-khelil/CVE_2025_23209](https://github.com/farid-khelil/CVE_2025_23209) :  ![starts](https://img.shields.io/github/stars/farid-khelil/CVE_2025_23209.svg) ![forks](https://img.shields.io/github/forks/farid-khelil/CVE_2025_23209.svg)


## CVE-2024-27348
Users are recommended to upgrade to version 1.3.0 with Java11 & enable the Auth system, which fixes the issue.

- [https://github.com/akelaqe/CVE-2024-27348-HugeGraph-RCE](https://github.com/akelaqe/CVE-2024-27348-HugeGraph-RCE) :  ![starts](https://img.shields.io/github/stars/akelaqe/CVE-2024-27348-HugeGraph-RCE.svg) ![forks](https://img.shields.io/github/forks/akelaqe/CVE-2024-27348-HugeGraph-RCE.svg)


## CVE-2024-6387
 A security regression (CVE-2006-5051) was discovered in OpenSSH's server (sshd). There is a race condition which can lead sshd to handle some signals in an unsafe manner. An unauthenticated, remote attacker may be able to trigger it by failing to authenticate within a set time period.

- [https://github.com/Doux-x/CVE-2024-6387-analysis](https://github.com/Doux-x/CVE-2024-6387-analysis) :  ![starts](https://img.shields.io/github/stars/Doux-x/CVE-2024-6387-analysis.svg) ![forks](https://img.shields.io/github/forks/Doux-x/CVE-2024-6387-analysis.svg)


## CVE-2024-3273
 ** UNSUPPORTED WHEN ASSIGNED ** A vulnerability, which was classified as critical, was found in D-Link DNS-320L, DNS-325, DNS-327L and DNS-340L up to 20240403. Affected is an unknown function of the file /cgi-bin/nas_sharing.cgi of the component HTTP GET Request Handler. The manipulation of the argument system leads to command injection. It is possible to launch the attack remotely. The exploit has been disclosed to the public and may be used. The identifier of this vulnerability is VDB-259284. NOTE: This vulnerability only affects products that are no longer supported by the maintainer. NOTE: Vendor was contacted early and confirmed immediately that the product is end-of-life. It should be retired and replaced.

- [https://github.com/JollyPropoganda/CVE_2024_3273_adv_shell_script](https://github.com/JollyPropoganda/CVE_2024_3273_adv_shell_script) :  ![starts](https://img.shields.io/github/stars/JollyPropoganda/CVE_2024_3273_adv_shell_script.svg) ![forks](https://img.shields.io/github/forks/JollyPropoganda/CVE_2024_3273_adv_shell_script.svg)


## CVE-2022-42889
 Apache Commons Text performs variable interpolation, allowing properties to be dynamically evaluated and expanded. The standard format for interpolation is "${prefix:name}", where "prefix" is used to locate an instance of org.apache.commons.text.lookup.StringLookup that performs the interpolation. Starting with version 1.5 and continuing through 1.9, the set of default Lookup instances included interpolators that could result in arbitrary code execution or contact with remote servers. These lookups are: - "script" - execute expressions using the JVM script execution engine (javax.script) - "dns" - resolve dns records - "url" - load values from urls, including from remote servers Applications using the interpolation defaults in the affected versions may be vulnerable to remote code execution or unintentional contact with remote servers if untrusted configuration values are used. Users are recommended to upgrade to Apache Commons Text 1.10.0, which disables the problematic interpolators by default.

- [https://github.com/KosmicOwl045/ICT287-CVE-2022-42889](https://github.com/KosmicOwl045/ICT287-CVE-2022-42889) :  ![starts](https://img.shields.io/github/stars/KosmicOwl045/ICT287-CVE-2022-42889.svg) ![forks](https://img.shields.io/github/forks/KosmicOwl045/ICT287-CVE-2022-42889.svg)


## CVE-2021-21192
 Heap buffer overflow in tab groups in Google Chrome prior to 89.0.4389.90 allowed a remote attacker to potentially exploit heap corruption via a crafted HTML page.

- [https://github.com/JacobTaylor3/CVE-2021-21191---CVE-2021-21192](https://github.com/JacobTaylor3/CVE-2021-21191---CVE-2021-21192) :  ![starts](https://img.shields.io/github/stars/JacobTaylor3/CVE-2021-21191---CVE-2021-21192.svg) ![forks](https://img.shields.io/github/forks/JacobTaylor3/CVE-2021-21191---CVE-2021-21192.svg)


## CVE-2021-21191
 Use after free in WebRTC in Google Chrome prior to 89.0.4389.90 allowed a remote attacker to potentially exploit heap corruption via a crafted HTML page.

- [https://github.com/JacobTaylor3/CVE-2021-21191---CVE-2021-21192](https://github.com/JacobTaylor3/CVE-2021-21191---CVE-2021-21192) :  ![starts](https://img.shields.io/github/stars/JacobTaylor3/CVE-2021-21191---CVE-2021-21192.svg) ![forks](https://img.shields.io/github/forks/JacobTaylor3/CVE-2021-21191---CVE-2021-21192.svg)


## CVE-2021-3345
 _gcry_md_block_write in cipher/hash-common.c in Libgcrypt version 1.9.0 has a heap-based buffer overflow when the digest final function sets a large count value. It is recommended to upgrade to 1.9.1 or later.

- [https://github.com/MLGRadish/CVE-2021-3345](https://github.com/MLGRadish/CVE-2021-3345) :  ![starts](https://img.shields.io/github/stars/MLGRadish/CVE-2021-3345.svg) ![forks](https://img.shields.io/github/forks/MLGRadish/CVE-2021-3345.svg)
- [https://github.com/SpiralBL0CK/CVE-2021-3345](https://github.com/SpiralBL0CK/CVE-2021-3345) :  ![starts](https://img.shields.io/github/stars/SpiralBL0CK/CVE-2021-3345.svg) ![forks](https://img.shields.io/github/forks/SpiralBL0CK/CVE-2021-3345.svg)


## CVE-2021-3279
 sz.chat version 4 allows injection of web scripts and HTML in the message box.

- [https://github.com/rafaelchriss/CVE-2021-3279](https://github.com/rafaelchriss/CVE-2021-3279) :  ![starts](https://img.shields.io/github/stars/rafaelchriss/CVE-2021-3279.svg) ![forks](https://img.shields.io/github/forks/rafaelchriss/CVE-2021-3279.svg)


## CVE-2020-13654
 XWiki Platform before 12.8 mishandles escaping in the property displayer.

- [https://github.com/Astaruf/CVE-2020-13654](https://github.com/Astaruf/CVE-2020-13654) :  ![starts](https://img.shields.io/github/stars/Astaruf/CVE-2020-13654.svg) ![forks](https://img.shields.io/github/forks/Astaruf/CVE-2020-13654.svg)


## CVE-2017-5638
 The Jakarta Multipart parser in Apache Struts 2 2.3.x before 2.3.32 and 2.5.x before 2.5.10.1 has incorrect exception handling and error-message generation during file-upload attempts, which allows remote attackers to execute arbitrary commands via a crafted Content-Type, Content-Disposition, or Content-Length HTTP header, as exploited in the wild in March 2017 with a Content-Type header containing a #cmd= string.

- [https://github.com/ericrlessa/java-exploitable-quiz](https://github.com/ericrlessa/java-exploitable-quiz) :  ![starts](https://img.shields.io/github/stars/ericrlessa/java-exploitable-quiz.svg) ![forks](https://img.shields.io/github/forks/ericrlessa/java-exploitable-quiz.svg)

