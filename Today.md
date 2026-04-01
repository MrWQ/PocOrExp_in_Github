# Update 2026-04-01
## CVE-2026-33634
 Trivy is a security scanner. On March 19, 2026, a threat actor used compromised credentials to publish a malicious Trivy v0.69.4 release, force-push 76 of 77 version tags in `aquasecurity/trivy-action` to credential-stealing malware, and replace all 7 tags in `aquasecurity/setup-trivy` with malicious commits. This incident is a continuation of the supply chain attack that began in late February 2026. Following the initial disclosure on March 1, credential rotation was performed but was not atomic (not all credentials were revoked simultaneously). The attacker could have use a valid token to exfiltrate newly rotated secrets during the rotation window (which lasted a few days). This could have allowed the attacker to retain access and execute the March 19 attack. Affected components include the `aquasecurity/trivy` Go / Container image version 0.69.4, the `aquasecurity/trivy-action` GitHub Action versions 0.0.1 – 0.34.2 (76/77), and the`aquasecurity/setup-trivy` GitHub Action versions 0.2.0 – 0.2.6, prior to the recreation of 0.2.6 with a safe commit. Known safe versions include versions 0.69.2 and 0.69.3 of the Trivy binary, version 0.35.0 of trivy-action, and version 0.2.6 of setup-trivy. Additionally, take other mitigations to ensure the safety of secrets. If there is any possibility that a compromised version ran in one's environment, all secrets accessible to affected pipelines must be treated as exposed and rotated immediately. Check whether one's organization pulled or executed Trivy v0.69.4 from any source. Remove any affected artifacts immediately. Review all workflows using `aquasecurity/trivy-action` or `aquasecurity/setup-trivy`. Those who referenced a version tag rather than a full commit SHA should check workflow run logs from March 19–20, 2026 for signs of compromise. Look for repositories named `tpcp-docs` in one's GitHub organization. The presence of such a repository may indicate that the fallback exfiltration mechanism was triggered and secrets were successfully stolen. Pin GitHub Actions to full, immutable commit SHA hashes, don't use mutable version tags.

