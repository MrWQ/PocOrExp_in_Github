# Update 2026-04-07
## CVE-2026-30951
 Sequelize is a Node.js ORM tool. Prior to 6.37.8, there is SQL injection via unescaped cast type in JSON/JSONB where clause processing. The _traverseJSON() function splits JSON path keys on :: to extract a cast type, which is interpolated raw into CAST(... AS type) SQL. An attacker who controls JSON object keys can inject arbitrary SQL and exfiltrate data from any table. This vulnerability is fixed in 6.37.8.

- [https://github.com/EQSTLab/CVE-2026-30951](https://github.com/EQSTLab/CVE-2026-30951) :  ![starts](https://img.shields.io/github/stars/EQSTLab/CVE-2026-30951.svg) ![forks](https://img.shields.io/github/forks/EQSTLab/CVE-2026-30951.svg)


## CVE-2026-28363
 In OpenClaw before 2026.2.23, tools.exec.safeBins validation for sort could be bypassed via GNU long-option abbreviations (such as --compress-prog) in allowlist mode, leading to approval-free execution paths that were intended to require approval. Only an exact string such as --compress-program was denied.

- [https://github.com/kaleth4/CVE-2026-28363](https://github.com/kaleth4/CVE-2026-28363) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-28363.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-28363.svg)


## CVE-2026-28286
 ZimaOS is a fork of CasaOS, an operating system for Zima devices and x86-64 systems with UEFI. In version 1.5.2-beta3, the application enforces restrictions in the frontend/UI to prevent users from creating files or folders in internal OS paths. However, when interacting directly with the API, the restrictions are bypass-able. By sending a crafted request targeting paths like /etc, /usr, or other sensitive system directories, the API successfully creates files or directories in locations where normal users should have no write access. This indicates that the API does not properly validate the target path, allowing unauthorized operations on critical system directories. No known patch is publicly available.

- [https://github.com/Rushi9/zimaos-cve-2026-28286-arbitrary-file-write](https://github.com/Rushi9/zimaos-cve-2026-28286-arbitrary-file-write) :  ![starts](https://img.shields.io/github/stars/Rushi9/zimaos-cve-2026-28286-arbitrary-file-write.svg) ![forks](https://img.shields.io/github/forks/Rushi9/zimaos-cve-2026-28286-arbitrary-file-write.svg)


## CVE-2026-25769
 Wazuh is a free and open source platform used for threat prevention, detection, and response. Versions 4.0.0 through 4.14.2 have a Remote Code Execution (RCE) vulnerability due to Deserialization of Untrusted Data). All Wazuh deployments using cluster mode (master/worker architecture) and any organization with a compromised worker node (e.g., through initial access, insider threat, or supply chain attack) are impacted. An attacker who gains access to a worker node (through any means) can achieve full RCE on the master node with root privileges. Version 4.14.3 fixes the issue.

- [https://github.com/njeru-codes/CVE-2026-25769](https://github.com/njeru-codes/CVE-2026-25769) :  ![starts](https://img.shields.io/github/stars/njeru-codes/CVE-2026-25769.svg) ![forks](https://img.shields.io/github/forks/njeru-codes/CVE-2026-25769.svg)


## CVE-2026-24061
 telnetd in GNU Inetutils through 2.7 allows remote authentication bypass via a "-f root" value for the USER environment variable.

- [https://github.com/Risma2025/CVE-2026-24061-GNU-InetUtils-telnetd-Authentication-Bypass-Vulnerability](https://github.com/Risma2025/CVE-2026-24061-GNU-InetUtils-telnetd-Authentication-Bypass-Vulnerability) :  ![starts](https://img.shields.io/github/stars/Risma2025/CVE-2026-24061-GNU-InetUtils-telnetd-Authentication-Bypass-Vulnerability.svg) ![forks](https://img.shields.io/github/forks/Risma2025/CVE-2026-24061-GNU-InetUtils-telnetd-Authentication-Bypass-Vulnerability.svg)


## CVE-2026-23398
perform strict tag validation.

- [https://github.com/JohannesLks/CVE-2026-23398](https://github.com/JohannesLks/CVE-2026-23398) :  ![starts](https://img.shields.io/github/stars/JohannesLks/CVE-2026-23398.svg) ![forks](https://img.shields.io/github/forks/JohannesLks/CVE-2026-23398.svg)


## CVE-2026-22557
 A malicious actor with access to the network could exploit a Path Traversal vulnerability found in the UniFi Network Application to access files on the underlying system that could be manipulated to access an underlying account.

- [https://github.com/0xBlackash/CVE-2026-22557](https://github.com/0xBlackash/CVE-2026-22557) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-22557.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-22557.svg)


## CVE-2026-2992
 The KiviCare – Clinic & Patient Management System (EHR) plugin for WordPress is vulnerable to Privilege Escalation due to missing authorization on the `/wp-json/kivicare/v1/setup-wizard/clinic` REST API endpoint in all versions up to, and including, 4.1.2. This makes it possible for unauthenticated attackers to create a new clinic and a WordPress user with clinic admin privileges.

- [https://github.com/Smarttfoxx/CVE-2026-29923](https://github.com/Smarttfoxx/CVE-2026-29923) :  ![starts](https://img.shields.io/github/stars/Smarttfoxx/CVE-2026-29923.svg) ![forks](https://img.shields.io/github/forks/Smarttfoxx/CVE-2026-29923.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)
- [https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478](https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478) :  ![starts](https://img.shields.io/github/stars/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg) ![forks](https://img.shields.io/github/forks/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/enochgitgamefied/NextJS-CVE-2025-29927](https://github.com/enochgitgamefied/NextJS-CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/enochgitgamefied/NextJS-CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/enochgitgamefied/NextJS-CVE-2025-29927.svg)


## CVE-2025-20282
This vulnerability is due a lack of file validation checks that would prevent uploaded files from being placed in privileged directories on an affected system. An attacker could exploit this vulnerability by uploading a crafted file to the affected device. A successful exploit could allow the attacker to store malicious files on the affected system and then execute arbitrary code or obtain root privileges on the system.

- [https://github.com/pwnc4t/cve-2025-20282](https://github.com/pwnc4t/cve-2025-20282) :  ![starts](https://img.shields.io/github/stars/pwnc4t/cve-2025-20282.svg) ![forks](https://img.shields.io/github/forks/pwnc4t/cve-2025-20282.svg)


## CVE-2025-1739
 An Authentication Bypass vulnerability has been found in Trivision Camera NC227WF v5.8.0 from TrivisionSecurity. This vulnerability allows an attacker to retrieve administrator's credentials in cleartext by sending a request against the server using curl with random credentials to "/en/player/activex_pal.asp" and successfully authenticating the application.

- [https://github.com/n0n4m3x41/CVE-2025-1739](https://github.com/n0n4m3x41/CVE-2025-1739) :  ![starts](https://img.shields.io/github/stars/n0n4m3x41/CVE-2025-1739.svg) ![forks](https://img.shields.io/github/forks/n0n4m3x41/CVE-2025-1739.svg)


## CVE-2025-1738
 A Password Transmitted over Query String vulnerability has been found in Trivision Camera NC227WF v5.8.0 from TrivisionSecurity, exposing this sensitive information to a third party.

- [https://github.com/n0n4m3x41/CVE-2025-1738](https://github.com/n0n4m3x41/CVE-2025-1738) :  ![starts](https://img.shields.io/github/stars/n0n4m3x41/CVE-2025-1738.svg) ![forks](https://img.shields.io/github/forks/n0n4m3x41/CVE-2025-1738.svg)


## CVE-2024-45496
 A flaw was found in OpenShift. This issue occurs due to the misuse of elevated privileges in the OpenShift Container Platform's build process. During the build initialization step, the git-clone container is run with a privileged security context, allowing unrestricted access to the node. An attacker with developer-level access can provide a crafted .gitconfig file containing commands executed during the cloning process, leading to arbitrary command execution on the worker node. An attacker running code in a privileged container could escalate their permissions on the node running the container.

- [https://github.com/pwnc4t/cve-2024-45496](https://github.com/pwnc4t/cve-2024-45496) :  ![starts](https://img.shields.io/github/stars/pwnc4t/cve-2024-45496.svg) ![forks](https://img.shields.io/github/forks/pwnc4t/cve-2024-45496.svg)


## CVE-2024-24488
 An issue in Shenzen Tenda Technology CP3V2.0 V11.10.00.2311090948 allows a local attacker to obtain sensitive information via the password component.

- [https://github.com/legacyobj/CVE-2024-24488](https://github.com/legacyobj/CVE-2024-24488) :  ![starts](https://img.shields.io/github/stars/legacyobj/CVE-2024-24488.svg) ![forks](https://img.shields.io/github/forks/legacyobj/CVE-2024-24488.svg)


## CVE-2024-7387
 A flaw was found in openshift/builder. This vulnerability allows command injection via path traversal, where a malicious user can execute arbitrary commands on the OpenShift node running the builder container. When using the “Docker” strategy, executable files inside the privileged build container can be overridden using the `spec.source.secrets.secret.destinationDir` attribute of the `BuildConfig` definition. An attacker running code in a privileged container could escalate their permissions on the node running the container.

- [https://github.com/pwnc4t/cve-2024-7387](https://github.com/pwnc4t/cve-2024-7387) :  ![starts](https://img.shields.io/github/stars/pwnc4t/cve-2024-7387.svg) ![forks](https://img.shields.io/github/forks/pwnc4t/cve-2024-7387.svg)


## CVE-2024-6387
 A security regression (CVE-2006-5051) was discovered in OpenSSH's server (sshd). There is a race condition which can lead sshd to handle some signals in an unsafe manner. An unauthenticated, remote attacker may be able to trigger it by failing to authenticate within a set time period.

- [https://github.com/particle99/CVE-2024-6387-POC](https://github.com/particle99/CVE-2024-6387-POC) :  ![starts](https://img.shields.io/github/stars/particle99/CVE-2024-6387-POC.svg) ![forks](https://img.shields.io/github/forks/particle99/CVE-2024-6387-POC.svg)


## CVE-2024-2370
 DO NOT USE THIS CVE ID NUMBER. Consult IDs: CVE-2018-5341. Reason: This CVE Record is a duplicate of CVE-2018-5341. Notes: All CVE users should reference CVE-2018-5341 instead of this record.

- [https://github.com/vinh0212/CVE-2024-23700](https://github.com/vinh0212/CVE-2024-23700) :  ![starts](https://img.shields.io/github/stars/vinh0212/CVE-2024-23700.svg) ![forks](https://img.shields.io/github/forks/vinh0212/CVE-2024-23700.svg)


## CVE-2023-27524
Alternatively you can set it with `SUPERSET_SECRET_KEY` environment variable.

- [https://github.com/rachidafaf/bola-CVE-2023-27524](https://github.com/rachidafaf/bola-CVE-2023-27524) :  ![starts](https://img.shields.io/github/stars/rachidafaf/bola-CVE-2023-27524.svg) ![forks](https://img.shields.io/github/forks/rachidafaf/bola-CVE-2023-27524.svg)


## CVE-2023-25690
Request splitting/smuggling could result in bypass of access controls in the proxy server, proxying unintended URLs to existing origin servers, and cache poisoning. Users are recommended to update to at least version 2.4.56 of Apache HTTP Server.

- [https://github.com/arnavps/CTF-Web-Exploitation](https://github.com/arnavps/CTF-Web-Exploitation) :  ![starts](https://img.shields.io/github/stars/arnavps/CTF-Web-Exploitation.svg) ![forks](https://img.shields.io/github/forks/arnavps/CTF-Web-Exploitation.svg)


## CVE-2021-3129
 Ignition before 2.5.2, as used in Laravel and other products, allows unauthenticated remote attackers to execute arbitrary code because of insecure usage of file_get_contents() and file_put_contents(). This is exploitable on sites using debug mode with Laravel before 8.4.2.

- [https://github.com/Nullsecur1ty/CVE-2021-3129](https://github.com/Nullsecur1ty/CVE-2021-3129) :  ![starts](https://img.shields.io/github/stars/Nullsecur1ty/CVE-2021-3129.svg) ![forks](https://img.shields.io/github/forks/Nullsecur1ty/CVE-2021-3129.svg)

