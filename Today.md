# Update 2026-04-21
## CVE-2026-35616
 A improper access control vulnerability in Fortinet FortiClientEMS 7.4.5 through 7.4.6 may allow an unauthenticated attacker to execute unauthorized code or commands via crafted requests.

- [https://github.com/Alaatk/CVE-2026-35616](https://github.com/Alaatk/CVE-2026-35616) :  ![starts](https://img.shields.io/github/stars/Alaatk/CVE-2026-35616.svg) ![forks](https://img.shields.io/github/forks/Alaatk/CVE-2026-35616.svg)


## CVE-2026-35584
 FreeScout is a free help desk and shared inbox built with PHP's Laravel framework. Prior to 1.8.212, the endpoint GET /thread/read/{conversation_id}/{thread_id} does not require authentication and does not validate whether the given thread_id belongs to the given conversation_id. This allows any unauthenticated attacker to mark any thread as read by passing arbitrary IDs, enumerate valid thread IDs via HTTP response codes (200 vs 404), and manipulate opened_at timestamps across conversations (IDOR). This vulnerability is fixed in 1.8.212.

- [https://github.com/NovaisLeonardo/CVE-2026-35584](https://github.com/NovaisLeonardo/CVE-2026-35584) :  ![starts](https://img.shields.io/github/stars/NovaisLeonardo/CVE-2026-35584.svg) ![forks](https://img.shields.io/github/forks/NovaisLeonardo/CVE-2026-35584.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/0xBlackash/CVE-2026-33017](https://github.com/0xBlackash/CVE-2026-33017) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-33017.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-33017.svg)


## CVE-2026-31908
Users are recommended to upgrade to version 3.16.0, which fixes the issue.

- [https://github.com/MehranTurk/CVE-2026-31908](https://github.com/MehranTurk/CVE-2026-31908) :  ![starts](https://img.shields.io/github/stars/MehranTurk/CVE-2026-31908.svg) ![forks](https://img.shields.io/github/forks/MehranTurk/CVE-2026-31908.svg)


## CVE-2026-27597
 Enclave is a secure JavaScript sandbox designed for safe AI agent code execution. Prior to version 2.11.1, it is possible to escape the security boundraries set by `@enclave-vm/core`, which can be used to achieve remote code execution (RCE). The issue has been fixed in version 2.11.1.

- [https://github.com/NetVanguard-cmd/CVE-2026-27597](https://github.com/NetVanguard-cmd/CVE-2026-27597) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2026-27597.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2026-27597.svg)


## CVE-2026-27507
 Binardat 10G08-0800GSM network switch firmware version V300SP10260209 and prior contain hard-coded administrative credentials that cannot be changed by users. Knowledge of these credentials allows full administrative access to the device.

- [https://github.com/NetVanguard-cmd/CVE-2026-27507](https://github.com/NetVanguard-cmd/CVE-2026-27507) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2026-27507.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2026-27507.svg)


## CVE-2026-26198
 Ormar is a async mini ORM for Python. In versions 0.9.9 through 0.22.0, when performing aggregate queries, Ormar ORM constructs SQL expressions by passing user-supplied column names directly into `sqlalchemy.text()` without any validation or sanitization. The `min()` and `max()` methods in the `QuerySet` class accept arbitrary string input as the column parameter. While `sum()` and `avg()` are partially protected by an `is_numeric` type check that rejects non-existent fields, `min()` and `max()` skip this validation entirely. As a result, an attacker-controlled string is embedded as raw SQL inside the aggregate function call. Any unauthorized user can exploit this vulnerability to read the entire database contents, including tables unrelated to the queried model, by injecting a subquery as the column parameter. Version 0.23.0 contains a patch.

- [https://github.com/NetVanguard-cmd/CVE-2026-26198](https://github.com/NetVanguard-cmd/CVE-2026-26198) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2026-26198.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2026-26198.svg)


## CVE-2026-5194
 Missing hash/digest size and OID checks allow digests smaller than allowed when verifying ECDSA certificates, or smaller than is appropriate for the relevant key type, to be accepted by signature verification functions. This could lead to reduced security of ECDSA certificate-based authentication if the public CA key used is also known. This affects ECDSA/ECC verification when EdDSA or ML-DSA is also enabled.

- [https://github.com/jenniferreire26/CVE-2026-5194](https://github.com/jenniferreire26/CVE-2026-5194) :  ![starts](https://img.shields.io/github/stars/jenniferreire26/CVE-2026-5194.svg) ![forks](https://img.shields.io/github/forks/jenniferreire26/CVE-2026-5194.svg)


## CVE-2026-4447
 Inappropriate implementation in V8 in Google Chrome prior to 146.0.7680.153 allowed a remote attacker to execute arbitrary code inside a sandbox via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/NetVanguard-cmd/CVE-2026-4447](https://github.com/NetVanguard-cmd/CVE-2026-4447) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2026-4447.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2026-4447.svg)


## CVE-2026-3055
 Insufficient input validation in NetScaler ADC and NetScaler Gateway when configured as a SAML IDP leading to memory overread

- [https://github.com/NetVanguard-cmd/CVE-2026-3055](https://github.com/NetVanguard-cmd/CVE-2026-3055) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2026-3055.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2026-3055.svg)


## CVE-2026-0745
 The User Language Switch plugin for WordPress is vulnerable to Server-Side Request Forgery in all versions up to, and including, 1.6.10 due to missing URL validation on the 'download_language()' function. This makes it possible for authenticated attackers, with Administrator-level access and above, to make web requests to arbitrary locations originating from the web application and can be used to query and modify information from internal services.

- [https://github.com/NetVanguard-cmd/CVE-2026-0745](https://github.com/NetVanguard-cmd/CVE-2026-0745) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2026-0745.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2026-0745.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-61882
 Vulnerability in the Oracle Concurrent Processing product of Oracle E-Business Suite (component: BI Publisher Integration).  Supported versions that are affected are 12.2.3-12.2.14. Easily exploitable vulnerability allows unauthenticated attacker with network access via HTTP to compromise Oracle Concurrent Processing.  Successful attacks of this vulnerability can result in takeover of Oracle Concurrent Processing. CVSS 3.1 Base Score 9.8 (Confidentiality, Integrity and Availability impacts).  CVSS Vector: (CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H).

- [https://github.com/NetVanguard-cmd/CVE-2025-61882](https://github.com/NetVanguard-cmd/CVE-2025-61882) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2025-61882.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2025-61882.svg)


## CVE-2025-59536
 Claude Code is an agentic coding tool. Versions before 1.0.111 were vulnerable to Code Injection due to a bug in the startup trust dialog implementation. Claude Code could be tricked to execute code contained in a project before the user accepted the startup trust dialog. Exploiting this requires a user to start Claude Code in an untrusted directory. Users on standard Claude Code auto-update will have received this fix automatically. Users performing manual updates are advised to update to the latest version. This issue is fixed in version 1.0.111.

- [https://github.com/NetVanguard-cmd/CVE-2025-59536](https://github.com/NetVanguard-cmd/CVE-2025-59536) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2025-59536.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2025-59536.svg)


## CVE-2025-55315
 Inconsistent interpretation of http requests ('http request/response smuggling') in ASP.NET Core allows an authorized attacker to bypass a security feature over a network.

- [https://github.com/NetVanguard-cmd/CVE-2025-55315](https://github.com/NetVanguard-cmd/CVE-2025-55315) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2025-55315.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2025-55315.svg)


## CVE-2025-11832
 Allocation of Resources Without Limits or Throttling vulnerability in Azure Access Technology BLU-IC2, Azure Access Technology BLU-IC4 allows Flooding.This issue affects BLU-IC2: through 1.19.5; BLU-IC4: through 1.19.5.

- [https://github.com/NetVanguard-cmd/CVE-2025-11832](https://github.com/NetVanguard-cmd/CVE-2025-11832) :  ![starts](https://img.shields.io/github/stars/NetVanguard-cmd/CVE-2025-11832.svg) ![forks](https://img.shields.io/github/forks/NetVanguard-cmd/CVE-2025-11832.svg)


## CVE-2025-2304
When a user wishes to change his password, the 'updated_ajax' method of the UsersController is called. The vulnerability stems from the use of the dangerous permit! method, which allows all parameters to pass through without any filtering.

- [https://github.com/mattiapertusati/htb-facts](https://github.com/mattiapertusati/htb-facts) :  ![starts](https://img.shields.io/github/stars/mattiapertusati/htb-facts.svg) ![forks](https://img.shields.io/github/forks/mattiapertusati/htb-facts.svg)


## CVE-2024-50379
Users are recommended to upgrade to version 11.0.2, 10.1.34 or 9.0.98, which fixes the issue.

- [https://github.com/Lux-J/CVE-2024-50379-exp](https://github.com/Lux-J/CVE-2024-50379-exp) :  ![starts](https://img.shields.io/github/stars/Lux-J/CVE-2024-50379-exp.svg) ![forks](https://img.shields.io/github/forks/Lux-J/CVE-2024-50379-exp.svg)


## CVE-2024-32114
Or we encourage users to upgrade to Apache ActiveMQ 6.1.2 where the default configuration has been updated with authentication by default.

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2024-28397
 An issue in the component js2py.disable_pyimport() of js2py up to v0.74 allows attackers to execute arbitrary code via a crafted API call.

- [https://github.com/s0m1s0ng/CVE-2024-28397-Reverse-Shell](https://github.com/s0m1s0ng/CVE-2024-28397-Reverse-Shell) :  ![starts](https://img.shields.io/github/stars/s0m1s0ng/CVE-2024-28397-Reverse-Shell.svg) ![forks](https://img.shields.io/github/forks/s0m1s0ng/CVE-2024-28397-Reverse-Shell.svg)


## CVE-2024-3400
Cloud NGFW, Panorama appliances, and Prisma Access are not impacted by this vulnerability.

- [https://github.com/wa6n3r/CVE-2024-3400](https://github.com/wa6n3r/CVE-2024-3400) :  ![starts](https://img.shields.io/github/stars/wa6n3r/CVE-2024-3400.svg) ![forks](https://img.shields.io/github/forks/wa6n3r/CVE-2024-3400.svg)


## CVE-2023-46604
which fixes this issue.

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2023-45802
Users are recommended to upgrade to version 2.4.58, which fixes the issue.

- [https://github.com/MehranTurk/CVE-2023-45802](https://github.com/MehranTurk/CVE-2023-45802) :  ![starts](https://img.shields.io/github/stars/MehranTurk/CVE-2023-45802.svg) ![forks](https://img.shields.io/github/forks/MehranTurk/CVE-2023-45802.svg)


## CVE-2022-41678
A more restrictive Jolokia configuration has been defined in default ActiveMQ distribution. We encourage users to upgrade to ActiveMQ distributions version including updated Jolokia configuration: 5.16.6, 5.17.4, 5.18.0, 6.0.0.

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2022-39299
 Passport-SAML is a SAML 2.0 authentication provider for Passport, the Node.js authentication library. A remote attacker may be able to bypass SAML authentication on a website using passport-saml. A successful attack requires that the attacker is in possession of an arbitrary IDP signed XML element. Depending on the IDP used, fully unauthenticated attacks (e.g without access to a valid user) might also be feasible if generation of a signed message can be triggered. Users should upgrade to passport-saml version 3.2.2 or newer. The issue was also present in the beta releases of `node-saml` before version 4.0.0-beta.5. If you cannot upgrade, disabling SAML authentication may be done as a workaround.

- [https://github.com/KaztoRay/CVE-2022-39299-Research](https://github.com/KaztoRay/CVE-2022-39299-Research) :  ![starts](https://img.shields.io/github/stars/KaztoRay/CVE-2022-39299-Research.svg) ![forks](https://img.shields.io/github/forks/KaztoRay/CVE-2022-39299-Research.svg)


## CVE-2022-0847
 A flaw was found in the way the "flags" member of the new pipe buffer structure was lacking proper initialization in copy_page_to_iter_pipe and push_pipe functions in the Linux kernel and could thus contain stale values. An unprivileged local user could use this flaw to write to pages in the page cache backed by read only files and as such escalate their privileges on the system.

- [https://github.com/AyoubNajim/cve-2022-0847dirtypipe-exploit](https://github.com/AyoubNajim/cve-2022-0847dirtypipe-exploit) :  ![starts](https://img.shields.io/github/stars/AyoubNajim/cve-2022-0847dirtypipe-exploit.svg) ![forks](https://img.shields.io/github/forks/AyoubNajim/cve-2022-0847dirtypipe-exploit.svg)


## CVE-2021-3560
 It was found that polkit could be tricked into bypassing the credential checks for D-Bus requests, elevating the privileges of the requestor to the root user. This flaw could be used by an unprivileged local attacker to, for example, create a new local administrator. The highest threat from this vulnerability is to data confidentiality and integrity as well as system availability.

- [https://github.com/Gerberayale521/pwnkit](https://github.com/Gerberayale521/pwnkit) :  ![starts](https://img.shields.io/github/stars/Gerberayale521/pwnkit.svg) ![forks](https://img.shields.io/github/forks/Gerberayale521/pwnkit.svg)


## CVE-2021-3493
 The overlayfs implementation in the linux kernel did not properly validate with respect to user namespaces the setting of file capabilities on files in an underlying file system. Due to the combination of unprivileged user namespaces along with a patch carried in the Ubuntu kernel to allow unprivileged overlay mounts, an attacker could use this to gain elevated privileges.

- [https://github.com/iqbalhussainas/OverlayFS-LPE-Exploit](https://github.com/iqbalhussainas/OverlayFS-LPE-Exploit) :  ![starts](https://img.shields.io/github/stars/iqbalhussainas/OverlayFS-LPE-Exploit.svg) ![forks](https://img.shields.io/github/forks/iqbalhussainas/OverlayFS-LPE-Exploit.svg)


## CVE-2017-0144
 The SMBv1 server in Microsoft Windows Vista SP2; Windows Server 2008 SP2 and R2 SP1; Windows 7 SP1; Windows 8.1; Windows Server 2012 Gold and R2; Windows RT 8.1; and Windows 10 Gold, 1511, and 1607; and Windows Server 2016 allows remote attackers to execute arbitrary code via crafted packets, aka "Windows SMB Remote Code Execution Vulnerability." This vulnerability is different from those described in CVE-2017-0143, CVE-2017-0145, CVE-2017-0146, and CVE-2017-0148.

- [https://github.com/klairmanraj/Multi-VLAN-Enterprise-Network-Security-Infrastructure](https://github.com/klairmanraj/Multi-VLAN-Enterprise-Network-Security-Infrastructure) :  ![starts](https://img.shields.io/github/stars/klairmanraj/Multi-VLAN-Enterprise-Network-Security-Infrastructure.svg) ![forks](https://img.shields.io/github/forks/klairmanraj/Multi-VLAN-Enterprise-Network-Security-Infrastructure.svg)
- [https://github.com/klairmanraj/Multi-VLAN-Enterprise-Network-Vulnerability-Assessment](https://github.com/klairmanraj/Multi-VLAN-Enterprise-Network-Vulnerability-Assessment) :  ![starts](https://img.shields.io/github/stars/klairmanraj/Multi-VLAN-Enterprise-Network-Vulnerability-Assessment.svg) ![forks](https://img.shields.io/github/forks/klairmanraj/Multi-VLAN-Enterprise-Network-Vulnerability-Assessment.svg)
- [https://github.com/klairmanraj/Vulnerability-Risk-Assessment-TVRA-Enterprise-Network](https://github.com/klairmanraj/Vulnerability-Risk-Assessment-TVRA-Enterprise-Network) :  ![starts](https://img.shields.io/github/stars/klairmanraj/Vulnerability-Risk-Assessment-TVRA-Enterprise-Network.svg) ![forks](https://img.shields.io/github/forks/klairmanraj/Vulnerability-Risk-Assessment-TVRA-Enterprise-Network.svg)


## CVE-2016-3088
 The Fileserver web application in Apache ActiveMQ 5.x before 5.14.0 allows remote attackers to upload and execute arbitrary files via an HTTP PUT followed by an HTTP MOVE request.

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2015-5254
 Apache ActiveMQ 5.x before 5.13.0 does not restrict the classes that can be serialized in the broker, which allows remote attackers to execute arbitrary code via a crafted serialized Java Message Service (JMS) ObjectMessage object.

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2007-4559
 Directory traversal vulnerability in the (1) extract and (2) extractall functions in the tarfile module in Python allows user-assisted remote attackers to overwrite arbitrary files via a .. (dot dot) sequence in filenames in a TAR archive, a related issue to CVE-2001-1267.

- [https://github.com/jithinodattu/CVE-2007-4559-lab](https://github.com/jithinodattu/CVE-2007-4559-lab) :  ![starts](https://img.shields.io/github/stars/jithinodattu/CVE-2007-4559-lab.svg) ![forks](https://img.shields.io/github/forks/jithinodattu/CVE-2007-4559-lab.svg)