- [https://github.com/fevar54/CVE-2026-33634-Scanner](https://github.com/fevar54/CVE-2026-33634-Scanner) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-33634-Scanner.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-33634-Scanner.svg)


## CVE-2026-32606
 IncusOS is an immutable OS image dedicated to running Incus. Prior to 202603142010, the default configuration of systemd-cryptenroll as used by IncusOS through mkosi allows for an attacker with physical access to the machine to access the encrypted data without requiring any interaction by the system's owner or any tampering of Secure Boot state or kernel (UKI) boot image. That's because in this configuration, the LUKS key is made available by the TPM so long as the system has the expected PCR7 value and the PCR11 policy matches. That default PCR11 policy importantly allows for the TPM to release the key to the booted system rather than just from the initrd part of the signed kernel image (UKI). The attack relies on the attacker being able to substitute the original encrypted root partition for one that they control. By doing so, the system will prompt for a recovery key on boot, which the attacker has defined and can provide, before booting the system using the attacker's root partition rather than the system's original one. The attacker only needs to put a systemd unit starting on system boot within their root partition to have the system run that logic on boot. That unit will then run in an environment where the TPM will allow for the retrieval of the encryption key of the real root disk, allowing the attacker to steal the LUKS volume key (immutable master key) and then use it against the real root disk, altering it or getting data out before putting the disk back the way it was and returning the system without a trace of this attack having happened. This is all possible because the system will have still booted with Secure Boot enabled, will have measured and ran the expected bootloader and kernel image (UKI). The initrd selects the root disk based on GPT partition identifiers making it possible to easily substitute the real root disk for an attacker controlled one. This doesn't lead to any change in the TPM state and therefore allows for retrieval of the LUKS key by the attacker through a boot time systemd unit on their alternative root partition. IncusOS version 202603142010 (2026/03/14 20:10 UTC)  includes the new PCR15 logic and will automatically update the TPM policy on boot. Anyone suspecting that their system may have been physically accessed while shut down should perform a full system wipe and reinstallation as only that will rotate the LUKS volume key and prevent subsequent access to the encrypted data should the system have been previously compromised. There are no known workarounds other than updating to a version with corrected logic which will automatically rebind the LUKS keys to the new set of TPM registers and prevent this from being exploited.

- [https://github.com/gibmat/CVE-2026-32606-POC](https://github.com/gibmat/CVE-2026-32606-POC) :  ![starts](https://img.shields.io/github/stars/gibmat/CVE-2026-32606-POC.svg) ![forks](https://img.shields.io/github/forks/gibmat/CVE-2026-32606-POC.svg)


## CVE-2026-30082
 Multiple stored cross-site scripting (XSS) vulnerabilities in the Edit feature of the Software Package List page of IngEstate Server v11.14.0 allow attackers to execute arbitrary web scripts or HTML via injecting a crafted payload into the About application, What's news, or Release note parameters.

- [https://github.com/Cr0wld3r/CVE-2026-30082](https://github.com/Cr0wld3r/CVE-2026-30082) :  ![starts](https://img.shields.io/github/stars/Cr0wld3r/CVE-2026-30082.svg) ![forks](https://img.shields.io/github/forks/Cr0wld3r/CVE-2026-30082.svg)


## CVE-2026-29954
 In KubePlus 4.1.4, the mutating webhook and kubeconfiggenerator components have an SSRF vulnerability when processing the chartURL field of ResourceComposition resources. The field is only URL-encoded without validating the target address. More critically, when kubeconfiggenerator uses wget to download charts, the chartURL is directly concatenated into the command, allowing attackers to inject wget's `--header` option to achieve arbitrary HTTP header injection.

- [https://github.com/b0b0haha/CVE-2026-29954](https://github.com/b0b0haha/CVE-2026-29954) :  ![starts](https://img.shields.io/github/stars/b0b0haha/CVE-2026-29954.svg) ![forks](https://img.shields.io/github/forks/b0b0haha/CVE-2026-29954.svg)


## CVE-2026-29909
 MRCMS V3.1.2 contains an unauthenticated directory enumeration vulnerability in the file management module. The /admin/file/list.do endpoint lacks authentication controls and proper input validation, allowing remote attackers to enumerate directory contents on the server without any credentials.

- [https://github.com/qflksheep/CVE-2026-29909-MRCMS-vulnerability](https://github.com/qflksheep/CVE-2026-29909-MRCMS-vulnerability) :  ![starts](https://img.shields.io/github/stars/qflksheep/CVE-2026-29909-MRCMS-vulnerability.svg) ![forks](https://img.shields.io/github/forks/qflksheep/CVE-2026-29909-MRCMS-vulnerability.svg)


## CVE-2026-29597
 Incorrect access control in the file_details.asp endpoint of DDSN Interactive Acora CMS v10.7.1 allows attackers with editor privileges to access sensitive files via crafted requests.

- [https://github.com/padayali-JD/CVE-2026-29597](https://github.com/padayali-JD/CVE-2026-29597) :  ![starts](https://img.shields.io/github/stars/padayali-JD/CVE-2026-29597.svg) ![forks](https://img.shields.io/github/forks/padayali-JD/CVE-2026-29597.svg)


## CVE-2026-27876
Only instances with the sqlExpressions feature toggle enabled are vulnerable.

- [https://github.com/0xBlackash/CVE-2026-27876](https://github.com/0xBlackash/CVE-2026-27876) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-27876.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-27876.svg)


## CVE-2026-20999
 Authentication bypass by replay in Smart Switch prior to version 3.7.69.15 allows remote attackers to trigger privileged functions.

- [https://github.com/lasdjk/CVE-2026-20999-my-thought](https://github.com/lasdjk/CVE-2026-20999-my-thought) :  ![starts](https://img.shields.io/github/stars/lasdjk/CVE-2026-20999-my-thought.svg) ![forks](https://img.shields.io/github/forks/lasdjk/CVE-2026-20999-my-thought.svg)


## CVE-2026-20698
 The issue was addressed with improved memory handling. This issue is fixed in iOS 26.4 and iPadOS 26.4, macOS Tahoe 26.4, tvOS 26.4, visionOS 26.4, watchOS 26.4. An app may be able to cause unexpected system termination or corrupt kernel memory.

- [https://github.com/Somisomair/CVE-2026-20698-PF_ROUTE-Heap-Overflow](https://github.com/Somisomair/CVE-2026-20698-PF_ROUTE-Heap-Overflow) :  ![starts](https://img.shields.io/github/stars/Somisomair/CVE-2026-20698-PF_ROUTE-Heap-Overflow.svg) ![forks](https://img.shields.io/github/forks/Somisomair/CVE-2026-20698-PF_ROUTE-Heap-Overflow.svg)


## CVE-2026-1529
 A flaw was found in Keycloak. An attacker can exploit this vulnerability by modifying the organization ID and target email within a legitimate invitation token's JSON Web Token (JWT) payload. This lack of cryptographic signature verification allows the attacker to successfully self-register into an unauthorized organization, leading to unauthorized access.

- [https://github.com/ackemed/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation](https://github.com/ackemed/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation) :  ![starts](https://img.shields.io/github/stars/ackemed/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation.svg) ![forks](https://img.shields.io/github/forks/ackemed/CVE-2026-1529-PoC-keycloak-unauthorized-registration-via-improper-invitation-token-validation.svg)


## CVE-2025-67303
 An issue in ComfyUI-Manager prior to version 3.38 allowed remote attackers to potentially manipulate its configuration and critical data. This was due to the application storing its files in an insufficiently protected location that was accessible via the web interface

- [https://github.com/wcnmwcis/CVE-2026-22777](https://github.com/wcnmwcis/CVE-2026-22777) :  ![starts](https://img.shields.io/github/stars/wcnmwcis/CVE-2026-22777.svg) ![forks](https://img.shields.io/github/forks/wcnmwcis/CVE-2026-22777.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg)


## CVE-2025-54123
 Hoverfly is an open source API simulation tool. In versions 1.11.3 and prior, the middleware functionality in Hoverfly is vulnerable to command injection vulnerability at `/api/v2/hoverfly/middleware` endpoint due to insufficient validation and sanitization in user input. The vulnerability exists in the middleware management API endpoint `/api/v2/hoverfly/middleware`. This issue is born due to combination of three code level flaws: Insufficient Input Validation in middleware.go line 94-96; Unsafe Command Execution in local_middleware.go line 14-19; and Immediate Execution During Testing in hoverfly_service.go line 173. This allows an attacker to gain remote code execution (RCE) on any system running the vulnerable Hoverfly service. Since the input is directly passed to system commands without proper checks, an attacker can upload a malicious payload or directly execute arbitrary commands (including reverse shells) on the host server with the privileges of the Hoverfly process. Commit 17e60a9bc78826deb4b782dca1c1abd3dbe60d40 in version 1.12.0 disables the set middleware API by default, and subsequent changes to documentation make users aware of the security changes of exposing the set middleware API.

- [https://github.com/f4dee-backup/CVE-2025-54123](https://github.com/f4dee-backup/CVE-2025-54123) :  ![starts](https://img.shields.io/github/stars/f4dee-backup/CVE-2025-54123.svg) ![forks](https://img.shields.io/github/forks/f4dee-backup/CVE-2025-54123.svg)


## CVE-2025-31161
 CrushFTP 10 before 10.8.4 and 11 before 11.3.1 allows authentication bypass and takeover of the crushadmin account (unless a DMZ proxy instance is used), as exploited in the wild in March and April 2025, aka "Unauthenticated HTTP(S) port access." A race condition exists in the AWS4-HMAC (compatible with S3) authorization method of the HTTP component of the FTP server. The server first verifies the existence of the user by performing a call to login_user_pass() with no password requirement. This will authenticate the session through the HMAC verification process and up until the server checks for user verification once more. The vulnerability can be further stabilized, eliminating the need for successfully triggering a race condition, by sending a mangled AWS4-HMAC header. By providing only the username and a following slash (/), the server will successfully find a username, which triggers the successful anypass authentication process, but the server will fail to find the expected SignedHeaders entry, resulting in an index-out-of-bounds error that stops the code from reaching the session cleanup. Together, these issues make it trivial to authenticate as any known or guessable user (e.g., crushadmin), and can lead to a full compromise of the system by obtaining an administrative account.

- [https://github.com/t0x1nsec/CVE-2025-31161](https://github.com/t0x1nsec/CVE-2025-31161) :  ![starts](https://img.shields.io/github/stars/t0x1nsec/CVE-2025-31161.svg) ![forks](https://img.shields.io/github/forks/t0x1nsec/CVE-2025-31161.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-27591
 A privilege escalation vulnerability existed in the Below service prior to v0.9.0 due to the creation of a world-writable directory at /var/log/below. This could have allowed local unprivileged users to escalate to root privileges through symlink attacks that manipulate files such as /etc/shadow.

- [https://github.com/nikolas-trey/CVE-2025-27591](https://github.com/nikolas-trey/CVE-2025-27591) :  ![starts](https://img.shields.io/github/stars/nikolas-trey/CVE-2025-27591.svg) ![forks](https://img.shields.io/github/forks/nikolas-trey/CVE-2025-27591.svg)


## CVE-2025-27237
 In Zabbix Agent and Agent 2 on Windows, the OpenSSL configuration file is loaded from a path writable by low-privileged users, allowing malicious modification and potential local privilege escalation by injecting a DLL.

- [https://github.com/HackingLZ/CVE-2025-27237](https://github.com/HackingLZ/CVE-2025-27237) :  ![starts](https://img.shields.io/github/stars/HackingLZ/CVE-2025-27237.svg) ![forks](https://img.shields.io/github/forks/HackingLZ/CVE-2025-27237.svg)


## CVE-2025-24071
 Exposure of sensitive information to an unauthorized actor in Windows File Explorer allows an unauthorized attacker to perform spoofing over a network.

- [https://github.com/t0x1nsec/Windows-Explorer-CVE-2025-24071](https://github.com/t0x1nsec/Windows-Explorer-CVE-2025-24071) :  ![starts](https://img.shields.io/github/stars/t0x1nsec/Windows-Explorer-CVE-2025-24071.svg) ![forks](https://img.shields.io/github/forks/t0x1nsec/Windows-Explorer-CVE-2025-24071.svg)


## CVE-2025-2886
 Missing validation of terminating delegation causes the client to continue searching the defined delegation list, even after searching a terminating delegation. This could cause the client to fetch a target from an incorrect source, altering the target contents. Users should upgrade to tough version 0.20.0 or later and ensure any forked or derivative code is patched to incorporate the new fixes.

- [https://github.com/murataydemir/AWS-Tough-Library-Multiple-CVEs](https://github.com/murataydemir/AWS-Tough-Library-Multiple-CVEs) :  ![starts](https://img.shields.io/github/stars/murataydemir/AWS-Tough-Library-Multiple-CVEs.svg) ![forks](https://img.shields.io/github/forks/murataydemir/AWS-Tough-Library-Multiple-CVEs.svg)


## CVE-2025-2783
 Incorrect handle provided in unspecified circumstances in Mojo in Google Chrome on Windows prior to 134.0.6998.177 allowed a remote attacker to perform a sandbox escape via a malicious file. (Chromium security severity: High)

- [https://github.com/Alchemist3dot14/CVE-2025-2783](https://github.com/Alchemist3dot14/CVE-2025-2783) :  ![starts](https://img.shields.io/github/stars/Alchemist3dot14/CVE-2025-2783.svg) ![forks](https://img.shields.io/github/forks/Alchemist3dot14/CVE-2025-2783.svg)
- [https://github.com/Leviticus-Triage/ChromSploit-Framework](https://github.com/Leviticus-Triage/ChromSploit-Framework) :  ![starts](https://img.shields.io/github/stars/Leviticus-Triage/ChromSploit-Framework.svg) ![forks](https://img.shields.io/github/forks/Leviticus-Triage/ChromSploit-Framework.svg)
- [https://github.com/byteReaper77/CVE-2025-2783](https://github.com/byteReaper77/CVE-2025-2783) :  ![starts](https://img.shields.io/github/stars/byteReaper77/CVE-2025-2783.svg) ![forks](https://img.shields.io/github/forks/byteReaper77/CVE-2025-2783.svg)


## CVE-2025-2534
 IBM Db2 11.1.0 through 11.1.4.7, 11.5.0 through 11.5.9, and 12.1.0 through 12.1.3 for Linux, UNIX and Windows (includes Db2 Connect Server) is vulnerable to a denial of service as the server may crash under certain conditions with a specially crafted query.

- [https://github.com/Yetazyyy/CVE-2025-25347](https://github.com/Yetazyyy/CVE-2025-25347) :  ![starts](https://img.shields.io/github/stars/Yetazyyy/CVE-2025-25347.svg) ![forks](https://img.shields.io/github/forks/Yetazyyy/CVE-2025-25347.svg)
- [https://github.com/l00neyhacker/CVE-2025-25340](https://github.com/l00neyhacker/CVE-2025-25340) :  ![starts](https://img.shields.io/github/stars/l00neyhacker/CVE-2025-25340.svg) ![forks](https://img.shields.io/github/forks/l00neyhacker/CVE-2025-25340.svg)


## CVE-2025-2502
 An improper default permissions vulnerability was reported in Lenovo PC Manager that could allow a local attacker to elevate privileges.

- [https://github.com/IHK-ONE/CVE-2025-2502](https://github.com/IHK-ONE/CVE-2025-2502) :  ![starts](https://img.shields.io/github/stars/IHK-ONE/CVE-2025-2502.svg) ![forks](https://img.shields.io/github/forks/IHK-ONE/CVE-2025-2502.svg)


## CVE-2025-0411
The specific flaw exists within the handling of archived files. When extracting files from a crafted archive that bears the Mark-of-the-Web, 7-Zip does not propagate the Mark-of-the-Web to the extracted files. An attacker can leverage this vulnerability to execute arbitrary code in the context of the current user. Was ZDI-CAN-25456.

- [https://github.com/t0x1nsec/7-Zip-CVE-2025-0411-POC](https://github.com/t0x1nsec/7-Zip-CVE-2025-0411-POC) :  ![starts](https://img.shields.io/github/stars/t0x1nsec/7-Zip-CVE-2025-0411-POC.svg) ![forks](https://img.shields.io/github/forks/t0x1nsec/7-Zip-CVE-2025-0411-POC.svg)


## CVE-2024-38998
 DO NOT USE THIS CANDIDATE NUMBER. ConsultIDs: none. Reason: This candidate was withdrawn by its CNA. Further investigation showed that it was not a security issue. Notes: none.

- [https://github.com/t0x1nsec/PP_CVE-2024-38998](https://github.com/t0x1nsec/PP_CVE-2024-38998) :  ![starts](https://img.shields.io/github/stars/t0x1nsec/PP_CVE-2024-38998.svg) ![forks](https://img.shields.io/github/forks/t0x1nsec/PP_CVE-2024-38998.svg)


## CVE-2024-3400
Cloud NGFW, Panorama appliances, and Prisma Access are not impacted by this vulnerability.

- [https://github.com/HackingLZ/panrapidcheck](https://github.com/HackingLZ/panrapidcheck) :  ![starts](https://img.shields.io/github/stars/HackingLZ/panrapidcheck.svg) ![forks](https://img.shields.io/github/forks/HackingLZ/panrapidcheck.svg)


## CVE-2024-1086
We recommend upgrading past commit f342de4e2f33e0e39165d8639387aa6c19dff660.

- [https://github.com/vettrivel007/CVE-2024-1086](https://github.com/vettrivel007/CVE-2024-1086) :  ![starts](https://img.shields.io/github/stars/vettrivel007/CVE-2024-1086.svg) ![forks](https://img.shields.io/github/forks/vettrivel007/CVE-2024-1086.svg)


## CVE-2023-48223
 fast-jwt provides fast JSON Web Token (JWT) implementation. Prior to version 3.3.2, the fast-jwt library does not properly prevent JWT algorithm confusion for all public key types. The 'publicKeyPemMatcher' in 'fast-jwt/src/crypto.js' does not properly match all common PEM formats for public keys. To exploit this vulnerability, an attacker needs to craft a malicious JWT token containing the HS256 algorithm, signed with the public RSA key of the victim application. This attack will only work if the victim application utilizes a public key containing the `BEGIN RSA PUBLIC KEY` header. Applications using the RS256 algorithm, a public key with a `BEGIN RSA PUBLIC KEY` header, and calling the verify function without explicitly providing an algorithm, are vulnerable to this algorithm confusion attack which allows attackers to sign arbitrary payloads which will be accepted by the verifier. Version 3.3.2 contains a patch for this issue. As a workaround, change line 29 of `blob/master/src/crypto.js` to include a regular expression.

- [https://github.com/lucastran05/CVE-2023-48223](https://github.com/lucastran05/CVE-2023-48223) :  ![starts](https://img.shields.io/github/stars/lucastran05/CVE-2023-48223.svg) ![forks](https://img.shields.io/github/forks/lucastran05/CVE-2023-48223.svg)


## CVE-2023-46604
which fixes this issue.

- [https://github.com/mkdemir/activemq-lockbit-analysis](https://github.com/mkdemir/activemq-lockbit-analysis) :  ![starts](https://img.shields.io/github/stars/mkdemir/activemq-lockbit-analysis.svg) ![forks](https://img.shields.io/github/forks/mkdemir/activemq-lockbit-analysis.svg)


## CVE-2023-3262
 The Dataprobe iBoot PDU running firmware version 1.43.03312023 or earlier uses hard-coded credentials for all interactions with the internal Postgres database.A malicious agent with the ability to execute operating system commands on the device can leverage this vulnerability to read, modify, or delete arbitrary database records.

- [https://github.com/SanjayRagavendar/Ubuntu-GameOver-Lay](https://github.com/SanjayRagavendar/Ubuntu-GameOver-Lay) :  ![starts](https://img.shields.io/github/stars/SanjayRagavendar/Ubuntu-GameOver-Lay.svg) ![forks](https://img.shields.io/github/forks/SanjayRagavendar/Ubuntu-GameOver-Lay.svg)


## CVE-2022-39299
 Passport-SAML is a SAML 2.0 authentication provider for Passport, the Node.js authentication library. A remote attacker may be able to bypass SAML authentication on a website using passport-saml. A successful attack requires that the attacker is in possession of an arbitrary IDP signed XML element. Depending on the IDP used, fully unauthenticated attacks (e.g without access to a valid user) might also be feasible if generation of a signed message can be triggered. Users should upgrade to passport-saml version 3.2.2 or newer. The issue was also present in the beta releases of `node-saml` before version 4.0.0-beta.5. If you cannot upgrade, disabling SAML authentication may be done as a workaround.

- [https://github.com/KaztoRay/CVE-2022-39299-Research](https://github.com/KaztoRay/CVE-2022-39299-Research) :  ![starts](https://img.shields.io/github/stars/KaztoRay/CVE-2022-39299-Research.svg) ![forks](https://img.shields.io/github/forks/KaztoRay/CVE-2022-39299-Research.svg)


## CVE-2022-22947
 In spring cloud gateway versions prior to 3.1.1+ and 3.0.7+ , applications are vulnerable to a code injection attack when the Gateway Actuator endpoint is enabled, exposed and unsecured. A remote attacker could make a maliciously crafted request that could allow arbitrary remote execution on the remote host.

- [https://github.com/SanderSchepers1993/CyberSec2026](https://github.com/SanderSchepers1993/CyberSec2026) :  ![starts](https://img.shields.io/github/stars/SanderSchepers1993/CyberSec2026.svg) ![forks](https://img.shields.io/github/forks/SanderSchepers1993/CyberSec2026.svg)


## CVE-2020-10188
 utility.c in telnetd in netkit telnet through 0.17 allows remote attackers to execute arbitrary code via short writes or urgent data, because of a buffer overflow involving the netclear and nextitem functions.

- [https://github.com/hackingyseguridad/ssha](https://github.com/hackingyseguridad/ssha) :  ![starts](https://img.shields.io/github/stars/hackingyseguridad/ssha.svg) ![forks](https://img.shields.io/github/forks/hackingyseguridad/ssha.svg)


## CVE-2019-1010298
 Linaro/OP-TEE OP-TEE 3.3.0 and earlier is affected by: Buffer Overflow. The impact is: Code execution in the context of TEE core (kernel). The component is: optee_os. The fixed version is: 3.4.0 and later.

- [https://github.com/RKX1209/CVE-2019-1010298](https://github.com/RKX1209/CVE-2019-1010298) :  ![starts](https://img.shields.io/github/stars/RKX1209/CVE-2019-1010298.svg) ![forks](https://img.shields.io/github/forks/RKX1209/CVE-2019-1010298.svg)


## CVE-2019-12588
 The client 802.11 mac implementation in Espressif ESP8266_NONOS_SDK 2.2.0 through 3.1.0 does not validate correctly the RSN AuthKey suite list count in beacon frames, probe responses, and association responses, which allows attackers in radio range to cause a denial of service (crash) via a crafted message.

- [https://github.com/Matheus-Garbelini/esp32_esp8266_attacks](https://github.com/Matheus-Garbelini/esp32_esp8266_attacks) :  ![starts](https://img.shields.io/github/stars/Matheus-Garbelini/esp32_esp8266_attacks.svg) ![forks](https://img.shields.io/github/forks/Matheus-Garbelini/esp32_esp8266_attacks.svg)


## CVE-2018-15473
 OpenSSH through 7.7 is prone to a user enumeration vulnerability due to not delaying bailout for an invalid authenticating user until after the packet containing the request has been fully parsed, related to auth2-gss.c, auth2-hostbased.c, and auth2-pubkey.c.

- [https://github.com/wtbacon/cve-2018-15473](https://github.com/wtbacon/cve-2018-15473) :  ![starts](https://img.shields.io/github/stars/wtbacon/cve-2018-15473.svg) ![forks](https://img.shields.io/github/forks/wtbacon/cve-2018-15473.svg)


## CVE-2018-6537
 A buffer overflow vulnerability in the control protocol of Flexense SyncBreeze Enterprise v10.4.18 allows remote attackers to execute arbitrary code by sending a crafted packet to TCP port 9121.

- [https://github.com/damariion/CVE-2018-6537.RCE](https://github.com/damariion/CVE-2018-6537.RCE) :  ![starts](https://img.shields.io/github/stars/damariion/CVE-2018-6537.RCE.svg) ![forks](https://img.shields.io/github/forks/damariion/CVE-2018-6537.RCE.svg)


## CVE-2017-14980
 Buffer overflow in Sync Breeze Enterprise 10.0.28 allows remote attackers to have unspecified impact via a long username parameter to /login.

- [https://github.com/damariion/CVE-2017-14980.RCE](https://github.com/damariion/CVE-2017-14980.RCE) :  ![starts](https://img.shields.io/github/stars/damariion/CVE-2017-14980.RCE.svg) ![forks](https://img.shields.io/github/forks/damariion/CVE-2017-14980.RCE.svg)


## CVE-2015-8522
 Buffer overflow in the server in IBM Tivoli Storage Manager FastBack 5.5.x and 6.x before 6.1.12.2 allows remote attackers to execute arbitrary code via a crafted command, a different vulnerability than CVE-2015-8519, CVE-2015-8520, and CVE-2015-8521.

- [https://github.com/damariion/CVE-2015-8522.RCE](https://github.com/damariion/CVE-2015-8522.RCE) :  ![starts](https://img.shields.io/github/stars/damariion/CVE-2015-8522.RCE.svg) ![forks](https://img.shields.io/github/forks/damariion/CVE-2015-8522.RCE.svg)


## CVE-2015-1925
 Stack-based buffer overflow in the server in IBM Tivoli Storage Manager FastBack 6.1 before 6.1.12 allows remote attackers to cause a denial of service (daemon crash) via unspecified vectors, a different vulnerability than CVE-2015-1924, CVE-2015-1929, CVE-2015-1930, CVE-2015-1948, CVE-2015-1953, CVE-2015-1954, CVE-2015-1962, CVE-2015-1963, CVE-2015-1964, and CVE-2015-1965.

- [https://github.com/damariion/CVE-2015-1925.RCE](https://github.com/damariion/CVE-2015-1925.RCE) :  ![starts](https://img.shields.io/github/stars/damariion/CVE-2015-1925.RCE.svg) ![forks](https://img.shields.io/github/forks/damariion/CVE-2015-1925.RCE.svg)

