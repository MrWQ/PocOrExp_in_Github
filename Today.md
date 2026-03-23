# Update 2026-03-23
## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/MaxMnMl/langflow-CVE-2026-33017-poc](https://github.com/MaxMnMl/langflow-CVE-2026-33017-poc) :  ![starts](https://img.shields.io/github/stars/MaxMnMl/langflow-CVE-2026-33017-poc.svg) ![forks](https://img.shields.io/github/forks/MaxMnMl/langflow-CVE-2026-33017-poc.svg)
- [https://github.com/omer-efe-curkus/CVE-2026-33017-Langflow-RCE-PoC](https://github.com/omer-efe-curkus/CVE-2026-33017-Langflow-RCE-PoC) :  ![starts](https://img.shields.io/github/stars/omer-efe-curkus/CVE-2026-33017-Langflow-RCE-PoC.svg) ![forks](https://img.shields.io/github/forks/omer-efe-curkus/CVE-2026-33017-Langflow-RCE-PoC.svg)
- [https://github.com/SimoesCTT/Sovereign-Echo-33017](https://github.com/SimoesCTT/Sovereign-Echo-33017) :  ![starts](https://img.shields.io/github/stars/SimoesCTT/Sovereign-Echo-33017.svg) ![forks](https://img.shields.io/github/forks/SimoesCTT/Sovereign-Echo-33017.svg)


## CVE-2026-32194
 Improper neutralization of special elements used in a command ('command injection') in Microsoft Bing Images allows an unauthorized attacker to execute code over a network.

- [https://github.com/z3r0h3ro/CVE-2026-32194-POC](https://github.com/z3r0h3ro/CVE-2026-32194-POC) :  ![starts](https://img.shields.io/github/stars/z3r0h3ro/CVE-2026-32194-POC.svg) ![forks](https://img.shields.io/github/forks/z3r0h3ro/CVE-2026-32194-POC.svg)


## CVE-2026-29000
 pac4j-jwt versions prior to 4.5.9, 5.7.9, and 6.3.3 contain an authentication bypass vulnerability in JwtAuthenticator when processing encrypted JWTs that allows remote attackers to forge authentication tokens. Attackers who possess the server's RSA public key can create a JWE-wrapped PlainJWT with arbitrary subject and role claims, bypassing signature verification to authenticate as any user including administrators.

- [https://github.com/oil-lamp-cat/CVE-2026-29000-pac4j-PoC](https://github.com/oil-lamp-cat/CVE-2026-29000-pac4j-PoC) :  ![starts](https://img.shields.io/github/stars/oil-lamp-cat/CVE-2026-29000-pac4j-PoC.svg) ![forks](https://img.shields.io/github/forks/oil-lamp-cat/CVE-2026-29000-pac4j-PoC.svg)


## CVE-2026-25770
 Wazuh is a free and open source platform used for threat prevention, detection, and response. Starting in version 3.9.0 and prior to version 4.14.3, a privilege escalation vulnerability exists in the Wazuh Manager's cluster synchronization protocol. The `wazuh-clusterd` service allows authenticated nodes to write arbitrary files to the manager’s file system with the permissions of the `wazuh` system user. Due to insecure default permissions, the `wazuh` user has write access to the manager's main configuration file (`/var/ossec/etc/ossec.conf`). By leveraging the cluster protocol to overwrite `ossec.conf`, an attacker can inject a malicious `localfile` command block. The `wazuh-logcollector` service, which runs as root, parses this configuration and executes the injected command. This chain allows an attacker with cluster credentials to gain full Root Remote Code Execution, violating the principle of least privilege and bypassing the intended security model. Version 4.14.3 fixes the issue.

- [https://github.com/Samres27/CVE-2026-25769---CVE-2026-25770](https://github.com/Samres27/CVE-2026-25769---CVE-2026-25770) :  ![starts](https://img.shields.io/github/stars/Samres27/CVE-2026-25769---CVE-2026-25770.svg) ![forks](https://img.shields.io/github/forks/Samres27/CVE-2026-25769---CVE-2026-25770.svg)


## CVE-2026-25769
 Wazuh is a free and open source platform used for threat prevention, detection, and response. Versions 4.0.0 through 4.14.2 have a Remote Code Execution (RCE) vulnerability due to Deserialization of Untrusted Data). All Wazuh deployments using cluster mode (master/worker architecture) and any organization with a compromised worker node (e.g., through initial access, insider threat, or supply chain attack) are impacted. An attacker who gains access to a worker node (through any means) can achieve full RCE on the master node with root privileges. Version 4.14.3 fixes the issue.

- [https://github.com/Samres27/CVE-2026-25769---CVE-2026-25770](https://github.com/Samres27/CVE-2026-25769---CVE-2026-25770) :  ![starts](https://img.shields.io/github/stars/Samres27/CVE-2026-25769---CVE-2026-25770.svg) ![forks](https://img.shields.io/github/forks/Samres27/CVE-2026-25769---CVE-2026-25770.svg)


## CVE-2026-23744
 MCPJam inspector is the local-first development platform for MCP servers. Versions 1.4.2 and earlier are vulnerable to remote code execution (RCE) vulnerability, which allows an attacker to send a crafted HTTP request that triggers the installation of an MCP server, leading to RCE. Since MCPJam inspector by default listens on 0.0.0.0 instead of 127.0.0.1, an attacker can trigger the RCE remotely via a simple HTTP request. Version 1.4.3 contains a patch.

- [https://github.com/suljov/CVE-2026-23744-Remote-Code-Execution-POC](https://github.com/suljov/CVE-2026-23744-Remote-Code-Execution-POC) :  ![starts](https://img.shields.io/github/stars/suljov/CVE-2026-23744-Remote-Code-Execution-POC.svg) ![forks](https://img.shields.io/github/forks/suljov/CVE-2026-23744-Remote-Code-Execution-POC.svg)


## CVE-2026-23520
 Arcane provides modern docker management. Prior to 1.13.0, Arcane has a command injection in the updater service. Arcane’s updater service supported lifecycle labels com.getarcaneapp.arcane.lifecycle.pre-update and com.getarcaneapp.arcane.lifecycle.post-update that allowed defining a command to run before or after a container update. The label value is passed directly to /bin/sh -c without sanitization or validation. Because any authenticated user (not limited to administrators) can create projects through the API, an attacker can create a project that specifies one of these lifecycle labels with a malicious command. When an administrator later triggers a container update (either manually or via scheduled update checks), Arcane reads the lifecycle label and executes its value as a shell command inside the container. This vulnerability is fixed in 1.13.0.

- [https://github.com/0xzap/CVE-2026-23520](https://github.com/0xzap/CVE-2026-23520) :  ![starts](https://img.shields.io/github/stars/0xzap/CVE-2026-23520.svg) ![forks](https://img.shields.io/github/forks/0xzap/CVE-2026-23520.svg)
- [https://github.com/Augmaster/POC-CVE-2026-23520](https://github.com/Augmaster/POC-CVE-2026-23520) :  ![starts](https://img.shields.io/github/stars/Augmaster/POC-CVE-2026-23520.svg) ![forks](https://img.shields.io/github/forks/Augmaster/POC-CVE-2026-23520.svg)


## CVE-2026-21994
 Vulnerability in the Oracle Edge Cloud Infrastructure Designer and Visualisation Toolkit product of Oracle Open Source Projects (component: Desktop).   The supported version that is affected is 0.3.0. Easily exploitable vulnerability allows unauthenticated attacker with network access via HTTP to compromise Oracle Edge Cloud Infrastructure Designer and Visualisation Toolkit.  Successful attacks of this vulnerability can result in takeover of Oracle Edge Cloud Infrastructure Designer and Visualisation Toolkit. CVSS 3.1 Base Score 9.8 (Confidentiality, Integrity and Availability impacts).  CVSS Vector: (CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H).

- [https://github.com/g0w6y/CVE-2026-21994](https://github.com/g0w6y/CVE-2026-21994) :  ![starts](https://img.shields.io/github/stars/g0w6y/CVE-2026-21994.svg) ![forks](https://img.shields.io/github/forks/g0w6y/CVE-2026-21994.svg)


## CVE-2026-21962
 Vulnerability in the Oracle HTTP Server, Oracle Weblogic Server Proxy Plug-in product of Oracle Fusion Middleware (component: Weblogic Server Proxy Plug-in for Apache HTTP Server, Weblogic Server Proxy Plug-in for IIS).  Supported versions that are affected are 12.2.1.4.0, 14.1.1.0.0 and  14.1.2.0.0. Easily exploitable vulnerability allows unauthenticated attacker with network access via HTTP to compromise Oracle HTTP Server, Oracle Weblogic Server Proxy Plug-in.  While the vulnerability is in Oracle HTTP Server, Oracle Weblogic Server Proxy Plug-in, attacks may significantly impact additional products (scope change).  Successful attacks of this vulnerability can result in  unauthorized creation, deletion or modification access to critical data or all Oracle HTTP Server, Oracle Weblogic Server Proxy Plug-in accessible data as well as  unauthorized access to critical data or complete access to all Oracle HTTP Server, Oracle Weblogic Server Proxy Plug-in accessible data. Note: Affected version for Weblogic Server Proxy Plug-in for IIS is 12.2.1.4.0 only. CVSS 3.1 Base Score 10.0 (Confidentiality and Integrity impacts).  CVSS Vector: (CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:N).

- [https://github.com/naozibuhao/CVE-2026-21962_Java_GUI_Exploit_Tool](https://github.com/naozibuhao/CVE-2026-21962_Java_GUI_Exploit_Tool) :  ![starts](https://img.shields.io/github/stars/naozibuhao/CVE-2026-21962_Java_GUI_Exploit_Tool.svg) ![forks](https://img.shields.io/github/forks/naozibuhao/CVE-2026-21962_Java_GUI_Exploit_Tool.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-66034
 fontTools is a library for manipulating fonts, written in Python. In versions from 4.33.0 to before 4.60.2, the fonttools varLib (or python3 -m fontTools.varLib) script has an arbitrary file write vulnerability that leads to remote code execution when a malicious .designspace file is processed. The vulnerability affects the main() code path of fontTools.varLib, used by the fonttools varLib CLI and any code that invokes fontTools.varLib.main(). This issue has been patched in version 4.60.2.

- [https://github.com/v3cn4x00/POC-CVE-2025-66034](https://github.com/v3cn4x00/POC-CVE-2025-66034) :  ![starts](https://img.shields.io/github/stars/v3cn4x00/POC-CVE-2025-66034.svg) ![forks](https://img.shields.io/github/forks/v3cn4x00/POC-CVE-2025-66034.svg)
- [https://github.com/d0x-awrqxavc/CVE-2025-66034](https://github.com/d0x-awrqxavc/CVE-2025-66034) :  ![starts](https://img.shields.io/github/stars/d0x-awrqxavc/CVE-2025-66034.svg) ![forks](https://img.shields.io/github/forks/d0x-awrqxavc/CVE-2025-66034.svg)
- [https://github.com/tristanqtn/CVE-2025-66034](https://github.com/tristanqtn/CVE-2025-66034) :  ![starts](https://img.shields.io/github/stars/tristanqtn/CVE-2025-66034.svg) ![forks](https://img.shields.io/github/forks/tristanqtn/CVE-2025-66034.svg)


## CVE-2025-53770
Microsoft is preparing and fully testing a comprehensive update to address this vulnerability.  In the meantime, please make sure that the mitigation provided in this CVE documentation is in place so that you are protected from exploitation.

- [https://github.com/J4ck3LSyN-Gen2/CVE-2025-53770](https://github.com/J4ck3LSyN-Gen2/CVE-2025-53770) :  ![starts](https://img.shields.io/github/stars/J4ck3LSyN-Gen2/CVE-2025-53770.svg) ![forks](https://img.shields.io/github/forks/J4ck3LSyN-Gen2/CVE-2025-53770.svg)


## CVE-2025-32463
 Sudo before 1.9.17p1 allows local users to obtain root access because /etc/nsswitch.conf from a user-controlled directory is used with the --chroot option.

- [https://github.com/oxborn3/CVE-2025-32463-EXPLOIT](https://github.com/oxborn3/CVE-2025-32463-EXPLOIT) :  ![starts](https://img.shields.io/github/stars/oxborn3/CVE-2025-32463-EXPLOIT.svg) ![forks](https://img.shields.io/github/forks/oxborn3/CVE-2025-32463-EXPLOIT.svg)


## CVE-2024-56348
 In JetBrains TeamCity before 2024.12 improper access control allowed viewing details of unauthorized agents

- [https://github.com/Msakhana68/cve-2024-56348](https://github.com/Msakhana68/cve-2024-56348) :  ![starts](https://img.shields.io/github/stars/Msakhana68/cve-2024-56348.svg) ![forks](https://img.shields.io/github/forks/Msakhana68/cve-2024-56348.svg)


## CVE-2024-50603
 An issue was discovered in Aviatrix Controller before 7.1.4191 and 7.2.x before 7.2.4996. Due to the improper neutralization of special elements used in an OS command, an unauthenticated attacker is able to execute arbitrary code. Shell metacharacters can be sent to /v1/api in cloud_type for list_flightpath_destination_instances, or src_cloud_type for flightpath_connection_test.

- [https://github.com/th3gokul/CVE-2024-50603](https://github.com/th3gokul/CVE-2024-50603) :  ![starts](https://img.shields.io/github/stars/th3gokul/CVE-2024-50603.svg) ![forks](https://img.shields.io/github/forks/th3gokul/CVE-2024-50603.svg)
- [https://github.com/newlinesec/CVE-2024-50603](https://github.com/newlinesec/CVE-2024-50603) :  ![starts](https://img.shields.io/github/stars/newlinesec/CVE-2024-50603.svg) ![forks](https://img.shields.io/github/forks/newlinesec/CVE-2024-50603.svg)


## CVE-2024-38063
 Windows TCP/IP Remote Code Execution Vulnerability

- [https://github.com/SALMA-ESSAOUD/CVE-CVSS--CVE-2024-38063-IPv6-TCP-IP-Remote-Code-Execution-Analysis](https://github.com/SALMA-ESSAOUD/CVE-CVSS--CVE-2024-38063-IPv6-TCP-IP-Remote-Code-Execution-Analysis) :  ![starts](https://img.shields.io/github/stars/SALMA-ESSAOUD/CVE-CVSS--CVE-2024-38063-IPv6-TCP-IP-Remote-Code-Execution-Analysis.svg) ![forks](https://img.shields.io/github/forks/SALMA-ESSAOUD/CVE-CVSS--CVE-2024-38063-IPv6-TCP-IP-Remote-Code-Execution-Analysis.svg)


## CVE-2024-10924
 The Really Simple Security (Free, Pro, and Pro Multisite) plugins for WordPress are vulnerable to authentication bypass in versions 9.0.0 to 9.1.1.1. This is due to improper user check error handling in the two-factor REST API actions with the 'check_login_and_get_user' function. This makes it possible for unauthenticated attackers to log in as any existing user on the site, such as an administrator, when the "Two-Factor Authentication" setting is enabled (disabled by default).

- [https://github.com/d0x-awrqxavc/-CVE-2024-10924](https://github.com/d0x-awrqxavc/-CVE-2024-10924) :  ![starts](https://img.shields.io/github/stars/d0x-awrqxavc/-CVE-2024-10924.svg) ![forks](https://img.shields.io/github/forks/d0x-awrqxavc/-CVE-2024-10924.svg)


## CVE-2023-48795
 The SSH transport protocol with certain OpenSSH extensions, found in OpenSSH before 9.6 and other products, allows remote attackers to bypass integrity checks such that some packets are omitted (from the extension negotiation message), and a client and server may consequently end up with a connection for which some security features have been downgraded or disabled, aka a Terrapin attack. This occurs because the SSH Binary Packet Protocol (BPP), implemented by these extensions, mishandles the handshake phase and mishandles use of sequence numbers. For example, there is an effective attack against SSH's use of ChaCha20-Poly1305 (and CBC with Encrypt-then-MAC). The bypass occurs in chacha20-poly1305@openssh.com and (if CBC is used) the -etm@openssh.com MAC algorithms. This also affects Maverick Synergy Java SSH API before 3.1.0-SNAPSHOT, Dropbear through 2022.83, Ssh before 5.1.1 in Erlang/OTP, PuTTY before 0.80, AsyncSSH before 2.14.2, golang.org/x/crypto before 0.17.0, libssh before 0.10.6, libssh2 through 1.11.0, Thorn Tech SFTP Gateway before 3.4.6, Tera Term before 5.1, Paramiko before 3.4.0, jsch before 0.2.15, SFTPGo before 2.5.6, Netgate pfSense Plus through 23.09.1, Netgate pfSense CE through 2.7.2, HPN-SSH through 18.2.0, ProFTPD before 1.3.8b (and before 1.3.9rc2), ORYX CycloneSSH before 2.3.4, NetSarang XShell 7 before Build 0144, CrushFTP before 10.6.0, ConnectBot SSH library before 2.2.22, Apache MINA sshd through 2.11.0, sshj through 0.37.0, TinySSH through 20230101, trilead-ssh2 6401, LANCOM LCOS and LANconfig, FileZilla before 3.66.4, Nova before 11.8, PKIX-SSH before 14.4, SecureCRT before 9.4.3, Transmit5 before 5.10.4, Win32-OpenSSH before 9.5.0.0p1-Beta, WinSCP before 6.2.2, Bitvise SSH Server before 9.32, Bitvise SSH Client before 9.33, KiTTY through 0.76.1.13, the net-ssh gem 7.2.0 for Ruby, the mscdex ssh2 module before 1.15.0 for Node.js, the thrussh library before 0.35.1 for Rust, and the Russh crate before 0.40.2 for Rust.

- [https://github.com/fumioryoto/Terrapin-attack](https://github.com/fumioryoto/Terrapin-attack) :  ![starts](https://img.shields.io/github/stars/fumioryoto/Terrapin-attack.svg) ![forks](https://img.shields.io/github/forks/fumioryoto/Terrapin-attack.svg)


## CVE-2023-21716
 Microsoft Word Remote Code Execution Vulnerability

- [https://github.com/muumthf/CVE-2023-21716](https://github.com/muumthf/CVE-2023-21716) :  ![starts](https://img.shields.io/github/stars/muumthf/CVE-2023-21716.svg) ![forks](https://img.shields.io/github/forks/muumthf/CVE-2023-21716.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/snapdowgg/CVE-2021-41773](https://github.com/snapdowgg/CVE-2021-41773) :  ![starts](https://img.shields.io/github/stars/snapdowgg/CVE-2021-41773.svg) ![forks](https://img.shields.io/github/forks/snapdowgg/CVE-2021-41773.svg)


## CVE-2011-2523
 vsftpd 2.3.4 downloaded between 20110630 and 20110703 contains a backdoor which opens a shell on port 6200/tcp.

- [https://github.com/brettsm/vsftpd2.3.4-backdoor-exploit](https://github.com/brettsm/vsftpd2.3.4-backdoor-exploit) :  ![starts](https://img.shields.io/github/stars/brettsm/vsftpd2.3.4-backdoor-exploit.svg) ![forks](https://img.shields.io/github/forks/brettsm/vsftpd2.3.4-backdoor-exploit.svg)
- [https://github.com/Tr00jan99/PwnTillDawn-Portal-Walkthrough](https://github.com/Tr00jan99/PwnTillDawn-Portal-Walkthrough) :  ![starts](https://img.shields.io/github/stars/Tr00jan99/PwnTillDawn-Portal-Walkthrough.svg) ![forks](https://img.shields.io/github/forks/Tr00jan99/PwnTillDawn-Portal-Walkthrough.svg)

