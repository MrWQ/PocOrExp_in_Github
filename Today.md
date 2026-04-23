# Update 2026-04-23
## CVE-2026-39866
 Lawnchair is a free, open-source home app for Android. Prior to commit fcba413f55dd47f8a3921445252849126c6266b2, command injection in release_update.yml workflow dispatch input allows arbitrary code execution. Commit fcba413f55dd47f8a3921445252849126c6266b2 patches the issue.

- [https://github.com/abhayclasher/CVE-2026-39866](https://github.com/abhayclasher/CVE-2026-39866) :  ![starts](https://img.shields.io/github/stars/abhayclasher/CVE-2026-39866.svg) ![forks](https://img.shields.io/github/forks/abhayclasher/CVE-2026-39866.svg)


## CVE-2026-39808
 A improper neutralization of special elements used in an os command ('os command injection') vulnerability in Fortinet FortiSandbox 4.4.0 through 4.4.8 may allow attacker to execute unauthorized code or commands via insert attack vector here

- [https://github.com/ynsmroztas/FortiSandbox-RCE-Exploit-CVE-2026-39808](https://github.com/ynsmroztas/FortiSandbox-RCE-Exploit-CVE-2026-39808) :  ![starts](https://img.shields.io/github/stars/ynsmroztas/FortiSandbox-RCE-Exploit-CVE-2026-39808.svg) ![forks](https://img.shields.io/github/forks/ynsmroztas/FortiSandbox-RCE-Exploit-CVE-2026-39808.svg)


## CVE-2026-37748
 Visitor Management System 1.0 by sanjay1313 is vulnerable to Unrestricted File Upload in vms/php/admin_user_insert.php and vms/php/update_1.php. The move_uploaded_file() function is called without any MIME type, extension, or content validation, allowing an authenticated admin to upload a PHP webshell and achieve Remote Code Execution on the server.

- [https://github.com/menevarad007/CVE-2026-37748](https://github.com/menevarad007/CVE-2026-37748) :  ![starts](https://img.shields.io/github/stars/menevarad007/CVE-2026-37748.svg) ![forks](https://img.shields.io/github/forks/menevarad007/CVE-2026-37748.svg)


## CVE-2026-35584
 FreeScout is a free help desk and shared inbox built with PHP's Laravel framework. Prior to 1.8.212, the endpoint GET /thread/read/{conversation_id}/{thread_id} does not require authentication and does not validate whether the given thread_id belongs to the given conversation_id. This allows any unauthenticated attacker to mark any thread as read by passing arbitrary IDs, enumerate valid thread IDs via HTTP response codes (200 vs 404), and manipulate opened_at timestamps across conversations (IDOR). This vulnerability is fixed in 1.8.212.

- [https://github.com/LeonardoNovais7/CVE-2026-35584](https://github.com/LeonardoNovais7/CVE-2026-35584) :  ![starts](https://img.shields.io/github/stars/LeonardoNovais7/CVE-2026-35584.svg) ![forks](https://img.shields.io/github/forks/LeonardoNovais7/CVE-2026-35584.svg)


## CVE-2026-33824
 Double free in Windows IKE Extension allows an unauthorized attacker to execute code over a network.

- [https://github.com/kaleth4/CVE-2026-33824](https://github.com/kaleth4/CVE-2026-33824) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-33824.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-33824.svg)


## CVE-2026-32613
 Spinnaker is an open source, multi-cloud continuous delivery platform. Echo like some other services, uses SPeL (Spring Expression Language) to process information - specifically around expected artifacts. In versions prior to 2026.1.0, 2026.0.1, 2025.4.2, and 2025.3.2, unlike orca, it was NOT restricting that context to a set of trusted classes, but allowing FULL JVM access. This enabled a user to use arbitrary java classes which allow deep access to the system. This enabled the ability to invoke commands, access files, etc. Versions 2026.1.0, 2026.0.1, 2025.4.2, and 2025.3.2 contain a patch. As a workaround, disable echo entirely.

- [https://github.com/ZeroPathAI/spinnaker-poc](https://github.com/ZeroPathAI/spinnaker-poc) :  ![starts](https://img.shields.io/github/stars/ZeroPathAI/spinnaker-poc.svg) ![forks](https://img.shields.io/github/forks/ZeroPathAI/spinnaker-poc.svg)


## CVE-2026-32604
 Spinnaker is an open source, multi-cloud continuous delivery platform. In versions prior to 2026.1.0, 2026.0.1, 2025.4.2, and 2025.3.2, a bad actor can execute arbitrary commands very simply on the clouddriver pods. This can expose credentials, remove files, or inject resources easily. Versions 2026.1.0, 2026.0.1, 2025.4.2, and 2025.3.2 contain a patch. As a workaround, disable the gitrepo artifact types.

- [https://github.com/ZeroPathAI/spinnaker-poc](https://github.com/ZeroPathAI/spinnaker-poc) :  ![starts](https://img.shields.io/github/stars/ZeroPathAI/spinnaker-poc.svg) ![forks](https://img.shields.io/github/forks/ZeroPathAI/spinnaker-poc.svg)


## CVE-2026-29053
 Ghost is a Node.js content management system. From version 0.7.2 to 6.19.0, specifically crafted malicious themes can execute arbitrary code on the server running Ghost. This issue has been patched in version 6.19.1.

- [https://github.com/AC8999/CVE-2026-29053](https://github.com/AC8999/CVE-2026-29053) :  ![starts](https://img.shields.io/github/stars/AC8999/CVE-2026-29053.svg) ![forks](https://img.shields.io/github/forks/AC8999/CVE-2026-29053.svg)


## CVE-2026-25049
 n8n is an open source workflow automation platform. Prior to versions 1.123.17 and 2.5.2, an authenticated user with permission to create or modify workflows could abuse crafted expressions in workflow parameters to trigger unintended system command execution on the host running n8n. This issue has been patched in versions 1.123.17 and 2.5.2.

- [https://github.com/0xBlackash/CVE-2026-25049](https://github.com/0xBlackash/CVE-2026-25049) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-25049.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-25049.svg)


## CVE-2026-20180
This vulnerability is due to insufficient validation of user-supplied input. An attacker could exploit this vulnerability by sending a crafted HTTP request to an affected device. A successful exploit could allow the attacker to obtain user-level access to the underlying operating system and then elevate privileges to&nbsp;root. In single-node ISE deployments, successful exploitation of these vulnerabilities could cause the affected ISE node to become unavailable, resulting in a denial of service (DoS) condition. In that condition, endpoints that have not already authenticated would be unable to access the network until the node is restored.

- [https://github.com/kaleth4/CVE-2026-20180](https://github.com/kaleth4/CVE-2026-20180) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-20180.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-20180.svg)


## CVE-2026-4821
 An improper neutralization of special elements vulnerability was identified in GitHub Enterprise Server that allowed an authenticated Management Console administrator to execute arbitrary OS commands via shell metacharacter injection in proxy configuration fields such as http_proxy. Exploitation of this vulnerability required access to the GitHub Enterprise Server instance and administrator privileges to the Management Console. This vulnerability affected all versions of GitHub Enterprise Server prior to 3.21 and was fixed in versions 3.20.1, 3.19.5, 3.18.8, 3.17.14, 3.16.17, 3.15.21, 3.14.26. This vulnerability was reported via the GitHub Bug Bounty program.

- [https://github.com/openexecution-coder/demo-cve-2026-4821](https://github.com/openexecution-coder/demo-cve-2026-4821) :  ![starts](https://img.shields.io/github/stars/openexecution-coder/demo-cve-2026-4821.svg) ![forks](https://img.shields.io/github/forks/openexecution-coder/demo-cve-2026-4821.svg)


## CVE-2026-3126
 This CVE ID has been rejected or withdrawn by its CVE Numbering Authority.

- [https://github.com/0xrixet/Craftcms-PoC-CVE-2026-31266](https://github.com/0xrixet/Craftcms-PoC-CVE-2026-31266) :  ![starts](https://img.shields.io/github/stars/0xrixet/Craftcms-PoC-CVE-2026-31266.svg) ![forks](https://img.shields.io/github/forks/0xrixet/Craftcms-PoC-CVE-2026-31266.svg)


## CVE-2026-2754
 Navtor NavBox exposes sensitive configuration and operational data due to missing authentication on HTTP API endpoints. An unauthenticated remote attacker with network access to the device can execute HTTP GET requests to TCP port 8080 to retrieve internal network parameters including ECDIS & OT Information, device identifiers, and service status logs.

- [https://github.com/PegasusMetaSec/Pegasus-CVE-2026-2754-Framework-](https://github.com/PegasusMetaSec/Pegasus-CVE-2026-2754-Framework-) :  ![starts](https://img.shields.io/github/stars/PegasusMetaSec/Pegasus-CVE-2026-2754-Framework-.svg) ![forks](https://img.shields.io/github/forks/PegasusMetaSec/Pegasus-CVE-2026-2754-Framework-.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-alias.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-tilde.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-zero-installs.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-realworld-calcom-yarn-monorepo.svg)


## CVE-2025-55182
 A pre-authentication remote code execution vulnerability exists in React Server Components versions 19.0.0, 19.1.0, 19.1.1, and 19.2.0 including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints.

- [https://github.com/CirqueiraDev/MassExploit-CVE-2025-55182](https://github.com/CirqueiraDev/MassExploit-CVE-2025-55182) :  ![starts](https://img.shields.io/github/stars/CirqueiraDev/MassExploit-CVE-2025-55182.svg) ![forks](https://img.shields.io/github/forks/CirqueiraDev/MassExploit-CVE-2025-55182.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/elshaheedy/CVE-2025-29927-Sigma-Rule](https://github.com/elshaheedy/CVE-2025-29927-Sigma-Rule) :  ![starts](https://img.shields.io/github/stars/elshaheedy/CVE-2025-29927-Sigma-Rule.svg) ![forks](https://img.shields.io/github/forks/elshaheedy/CVE-2025-29927-Sigma-Rule.svg)
- [https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927](https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/sn1p3rt3s7/NextJS_CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/sn1p3rt3s7/NextJS_CVE-2025-29927.svg)


## CVE-2024-25600
 Improper Control of Generation of Code ('Code Injection') vulnerability in Codeer Limited Bricks Builder allows Code Injection.This issue affects Bricks Builder: from n/a through 1.9.6.

- [https://github.com/w666-glitch/CVE-2024-25600](https://github.com/w666-glitch/CVE-2024-25600) :  ![starts](https://img.shields.io/github/stars/w666-glitch/CVE-2024-25600.svg) ![forks](https://img.shields.io/github/forks/w666-glitch/CVE-2024-25600.svg)


## CVE-2024-7928
 A vulnerability, which was classified as problematic, has been found in FastAdmin up to 1.3.3.20220121. Affected by this issue is some unknown functionality of the file /index/ajax/lang. The manipulation of the argument lang leads to path traversal. The attack may be launched remotely. The exploit has been disclosed to the public and may be used. Upgrading to version 1.3.4.20220530 is able to address this issue. It is recommended to upgrade the affected component.

- [https://github.com/w666-glitch/CVE-2024-7928](https://github.com/w666-glitch/CVE-2024-7928) :  ![starts](https://img.shields.io/github/stars/w666-glitch/CVE-2024-7928.svg) ![forks](https://img.shields.io/github/forks/w666-glitch/CVE-2024-7928.svg)


## CVE-2024-4663
 The OSM Map Widget for Elementor plugin for WordPress is vulnerable to Reflected Cross-Site Scripting via the ‘id’ parameter in all versions up to, and including, 1.2.2 due to insufficient input sanitization and output escaping. This makes it possible for unauthenticated attackers to inject arbitrary web scripts in pages that execute if they can successfully trick a user into performing an action such as clicking on a link.

- [https://github.com/NU1L0/CVE-2024-46636-SQLi-MODAPS](https://github.com/NU1L0/CVE-2024-46636-SQLi-MODAPS) :  ![starts](https://img.shields.io/github/stars/NU1L0/CVE-2024-46636-SQLi-MODAPS.svg) ![forks](https://img.shields.io/github/forks/NU1L0/CVE-2024-46636-SQLi-MODAPS.svg)


## CVE-2024-4577
 In PHP versions 8.1.* before 8.1.29, 8.2.* before 8.2.20, 8.3.* before 8.3.8, when using Apache and PHP-CGI on Windows, if the system is set up to use certain code pages, Windows may use "Best-Fit" behavior to replace characters in command line given to Win32 API functions. PHP CGI module may misinterpret those characters as PHP options, which may allow a malicious user to pass options to PHP binary being run, and thus reveal the source code of scripts, run arbitrary PHP code on the server, etc.

- [https://github.com/CirqueiraDev/MassExploit-CVE-2024-4577](https://github.com/CirqueiraDev/MassExploit-CVE-2024-4577) :  ![starts](https://img.shields.io/github/stars/CirqueiraDev/MassExploit-CVE-2024-4577.svg) ![forks](https://img.shields.io/github/forks/CirqueiraDev/MassExploit-CVE-2024-4577.svg)


## CVE-2024-2997
 A vulnerability was found in Bdtask Multi-Store Inventory Management System up to 20240320. It has been declared as problematic. Affected by this vulnerability is an unknown functionality. The manipulation of the argument Category Name/Model Name/Brand Name/Unit Name leads to cross site scripting. The attack can be launched remotely. The exploit has been disclosed to the public and may be used. The associated identifier of this vulnerability is VDB-258199. NOTE: The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/o9-9/CVE-2024-2997](https://github.com/o9-9/CVE-2024-2997) :  ![starts](https://img.shields.io/github/stars/o9-9/CVE-2024-2997.svg) ![forks](https://img.shields.io/github/forks/o9-9/CVE-2024-2997.svg)


## CVE-2024-1086
We recommend upgrading past commit f342de4e2f33e0e39165d8639387aa6c19dff660.

- [https://github.com/ClaraSto/CVE-2024-1086_Ausarbeitung](https://github.com/ClaraSto/CVE-2024-1086_Ausarbeitung) :  ![starts](https://img.shields.io/github/stars/ClaraSto/CVE-2024-1086_Ausarbeitung.svg) ![forks](https://img.shields.io/github/forks/ClaraSto/CVE-2024-1086_Ausarbeitung.svg)


## CVE-2023-46604
which fixes this issue.

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2023-45648
Users are recommended to upgrade to version 11.0.0-M12 onwards, 10.1.14 onwards, 9.0.81 onwards or 8.5.94 onwards, which fix the issue.

- [https://github.com/latr0phil/CVE-2023-45648-Hang-Check](https://github.com/latr0phil/CVE-2023-45648-Hang-Check) :  ![starts](https://img.shields.io/github/stars/latr0phil/CVE-2023-45648-Hang-Check.svg) ![forks](https://img.shields.io/github/forks/latr0phil/CVE-2023-45648-Hang-Check.svg)


## CVE-2023-20198
 Cisco is providing an update for the ongoing investigation into observed exploitation of the web UI feature in Cisco IOS XE Software. We are updating the list of fixed releases and adding the Software Checker. Our investigation has determined that the actors exploited two previously unknown issues. The attacker first exploited CVE-2023-20198 to gain initial access and issued a privilege 15 command to create a local user and password combination. This allowed the user to log in with normal user access. The attacker then exploited another component of the web UI feature, leveraging the new local user to elevate privilege to root and write the implant to the file system. Cisco has assigned CVE-2023-20273 to this issue. CVE-2023-20198 has been assigned a CVSS Score of 10.0. CVE-2023-20273 has been assigned a CVSS Score of 7.2. Both of these CVEs are being tracked by CSCwh87343.

- [https://github.com/DOMINIC471/qub-network-security-cve-2023-20198](https://github.com/DOMINIC471/qub-network-security-cve-2023-20198) :  ![starts](https://img.shields.io/github/stars/DOMINIC471/qub-network-security-cve-2023-20198.svg) ![forks](https://img.shields.io/github/forks/DOMINIC471/qub-network-security-cve-2023-20198.svg)


## CVE-2022-47102
 A cross-site scripting (XSS) vulnerability in Student Study Center Management System V 1.0 allows attackers to execute arbitrary web scripts or HTML via a crafted payload injected into the name parameter.

- [https://github.com/sudoninja-noob/CVE-2022-47102](https://github.com/sudoninja-noob/CVE-2022-47102) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-47102.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-47102.svg)


## CVE-2022-46623
 Judging Management System v1.0.0 was discovered to contain a SQL injection vulnerability via the username parameter.

- [https://github.com/sudoninja-noob/CVE-2022-46623](https://github.com/sudoninja-noob/CVE-2022-46623) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-46623.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-46623.svg)


## CVE-2022-46622
 A cross-site scripting (XSS) vulnerability in Judging Management System v1.0 allows attackers to execute arbitrary web scripts or HTML via a crafted payload injected into the firstname parameter.

- [https://github.com/sudoninja-noob/CVE-2022-46622](https://github.com/sudoninja-noob/CVE-2022-46622) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-46622.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-46622.svg)


## CVE-2022-45729
 A cross-site scripting (XSS) vulnerability in Doctor Appointment Management System v1.0.0 allows attackers to execute arbitrary web scripts or HTML via a crafted payload injected into the Employee ID parameter.

- [https://github.com/sudoninja-noob/CVE-2022-45729](https://github.com/sudoninja-noob/CVE-2022-45729) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-45729.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-45729.svg)


## CVE-2022-45728
 Doctor Appointment Management System v1.0.0 was discovered to contain a cross-site scripting (XSS) vulnerability.

- [https://github.com/sudoninja-noob/CVE-2022-45728](https://github.com/sudoninja-noob/CVE-2022-45728) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-45728.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-45728.svg)


## CVE-2022-45217
 A cross-site scripting (XSS) vulnerability in Book Store Management System v1.0.0 allows attackers to execute arbitrary web scripts or HTML via a crafted payload injected into the Level parameter under the Add New System User module.

- [https://github.com/sudoninja-noob/CVE-2022-45217](https://github.com/sudoninja-noob/CVE-2022-45217) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-45217.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-45217.svg)


## CVE-2022-43369
 AutoTaxi Stand Management System v1.0 was discovered to contain a cross-site scripting (XSS) vulnerability via the component search.php.

- [https://github.com/sudoninja-noob/CVE-2022-43369](https://github.com/sudoninja-noob/CVE-2022-43369) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-43369.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-43369.svg)


## CVE-2022-41678
A more restrictive Jolokia configuration has been defined in default ActiveMQ distribution. We encourage users to upgrade to ActiveMQ distributions version including updated Jolokia configuration: 5.16.6, 5.17.4, 5.18.0, 6.0.0.

- [https://github.com/Catherines77/ActiveMQ-EXPtools](https://github.com/Catherines77/ActiveMQ-EXPtools) :  ![starts](https://img.shields.io/github/stars/Catherines77/ActiveMQ-EXPtools.svg) ![forks](https://img.shields.io/github/forks/Catherines77/ActiveMQ-EXPtools.svg)


## CVE-2022-29009
 Multiple SQL injection vulnerabilities via the username and password parameters in the Admin panel of Cyber Cafe Management System Project v1.0 allows attackers to bypass authentication.

- [https://github.com/sudoninja-noob/CVE-2022-29009](https://github.com/sudoninja-noob/CVE-2022-29009) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-29009.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-29009.svg)


## CVE-2022-29008
 An insecure direct object reference (IDOR) vulnerability in the viewid parameter of Bus Pass Management System v1.0 allows attackers to access sensitive information.

- [https://github.com/sudoninja-noob/CVE-2022-29008](https://github.com/sudoninja-noob/CVE-2022-29008) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-29008.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-29008.svg)


## CVE-2022-29007
 Multiple SQL injection vulnerabilities via the username and password parameters in the Admin panel of Dairy Farm Shop Management System v1.0 allows attackers to bypass authentication.

- [https://github.com/sudoninja-noob/CVE-2022-29007](https://github.com/sudoninja-noob/CVE-2022-29007) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-29007.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-29007.svg)


## CVE-2022-29006
 Multiple SQL injection vulnerabilities via the username and password parameters in the Admin panel of Directory Management System v1.0 allows attackers to bypass authentication.

- [https://github.com/sudoninja-noob/CVE-2022-29006](https://github.com/sudoninja-noob/CVE-2022-29006) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-29006.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-29006.svg)


## CVE-2022-29005
 Multiple cross-site scripting (XSS) vulnerabilities in the component /obcs/user/profile.php of Online Birth Certificate System v1.2 allows attackers to execute arbitrary web scripts or HTML via a crafted payload injected into the fname or lname parameters.

- [https://github.com/sudoninja-noob/CVE-2022-29005](https://github.com/sudoninja-noob/CVE-2022-29005) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-29005.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-29005.svg)


## CVE-2022-29004
 Diary Management System v1.0 was discovered to contain a cross-site scripting (XSS) vulnerability via the Name parameter in search-result.php.

- [https://github.com/sudoninja-noob/CVE-2022-29004](https://github.com/sudoninja-noob/CVE-2022-29004) :  ![starts](https://img.shields.io/github/stars/sudoninja-noob/CVE-2022-29004.svg) ![forks](https://img.shields.io/github/forks/sudoninja-noob/CVE-2022-29004.svg)


## CVE-2022-3590
 WordPress is affected by an unauthenticated blind SSRF in the pingback feature. Because of a TOCTOU race condition between the validation checks and the HTTP request, attackers can reach internal hosts that are explicitly forbidden.

- [https://github.com/TJouleL/WordPress-6.9.1-Blind-SSRF](https://github.com/TJouleL/WordPress-6.9.1-Blind-SSRF) :  ![starts](https://img.shields.io/github/stars/TJouleL/WordPress-6.9.1-Blind-SSRF.svg) ![forks](https://img.shields.io/github/forks/TJouleL/WordPress-6.9.1-Blind-SSRF.svg)


## CVE-2019-15107
 An issue was discovered in Webmin =1.920. The parameter old in password_change.cgi contains a command injection vulnerability.

- [https://github.com/viglia/cve-2019-15107](https://github.com/viglia/cve-2019-15107) :  ![starts](https://img.shields.io/github/stars/viglia/cve-2019-15107.svg) ![forks](https://img.shields.io/github/forks/viglia/cve-2019-15107.svg)


## CVE-2019-2215
 A use-after-free in binder.c allows an elevation of privilege from an application to the Linux Kernel. No user interaction is required to exploit this vulnerability, however exploitation does require either the installation of a malicious local application or a separate vulnerability in a network facing application.Product: AndroidAndroid ID: A-141720095

- [https://github.com/wired0ut/CVE-2019-2215](https://github.com/wired0ut/CVE-2019-2215) :  ![starts](https://img.shields.io/github/stars/wired0ut/CVE-2019-2215.svg) ![forks](https://img.shields.io/github/forks/wired0ut/CVE-2019-2215.svg)


## CVE-2018-16763
 FUEL CMS 1.4.1 allows PHP Code Evaluation via the pages/select/ filter parameter or the preview/ data parameter. This can lead to Pre-Auth Remote Code Execution.

- [https://github.com/bad-c0de/CVE-2018-16763_FuelCMS-1.4.1_RCE](https://github.com/bad-c0de/CVE-2018-16763_FuelCMS-1.4.1_RCE) :  ![starts](https://img.shields.io/github/stars/bad-c0de/CVE-2018-16763_FuelCMS-1.4.1_RCE.svg) ![forks](https://img.shields.io/github/forks/bad-c0de/CVE-2018-16763_FuelCMS-1.4.1_RCE.svg)


## CVE-2017-0144
 The SMBv1 server in Microsoft Windows Vista SP2; Windows Server 2008 SP2 and R2 SP1; Windows 7 SP1; Windows 8.1; Windows Server 2012 Gold and R2; Windows RT 8.1; and Windows 10 Gold, 1511, and 1607; and Windows Server 2016 allows remote attackers to execute arbitrary code via crafted packets, aka "Windows SMB Remote Code Execution Vulnerability." This vulnerability is different from those described in CVE-2017-0143, CVE-2017-0145, CVE-2017-0146, and CVE-2017-0148.

- [https://github.com/dannic145/EternalBlue-DoublePulsar-Exploit-Demonstration](https://github.com/dannic145/EternalBlue-DoublePulsar-Exploit-Demonstration) :  ![starts](https://img.shields.io/github/stars/dannic145/EternalBlue-DoublePulsar-Exploit-Demonstration.svg) ![forks](https://img.shields.io/github/forks/dannic145/EternalBlue-DoublePulsar-Exploit-Demonstration.svg)
- [https://github.com/ichhyak22/EternalBlue-DoublePulsar-Exploit-Demonstration](https://github.com/ichhyak22/EternalBlue-DoublePulsar-Exploit-Demonstration) :  ![starts](https://img.shields.io/github/stars/ichhyak22/EternalBlue-DoublePulsar-Exploit-Demonstration.svg) ![forks](https://img.shields.io/github/forks/ichhyak22/EternalBlue-DoublePulsar-Exploit-Demonstration.svg)


## CVE-2014-6271
 GNU Bash through 4.3 processes trailing strings after function definitions in the values of environment variables, which allows remote attackers to execute arbitrary code via a crafted environment, as demonstrated by vectors involving the ForceCommand feature in OpenSSH sshd, the mod_cgi and mod_cgid modules in the Apache HTTP Server, scripts executed by unspecified DHCP clients, and other situations in which setting the environment occurs across a privilege boundary from Bash execution, aka "ShellShock."  NOTE: the original fix for this issue was incorrect; CVE-2014-7169 has been assigned to cover the vulnerability that is still present after the incorrect fix.

- [https://github.com/V3nG4mxV1p3r/Mobile-Drop-Device-SOC-Detection](https://github.com/V3nG4mxV1p3r/Mobile-Drop-Device-SOC-Detection) :  ![starts](https://img.shields.io/github/stars/V3nG4mxV1p3r/Mobile-Drop-Device-SOC-Detection.svg) ![forks](https://img.shields.io/github/forks/V3nG4mxV1p3r/Mobile-Drop-Device-SOC-Detection.svg)


## CVE-2008-5416
 Heap-based buffer overflow in Microsoft SQL Server 2000 SP4, 8.00.2050, 8.00.2039, and earlier; SQL Server 2000 Desktop Engine (MSDE 2000) SP4; SQL Server 2005 SP2 and 9.00.1399.06; SQL Server 2000 Desktop Engine (WMSDE) on Windows Server 2003 SP1 and SP2; and Windows Internal Database (WYukon) SP2 allows remote authenticated users to cause a denial of service (access violation exception) or execute arbitrary code by calling the sp_replwritetovarbin extended stored procedure with a set of invalid parameters that trigger memory overwrite, aka "SQL Server sp_replwritetovarbin Limited Memory Overwrite Vulnerability."

- [https://github.com/SECFORCE/CVE-2008-5416](https://github.com/SECFORCE/CVE-2008-5416) :  ![starts](https://img.shields.io/github/stars/SECFORCE/CVE-2008-5416.svg) ![forks](https://img.shields.io/github/forks/SECFORCE/CVE-2008-5416.svg)

