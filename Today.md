# Update 2026-03-26
## CVE-2026-33634
 Trivy is a security scanner. On March 19, 2026, a threat actor used compromised credentials to publish a malicious Trivy v0.69.4 release, force-push 76 of 77 version tags in `aquasecurity/trivy-action` to credential-stealing malware, and replace all 7 tags in `aquasecurity/setup-trivy` with malicious commits. This incident is a continuation of the supply chain attack that began in late February 2026. Following the initial disclosure on March 1, credential rotation was performed but was not atomic (not all credentials were revoked simultaneously). The attacker could have use a valid token to exfiltrate newly rotated secrets during the rotation window (which lasted a few days). This could have allowed the attacker to retain access and execute the March 19 attack. Affected components include the `aquasecurity/trivy` Go / Container image version 0.69.4, the `aquasecurity/trivy-action` GitHub Action versions 0.0.1 – 0.34.2 (76/77), and the`aquasecurity/setup-trivy` GitHub Action versions 0.2.0 – 0.2.6, prior to the recreation of 0.2.6 with a safe commit. Known safe versions include versions 0.69.2 and 0.69.3 of the Trivy binary, version 0.35.0 of trivy-action, and version 0.2.6 of setup-trivy. Additionally, take other mitigations to ensure the safety of secrets. If there is any possibility that a compromised version ran in one's environment, all secrets accessible to affected pipelines must be treated as exposed and rotated immediately. Check whether one's organization pulled or executed Trivy v0.69.4 from any source. Remove any affected artifacts immediately. Review all workflows using `aquasecurity/trivy-action` or `aquasecurity/setup-trivy`. Those who referenced a version tag rather than a full commit SHA should check workflow run logs from March 19–20, 2026 for signs of compromise. Look for repositories named `tpcp-docs` in one's GitHub organization. The presence of such a repository may indicate that the fallback exfiltration mechanism was triggered and secrets were successfully stolen. Pin GitHub Actions to full, immutable commit SHA hashes, don't use mutable version tags.

- [https://github.com/ugurrates/teampcp-supply-chain-attack](https://github.com/ugurrates/teampcp-supply-chain-attack) :  ![starts](https://img.shields.io/github/stars/ugurrates/teampcp-supply-chain-attack.svg) ![forks](https://img.shields.io/github/forks/ugurrates/teampcp-supply-chain-attack.svg)


## CVE-2026-32913
 OpenClaw before 2026.3.7 contains an improper header validation vulnerability in fetchWithSsrFGuard that forwards custom authorization headers across cross-origin redirects. Attackers can trigger redirects to different origins to intercept sensitive headers like X-Api-Key and Private-Token intended for the original destination.

- [https://github.com/Rickidevs/CVE-2026-32913](https://github.com/Rickidevs/CVE-2026-32913) :  ![starts](https://img.shields.io/github/stars/Rickidevs/CVE-2026-32913.svg) ![forks](https://img.shields.io/github/forks/Rickidevs/CVE-2026-32913.svg)


## CVE-2026-30655
 SQL injection in Solicitante::resetaSenha() in esiclivre/esiclivre v0.2.2 and earlier allows unauthenticated remote attackers to gain unauthorized access to sensitive information via the cpfcnpj parameter in /reset/index.php

- [https://github.com/brynax/CVE-2026-30655](https://github.com/brynax/CVE-2026-30655) :  ![starts](https://img.shields.io/github/stars/brynax/CVE-2026-30655.svg) ![forks](https://img.shields.io/github/forks/brynax/CVE-2026-30655.svg)


## CVE-2026-29000
 pac4j-jwt versions prior to 4.5.9, 5.7.9, and 6.3.3 contain an authentication bypass vulnerability in JwtAuthenticator when processing encrypted JWTs that allows remote attackers to forge authentication tokens. Attackers who possess the server's RSA public key can create a JWE-wrapped PlainJWT with arbitrary subject and role claims, bypassing signature verification to authenticate as any user including administrators.

- [https://github.com/PtechAmanja/CVE-2026-29000-pac4j-jwt-auth-bypass](https://github.com/PtechAmanja/CVE-2026-29000-pac4j-jwt-auth-bypass) :  ![starts](https://img.shields.io/github/stars/PtechAmanja/CVE-2026-29000-pac4j-jwt-auth-bypass.svg) ![forks](https://img.shields.io/github/forks/PtechAmanja/CVE-2026-29000-pac4j-jwt-auth-bypass.svg)


## CVE-2026-25253
 OpenClaw (aka clawdbot or Moltbot) before 2026.1.29 obtains a gatewayUrl value from a query string and automatically makes a WebSocket connection without prompting, sending a token value.

- [https://github.com/ZhaoymOvO/openclaw-1click-rce-env](https://github.com/ZhaoymOvO/openclaw-1click-rce-env) :  ![starts](https://img.shields.io/github/stars/ZhaoymOvO/openclaw-1click-rce-env.svg) ![forks](https://img.shields.io/github/forks/ZhaoymOvO/openclaw-1click-rce-env.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/InzegoSec/CVE-2026-23744](https://github.com/InzegoSec/CVE-2026-23744) :  ![starts](https://img.shields.io/github/stars/InzegoSec/CVE-2026-23744.svg) ![forks](https://img.shields.io/github/forks/InzegoSec/CVE-2026-23744.svg)


## CVE-2026-21509
 Reliance on untrusted inputs in a security decision in Microsoft Office allows an unauthorized attacker to bypass a security feature locally.

- [https://github.com/YoussefMami/CVE2026_21509](https://github.com/YoussefMami/CVE2026_21509) :  ![starts](https://img.shields.io/github/stars/YoussefMami/CVE2026_21509.svg) ![forks](https://img.shields.io/github/forks/YoussefMami/CVE2026_21509.svg)


## CVE-2026-2683
 A vulnerability was found in Tsinghua Unigroup Electronic Archives System 3.2.210802(62532). The affected element is an unknown function of the file /Using/Subject/downLoad.html. Performing a manipulation of the argument path results in path traversal. The attack may be initiated remotely. The exploit has been made public and could be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/zebbernCVE/CVE-2026-26832](https://github.com/zebbernCVE/CVE-2026-26832) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26832.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26832.svg)
- [https://github.com/zebbernCVE/CVE-2026-26833](https://github.com/zebbernCVE/CVE-2026-26833) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26833.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26833.svg)
- [https://github.com/zebbernCVE/CVE-2026-26830](https://github.com/zebbernCVE/CVE-2026-26830) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26830.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26830.svg)
- [https://github.com/zebbernCVE/CVE-2026-26831](https://github.com/zebbernCVE/CVE-2026-26831) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-26831.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-26831.svg)
- [https://github.com/zebbernCVE/npm-cve-2026-26830-26833](https://github.com/zebbernCVE/npm-cve-2026-26830-26833) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/npm-cve-2026-26830-26833.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/npm-cve-2026-26830-26833.svg)


## CVE-2026-2068
 A vulnerability was detected in UTT 进取 520W 1.7.7-180627. This issue affects the function strcpy of the file /goform/formSyslogConf. The manipulation of the argument ServerIp results in buffer overflow. The attack may be launched remotely. The exploit is now public and may be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF](https://github.com/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF) :  ![starts](https://img.shields.io/github/stars/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF.svg) ![forks](https://img.shields.io/github/forks/zeroxjf/CVE-2026-20687-AppleSEPKeyStore-UAF.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/InferiorAK/CVE-2025-55182-React2Shell-Async-Scanner](https://github.com/InferiorAK/CVE-2025-55182-React2Shell-Async-Scanner) :  ![starts](https://img.shields.io/github/stars/InferiorAK/CVE-2025-55182-React2Shell-Async-Scanner.svg) ![forks](https://img.shields.io/github/forks/InferiorAK/CVE-2025-55182-React2Shell-Async-Scanner.svg)
- [https://github.com/meneim99/react2shell-scanner](https://github.com/meneim99/react2shell-scanner) :  ![starts](https://img.shields.io/github/stars/meneim99/react2shell-scanner.svg) ![forks](https://img.shields.io/github/forks/meneim99/react2shell-scanner.svg)


## CVE-2025-50472
 The modelscope/ms-swift library thru 2.6.1 is vulnerable to arbitrary code execution through deserialization of untrusted data within the `load_model_meta()` function of the `ModelFileSystemCache()` class. Attackers can execute arbitrary code and commands by crafting a malicious serialized `.mdl` payload, exploiting the use of `pickle.load()` on data from potentially untrusted sources. This vulnerability allows for remote code execution (RCE) by deceiving victims into loading a seemingly harmless checkpoint during a normal training process, thereby enabling attackers to execute arbitrary code on the targeted machine. Note that the payload file is a hidden file, making it difficult for the victim to detect tampering. More importantly, during the model training process, after the `.mdl` file is loaded and executes arbitrary code, the normal training process remains unaffected'meaning the user remains unaware of the arbitrary code execution.

- [https://github.com/Before-Rain/CVE-2025-50472](https://github.com/Before-Rain/CVE-2025-50472) :  ![starts](https://img.shields.io/github/stars/Before-Rain/CVE-2025-50472.svg) ![forks](https://img.shields.io/github/forks/Before-Rain/CVE-2025-50472.svg)


## CVE-2025-49596
 The MCP inspector is a developer tool for testing and debugging MCP servers. Versions of MCP Inspector below 0.14.1 are vulnerable to remote code execution due to lack of authentication between the Inspector client and proxy, allowing unauthenticated requests to launch MCP commands over stdio. Users should immediately upgrade to version 0.14.1 or later to address these vulnerabilities.

- [https://github.com/pppxo/CVE-2025-49596-PoC](https://github.com/pppxo/CVE-2025-49596-PoC) :  ![starts](https://img.shields.io/github/stars/pppxo/CVE-2025-49596-PoC.svg) ![forks](https://img.shields.io/github/forks/pppxo/CVE-2025-49596-PoC.svg)


## CVE-2025-27591
 A privilege escalation vulnerability existed in the Below service prior to v0.9.0 due to the creation of a world-writable directory at /var/log/below. This could have allowed local unprivileged users to escalate to root privileges through symlink attacks that manipulate files such as /etc/shadow.

- [https://github.com/umutatalar/CVE-2025-27591](https://github.com/umutatalar/CVE-2025-27591) :  ![starts](https://img.shields.io/github/stars/umutatalar/CVE-2025-27591.svg) ![forks](https://img.shields.io/github/forks/umutatalar/CVE-2025-27591.svg)


## CVE-2025-21298
 Windows OLE Remote Code Execution Vulnerability

- [https://github.com/tarunbharathe/Zero-Click-RCE-Incident-Response-CVE-2025-21298](https://github.com/tarunbharathe/Zero-Click-RCE-Incident-Response-CVE-2025-21298) :  ![starts](https://img.shields.io/github/stars/tarunbharathe/Zero-Click-RCE-Incident-Response-CVE-2025-21298.svg) ![forks](https://img.shields.io/github/forks/tarunbharathe/Zero-Click-RCE-Incident-Response-CVE-2025-21298.svg)


## CVE-2025-14340
 Cross-site scripting in REST Management Interface in Payara Server 4.1.2.191.54, 5.83.0, 6.34.0, 7.2026.1 allows an attacker to mislead the administrator to change the admin password via URL Payload.

- [https://github.com/DeepSecurityResearch/CVE-2025-14340](https://github.com/DeepSecurityResearch/CVE-2025-14340) :  ![starts](https://img.shields.io/github/stars/DeepSecurityResearch/CVE-2025-14340.svg) ![forks](https://img.shields.io/github/forks/DeepSecurityResearch/CVE-2025-14340.svg)


## CVE-2025-9074
This can lead to execution of a wide range of privileged commands to the engine API, including controlling other containers, creating new ones, managing images etc. In some circumstances (e.g. Docker Desktop for Windows with WSL backend) it also allows mounting the host drive with the same privileges as the user running Docker Desktop.

- [https://github.com/XRayZen/cve-2025-9074-poc](https://github.com/XRayZen/cve-2025-9074-poc) :  ![starts](https://img.shields.io/github/stars/XRayZen/cve-2025-9074-poc.svg) ![forks](https://img.shields.io/github/forks/XRayZen/cve-2025-9074-poc.svg)


## CVE-2025-3248
code.

- [https://github.com/12-test-12/CVE-2025-3248](https://github.com/12-test-12/CVE-2025-3248) :  ![starts](https://img.shields.io/github/stars/12-test-12/CVE-2025-3248.svg) ![forks](https://img.shields.io/github/forks/12-test-12/CVE-2025-3248.svg)


## CVE-2025-2534
 IBM Db2 11.1.0 through 11.1.4.7, 11.5.0 through 11.5.9, and 12.1.0 through 12.1.3 for Linux, UNIX and Windows (includes Db2 Connect Server) is vulnerable to a denial of service as the server may crash under certain conditions with a specially crafted query.

- [https://github.com/Yetazyyy/CVE-2025-25347](https://github.com/Yetazyyy/CVE-2025-25347) :  ![starts](https://img.shields.io/github/stars/Yetazyyy/CVE-2025-25347.svg) ![forks](https://img.shields.io/github/forks/Yetazyyy/CVE-2025-25347.svg)


## CVE-2024-51324
 An issue in the BdApiUtil driver of Baidu Antivirus v5.2.3.116083 allows attackers to terminate arbitrary process via executing a BYOVD (Bring Your Own Vulnerable Driver) attack.

- [https://github.com/devianntsec/CVE-2024-51324-BYOVD-Masters-Thesis](https://github.com/devianntsec/CVE-2024-51324-BYOVD-Masters-Thesis) :  ![starts](https://img.shields.io/github/stars/devianntsec/CVE-2024-51324-BYOVD-Masters-Thesis.svg) ![forks](https://img.shields.io/github/forks/devianntsec/CVE-2024-51324-BYOVD-Masters-Thesis.svg)


## CVE-2024-30051
 Windows DWM Core Library Elevation of Privilege Vulnerability

- [https://github.com/devianntsec/CVE-2024-30051-DWMHeapOverflow-Masters-Thesis](https://github.com/devianntsec/CVE-2024-30051-DWMHeapOverflow-Masters-Thesis) :  ![starts](https://img.shields.io/github/stars/devianntsec/CVE-2024-30051-DWMHeapOverflow-Masters-Thesis.svg) ![forks](https://img.shields.io/github/forks/devianntsec/CVE-2024-30051-DWMHeapOverflow-Masters-Thesis.svg)


## CVE-2022-30190
Please see the MSRC Blog Entry for important information about steps you can take to protect your system from this vulnerability.

- [https://github.com/ImVihanga03/Static-Malware-Analysis-Follina-CVE-2022-30190](https://github.com/ImVihanga03/Static-Malware-Analysis-Follina-CVE-2022-30190) :  ![starts](https://img.shields.io/github/stars/ImVihanga03/Static-Malware-Analysis-Follina-CVE-2022-30190.svg) ![forks](https://img.shields.io/github/forks/ImVihanga03/Static-Malware-Analysis-Follina-CVE-2022-30190.svg)


## CVE-2022-22965
 A Spring MVC or Spring WebFlux application running on JDK 9+ may be vulnerable to remote code execution (RCE) via data binding. The specific exploit requires the application to run on Tomcat as a WAR deployment. If the application is deployed as a Spring Boot executable jar, i.e. the default, it is not vulnerable to the exploit. However, the nature of the vulnerability is more general, and there may be other ways to exploit it.

- [https://github.com/Shakur1314/CVE-2022-22965-Spring4Shell-Security-Operations-Analysis](https://github.com/Shakur1314/CVE-2022-22965-Spring4Shell-Security-Operations-Analysis) :  ![starts](https://img.shields.io/github/stars/Shakur1314/CVE-2022-22965-Spring4Shell-Security-Operations-Analysis.svg) ![forks](https://img.shields.io/github/forks/Shakur1314/CVE-2022-22965-Spring4Shell-Security-Operations-Analysis.svg)


## CVE-2022-0944
 Template injection in connection test endpoint leads to RCE in GitHub repository sqlpad/sqlpad prior to 6.10.1.

- [https://github.com/NeoArtemis37/OverlayFS-PrivEsc-CVE-2022-0944](https://github.com/NeoArtemis37/OverlayFS-PrivEsc-CVE-2022-0944) :  ![starts](https://img.shields.io/github/stars/NeoArtemis37/OverlayFS-PrivEsc-CVE-2022-0944.svg) ![forks](https://img.shields.io/github/forks/NeoArtemis37/OverlayFS-PrivEsc-CVE-2022-0944.svg)


## CVE-2021-22911
 A improper input sanitization vulnerability exists in Rocket.Chat server 3.11, 3.12 & 3.13 that could lead to unauthenticated NoSQL injection, resulting potentially in RCE.

- [https://github.com/Faridi-m/CVE-2021-22911-RocketChat](https://github.com/Faridi-m/CVE-2021-22911-RocketChat) :  ![starts](https://img.shields.io/github/stars/Faridi-m/CVE-2021-22911-RocketChat.svg) ![forks](https://img.shields.io/github/forks/Faridi-m/CVE-2021-22911-RocketChat.svg)


## CVE-2019-13506
 @nuxt/devalue before 1.2.3, as used in Nuxt.js before 2.6.2, mishandles object keys, leading to XSS.

- [https://github.com/CQ-Tools/CVE-2019-13506-unfixed](https://github.com/CQ-Tools/CVE-2019-13506-unfixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2019-13506-unfixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2019-13506-unfixed.svg)
- [https://github.com/CQ-Tools/CVE-2019-13506-fixed](https://github.com/CQ-Tools/CVE-2019-13506-fixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2019-13506-fixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2019-13506-fixed.svg)
- [https://github.com/ossf-cve-benchmark/CVE-2019-13506](https://github.com/ossf-cve-benchmark/CVE-2019-13506) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2019-13506.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2019-13506.svg)


## CVE-2018-15473
 OpenSSH through 7.7 is prone to a user enumeration vulnerability due to not delaying bailout for an invalid authenticating user until after the packet containing the request has been fully parsed, related to auth2-gss.c, auth2-hostbased.c, and auth2-pubkey.c.

- [https://github.com/K3rn3l-32/Threaded-CVE-2018-15473](https://github.com/K3rn3l-32/Threaded-CVE-2018-15473) :  ![starts](https://img.shields.io/github/stars/K3rn3l-32/Threaded-CVE-2018-15473.svg) ![forks](https://img.shields.io/github/forks/K3rn3l-32/Threaded-CVE-2018-15473.svg)

