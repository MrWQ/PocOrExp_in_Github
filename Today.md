# Update 2026-04-04
## CVE-2026-34828
 listmonk is a standalone, self-hosted, newsletter and mailing list manager. From version 4.1.0 to before version 6.1.0, a session management vulnerability allows previously issued authenticated sessions to remain valid after sensitive account security changes, specifically password reset and password change. As a result, an attacker who has already obtained a valid session cookie can retain access to the account even after the victim changes or resets their password. This weakens account recovery and session security guarantees. This issue has been patched in version 6.1.0.

- [https://github.com/0xmrma/CVE-2026-34828](https://github.com/0xmrma/CVE-2026-34828) :  ![starts](https://img.shields.io/github/stars/0xmrma/CVE-2026-34828.svg) ![forks](https://img.shields.io/github/forks/0xmrma/CVE-2026-34828.svg)


## CVE-2026-33936
 The `ecdsa` PyPI package is a pure Python implementation of ECC (Elliptic Curve Cryptography) with support for ECDSA (Elliptic Curve Digital Signature Algorithm), EdDSA (Edwards-curve Digital Signature Algorithm) and ECDH (Elliptic Curve Diffie-Hellman). Prior to version 0.19.2, an issue in the low-level DER parsing functions can cause unexpected exceptions to be raised from the public API functions. `ecdsa.der.remove_octet_string()` accepts truncated DER where the encoded length exceeds the available buffer. For example, an OCTET STRING that declares a length of 4096 bytes but provides only 3 bytes is parsed successfully instead of being rejected. Because of that, a crafted DER input can cause `SigningKey.from_der()` to raise an internal exception (`IndexError: index out of bounds on dimension 1`) rather than cleanly rejecting malformed DER (e.g., raising `UnexpectedDER` or `ValueError`). Applications that parse untrusted DER private keys may crash if they do not handle unexpected exceptions, resulting in a denial of service. Version 0.19.2 patches the issue.

- [https://github.com/0xmrma/CVE-2026-33936](https://github.com/0xmrma/CVE-2026-33936) :  ![starts](https://img.shields.io/github/stars/0xmrma/CVE-2026-33936.svg) ![forks](https://img.shields.io/github/forks/0xmrma/CVE-2026-33936.svg)


## CVE-2026-32746
 telnetd in GNU inetutils through 2.7 allows an out-of-bounds write in the LINEMODE SLC (Set Local Characters) suboption handler because add_slc does not check whether the buffer is full.

- [https://github.com/ekomsSavior/telnet_scan](https://github.com/ekomsSavior/telnet_scan) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/telnet_scan.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/telnet_scan.svg)


## CVE-2026-30332
 A Time-of-Check to Time-of-Use (TOCTOU) race condition vulnerability in Balena Etcher for Windows prior to v2.1.4 allows attackers to escalate privileges and execute arbitrary code via replacing a legitimate script with a crafted payload during the flashing process.

- [https://github.com/B1tBreaker/CVE-2026-30332](https://github.com/B1tBreaker/CVE-2026-30332) :  ![starts](https://img.shields.io/github/stars/B1tBreaker/CVE-2026-30332.svg) ![forks](https://img.shields.io/github/forks/B1tBreaker/CVE-2026-30332.svg)


## CVE-2026-27944
 Nginx UI is a web user interface for the Nginx web server. Prior to version 2.3.3, the /api/backup endpoint is accessible without authentication and discloses the encryption keys required to decrypt the backup in the X-Backup-Security response header. This allows an unauthenticated attacker to download a full system backup containing sensitive data (user credentials, session tokens, SSL private keys, Nginx configurations) and decrypt it immediately. This issue has been patched in version 2.3.3.

- [https://github.com/Goultarde/CVE-2026-27944-poc](https://github.com/Goultarde/CVE-2026-27944-poc) :  ![starts](https://img.shields.io/github/stars/Goultarde/CVE-2026-27944-poc.svg) ![forks](https://img.shields.io/github/forks/Goultarde/CVE-2026-27944-poc.svg)


## CVE-2026-24061
 telnetd in GNU Inetutils through 2.7 allows remote authentication bypass via a "-f root" value for the USER environment variable.

- [https://github.com/ekomsSavior/telnet_scan](https://github.com/ekomsSavior/telnet_scan) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/telnet_scan.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/telnet_scan.svg)


## CVE-2026-23416
also happens to simplify the logic.

- [https://github.com/bluedragonsecurity/CVE-2026-23416-POC](https://github.com/bluedragonsecurity/CVE-2026-23416-POC) :  ![starts](https://img.shields.io/github/stars/bluedragonsecurity/CVE-2026-23416-POC.svg) ![forks](https://img.shields.io/github/forks/bluedragonsecurity/CVE-2026-23416-POC.svg)


## CVE-2026-22738
This issue affects Spring AI: from 1.0.0 before 1.0.5, from 1.1.0 before 1.1.4.

- [https://github.com/n0n4m3x41/CVE-2026-22738-POC](https://github.com/n0n4m3x41/CVE-2026-22738-POC) :  ![starts](https://img.shields.io/github/stars/n0n4m3x41/CVE-2026-22738-POC.svg) ![forks](https://img.shields.io/github/forks/n0n4m3x41/CVE-2026-22738-POC.svg)


## CVE-2026-21628
 A improperly secured file management feature allows uploads of dangerous data types for unauthenticated users, leading to remote code execution.

- [https://github.com/webshellseo8/CVE-2026-21628-POC](https://github.com/webshellseo8/CVE-2026-21628-POC) :  ![starts](https://img.shields.io/github/stars/webshellseo8/CVE-2026-21628-POC.svg) ![forks](https://img.shields.io/github/forks/webshellseo8/CVE-2026-21628-POC.svg)


## CVE-2026-5281
 Use after free in Dawn in Google Chrome prior to 146.0.7680.178 allowed a remote attacker who had compromised the renderer process to execute arbitrary code via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/umair-aziz025/CVE-2026-5281-Research-Toolkit](https://github.com/umair-aziz025/CVE-2026-5281-Research-Toolkit) :  ![starts](https://img.shields.io/github/stars/umair-aziz025/CVE-2026-5281-Research-Toolkit.svg) ![forks](https://img.shields.io/github/forks/umair-aziz025/CVE-2026-5281-Research-Toolkit.svg)


## CVE-2026-5027
 The 'POST /api/v2/files' endpoint does not sanitize the 'filename' parameter from the multipart form data, allowing an attacker to write files to arbitrary locations on the filesystem using path traversal sequences ('../').

- [https://github.com/yahiahamza/CVE-2026-5027](https://github.com/yahiahamza/CVE-2026-5027) :  ![starts](https://img.shields.io/github/stars/yahiahamza/CVE-2026-5027.svg) ![forks](https://img.shields.io/github/forks/yahiahamza/CVE-2026-5027.svg)


## CVE-2026-3266
This issue affects Filr: through 25.1.2.

- [https://github.com/MichaelAdamGroberman/CVE-2026-32662](https://github.com/MichaelAdamGroberman/CVE-2026-32662) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-32662.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-32662.svg)


## CVE-2026-3264
 A vulnerability was determined in go2ismail Free-CRM up to b83c40a90726d5e58f0cc680ffdcaa28a03fb5d1. Affected by this issue is some unknown functionality of the component Administrative Interface. Executing a manipulation can lead to execution after redirect. The attack can be executed remotely. The exploit has been publicly disclosed and may be utilized. This product implements a rolling release for ongoing delivery, which means version information for affected or updated releases is unavailable. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/MichaelAdamGroberman/CVE-2026-32646](https://github.com/MichaelAdamGroberman/CVE-2026-32646) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-32646.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-32646.svg)


## CVE-2026-2876
 A vulnerability was determined in Tenda A18 15.13.07.13. This affects the function parse_macfilter_rule of the file /goform/setBlackRule. This manipulation of the argument deviceList causes stack-based buffer overflow. The attack may be initiated remotely. The exploit has been publicly disclosed and may be utilized.

- [https://github.com/MichaelAdamGroberman/CVE-2026-28767](https://github.com/MichaelAdamGroberman/CVE-2026-28767) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-28767.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-28767.svg)
- [https://github.com/MichaelAdamGroberman/CVE-2026-28766](https://github.com/MichaelAdamGroberman/CVE-2026-28766) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2026-28766.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2026-28766.svg)


## CVE-2026-2699
 Customer Managed ShareFile Storage Zones Controller (SZC) allows an unauthenticated attacker to access restricted configuration pages. This leads to changing system configuration and potential remote code execution.

- [https://github.com/watchtowrlabs/watchTowr-vs-Progress-ShareFile-CVE-2026-2699](https://github.com/watchtowrlabs/watchTowr-vs-Progress-ShareFile-CVE-2026-2699) :  ![starts](https://img.shields.io/github/stars/watchtowrlabs/watchTowr-vs-Progress-ShareFile-CVE-2026-2699.svg) ![forks](https://img.shields.io/github/forks/watchtowrlabs/watchTowr-vs-Progress-ShareFile-CVE-2026-2699.svg)


## CVE-2025-47812
 In Wing FTP Server before 7.4.4. the user and admin web interfaces mishandle '\0' bytes, ultimately allowing injection of arbitrary Lua code into user session files. This can be used to execute arbitrary system commands with the privileges of the FTP service (root or SYSTEM by default). This is thus a remote code execution vulnerability that guarantees a total server compromise. This is also exploitable via anonymous FTP accounts.

- [https://github.com/havbay/CVE-2025-47812-PoC](https://github.com/havbay/CVE-2025-47812-PoC) :  ![starts](https://img.shields.io/github/stars/havbay/CVE-2025-47812-PoC.svg) ![forks](https://img.shields.io/github/forks/havbay/CVE-2025-47812-PoC.svg)


## CVE-2025-34037
 An OS command injection vulnerability exists in various models of E-Series Linksys routers via the /tmUnblock.cgi and /hndUnblock.cgi endpoints over HTTP on port 8080. The CGI scripts improperly process user-supplied input passed to the ttcp_ip parameter without sanitization, allowing unauthenticated attackers to inject shell commands. This vulnerability was reported to be exploited in the wild by the "TheMoon" worm  in 2014 to deploy a MIPS ELF payload, enabling arbitrary code execution on the router. Additionally, this vulnerability may affect other Linksys products to include, but not limited to, WAG/WAP/WES/WET/WRT-series router models and Wireless-N access points and routers. Exploitation evidence was observed by the Shadowserver Foundation on 2025-02-06 UTC.

- [https://github.com/Taxanehh/CVE-2025-34037](https://github.com/Taxanehh/CVE-2025-34037) :  ![starts](https://img.shields.io/github/stars/Taxanehh/CVE-2025-34037.svg) ![forks](https://img.shields.io/github/forks/Taxanehh/CVE-2025-34037.svg)


## CVE-2025-32433
 Erlang/OTP is a set of libraries for the Erlang programming language. Prior to versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20, a SSH server may allow an attacker to perform unauthenticated remote code execution (RCE). By exploiting a flaw in SSH protocol message handling, a malicious actor could gain unauthorized access to affected systems and execute arbitrary commands without valid credentials. This issue is patched in versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20. A temporary workaround involves disabling the SSH server or to prevent access via firewall rules.

- [https://github.com/ekomsSavior/POC_CVE-2025-32433](https://github.com/ekomsSavior/POC_CVE-2025-32433) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/POC_CVE-2025-32433.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/POC_CVE-2025-32433.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/metasploit403/cve-2025-29927-lab](https://github.com/metasploit403/cve-2025-29927-lab) :  ![starts](https://img.shields.io/github/stars/metasploit403/cve-2025-29927-lab.svg) ![forks](https://img.shields.io/github/forks/metasploit403/cve-2025-29927-lab.svg)


## CVE-2025-26466
 A flaw was found in the OpenSSH package. For each ping packet the SSH server receives, a pong packet is allocated in a memory buffer and stored in a queue of packages. It is only freed when the server/client key exchange has finished. A malicious client may keep sending such packages, leading to an uncontrolled increase in memory consumption on the server side. Consequently, the server may become unavailable, resulting in a denial of service attack.

- [https://github.com/tpirate/CVE-2025-26466](https://github.com/tpirate/CVE-2025-26466) :  ![starts](https://img.shields.io/github/stars/tpirate/CVE-2025-26466.svg) ![forks](https://img.shields.io/github/forks/tpirate/CVE-2025-26466.svg)


## CVE-2025-24999
 Improper access control in SQL Server allows an authorized attacker to elevate privileges over a network.

- [https://github.com/emad-almousa/CVE-2025-24999](https://github.com/emad-almousa/CVE-2025-24999) :  ![starts](https://img.shields.io/github/stars/emad-almousa/CVE-2025-24999.svg) ![forks](https://img.shields.io/github/forks/emad-almousa/CVE-2025-24999.svg)


## CVE-2025-24252
 A use-after-free issue was addressed with improved memory management. This issue is fixed in iOS 18.4 and iPadOS 18.4, iPadOS 17.7.6, macOS Sequoia 15.4, macOS Sonoma 14.7.5, macOS Ventura 13.7.5, tvOS 18.4, visionOS 2.4. An attacker on the local network may be able to corrupt process memory.

- [https://github.com/ekomsSavior/AirBorne-PoC](https://github.com/ekomsSavior/AirBorne-PoC) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/AirBorne-PoC.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/AirBorne-PoC.svg)


## CVE-2025-24132
 The issue was addressed with improved memory handling. This issue is fixed in AirPlay audio SDK 2.7.1 and AirPlay video SDK 3.6.0.126. An attacker on the local network may cause an unexpected app termination.

- [https://github.com/ekomsSavior/AirBorne-PoC](https://github.com/ekomsSavior/AirBorne-PoC) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/AirBorne-PoC.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/AirBorne-PoC.svg)


## CVE-2025-1068
 There is an untrusted search path vulnerability in Esri ArcGIS AllSource 1.2 and 1.3 that may allow a low privileged attacker with write privileges to the local file system to introduce a malicious executable to the filesystem. When the victim performs a specific action using ArcGIS AllSource, the file could execute and run malicious commands under the context of the victim. This issue is corrected in ArcGIS AllSource 1.2.1 and 1.3.1.

- [https://github.com/MichaelAdamGroberman/CVE-2025-10681](https://github.com/MichaelAdamGroberman/CVE-2025-10681) :  ![starts](https://img.shields.io/github/stars/MichaelAdamGroberman/CVE-2025-10681.svg) ![forks](https://img.shields.io/github/forks/MichaelAdamGroberman/CVE-2025-10681.svg)


## CVE-2023-50094
 reNgine before 2.1.2 allows OS Command Injection if an adversary has a valid session ID. The attack places shell metacharacters in an api/tools/waf_detector/?url= string. The commands are executed as root via subprocess.check_output.

- [https://github.com/Zierax/CVE-2023-50094_POC](https://github.com/Zierax/CVE-2023-50094_POC) :  ![starts](https://img.shields.io/github/stars/Zierax/CVE-2023-50094_POC.svg) ![forks](https://img.shields.io/github/forks/Zierax/CVE-2023-50094_POC.svg)


## CVE-2022-46169
This command injection vulnerability allows an unauthenticated user to execute arbitrary commands if a `poller_item` with the `action` type `POLLER_ACTION_SCRIPT_PHP` (`2`) is configured. The authorization bypass should be prevented by not allowing an attacker to make `get_client_addr` (file `lib/functions.php`) return an arbitrary IP address. This could be done by not honoring the `HTTP_...` `$_SERVER` variables. If these should be kept for compatibility reasons it should at least be prevented to fake the IP address of the server running Cacti. This vulnerability has been addressed in both the 1.2.x and 1.3.x release branches with `1.2.23` being the first release containing the patch.

- [https://github.com/nicostan15/CVE-2022-46169](https://github.com/nicostan15/CVE-2022-46169) :  ![starts](https://img.shields.io/github/stars/nicostan15/CVE-2022-46169.svg) ![forks](https://img.shields.io/github/forks/nicostan15/CVE-2022-46169.svg)


## CVE-2021-43798
 Grafana is an open-source platform for monitoring and observability. Grafana versions 8.0.0-beta1 through 8.3.0 (except for patched versions) iss vulnerable to directory traversal, allowing access to local files. The vulnerable URL path is: `grafana_host_url/public/plugins//`, where is the plugin ID for any installed plugin. At no time has Grafana Cloud been vulnerable. Users are advised to upgrade to patched versions 8.0.7, 8.1.8, 8.2.7, or 8.3.1. The GitHub Security Advisory contains more information about vulnerable URL paths, mitigation, and the disclosure timeline.

- [https://github.com/kikechans/Grafana-LFI-Exploit-CVE-2021-43798-](https://github.com/kikechans/Grafana-LFI-Exploit-CVE-2021-43798-) :  ![starts](https://img.shields.io/github/stars/kikechans/Grafana-LFI-Exploit-CVE-2021-43798-.svg) ![forks](https://img.shields.io/github/forks/kikechans/Grafana-LFI-Exploit-CVE-2021-43798-.svg)


## CVE-2021-21220
 Insufficient validation of untrusted input in V8 in Google Chrome prior to 89.0.4389.128 allowed a remote attacker to potentially exploit heap corruption via a crafted HTML page.

- [https://github.com/JacobTaylor3/CVE-2021-21220](https://github.com/JacobTaylor3/CVE-2021-21220) :  ![starts](https://img.shields.io/github/stars/JacobTaylor3/CVE-2021-21220.svg) ![forks](https://img.shields.io/github/forks/JacobTaylor3/CVE-2021-21220.svg)


## CVE-2019-11043
 In PHP versions 7.1.x below 7.1.33, 7.2.x below 7.2.24 and 7.3.x below 7.3.11 in certain configurations of FPM setup it is possible to cause FPM module to write past allocated buffers into the space reserved for FCGI protocol data, thus opening the possibility of remote code execution.

- [https://github.com/bayazid-bit/CVE-2019-11043](https://github.com/bayazid-bit/CVE-2019-11043) :  ![starts](https://img.shields.io/github/stars/bayazid-bit/CVE-2019-11043.svg) ![forks](https://img.shields.io/github/forks/bayazid-bit/CVE-2019-11043.svg)


## CVE-2018-15473
 OpenSSH through 7.7 is prone to a user enumeration vulnerability due to not delaying bailout for an invalid authenticating user until after the packet containing the request has been fully parsed, related to auth2-gss.c, auth2-hostbased.c, and auth2-pubkey.c.

- [https://github.com/kikechans/SSH-Enum-CVE-2018-15473](https://github.com/kikechans/SSH-Enum-CVE-2018-15473) :  ![starts](https://img.shields.io/github/stars/kikechans/SSH-Enum-CVE-2018-15473.svg) ![forks](https://img.shields.io/github/forks/kikechans/SSH-Enum-CVE-2018-15473.svg)


## CVE-2018-13379
 An Improper Limitation of a Pathname to a Restricted Directory ("Path Traversal") in Fortinet FortiOS 6.0.0 to 6.0.4, 5.6.3 to 5.6.7 and 5.4.6 to 5.4.12 and FortiProxy 2.0.0, 1.2.0 to 1.2.8, 1.1.0 to 1.1.6, 1.0.0 to 1.0.7 under SSL VPN web portal allows an unauthenticated attacker to download system files via special crafted HTTP resource requests.

- [https://github.com/Zierax/CVE-2018-13379](https://github.com/Zierax/CVE-2018-13379) :  ![starts](https://img.shields.io/github/stars/Zierax/CVE-2018-13379.svg) ![forks](https://img.shields.io/github/forks/Zierax/CVE-2018-13379.svg)


## CVE-2017-0144
 The SMBv1 server in Microsoft Windows Vista SP2; Windows Server 2008 SP2 and R2 SP1; Windows 7 SP1; Windows 8.1; Windows Server 2012 Gold and R2; Windows RT 8.1; and Windows 10 Gold, 1511, and 1607; and Windows Server 2016 allows remote attackers to execute arbitrary code via crafted packets, aka "Windows SMB Remote Code Execution Vulnerability." This vulnerability is different from those described in CVE-2017-0143, CVE-2017-0145, CVE-2017-0146, and CVE-2017-0148.

- [https://github.com/althany/CVE-2017-0144_Lab-Guide](https://github.com/althany/CVE-2017-0144_Lab-Guide) :  ![starts](https://img.shields.io/github/stars/althany/CVE-2017-0144_Lab-Guide.svg) ![forks](https://img.shields.io/github/forks/althany/CVE-2017-0144_Lab-Guide.svg)


## CVE-2012-1823
 sapi/cgi/cgi_main.c in PHP before 5.3.12 and 5.4.x before 5.4.2, when configured as a CGI script (aka php-cgi), does not properly handle query strings that lack an = (equals sign) character, which allows remote attackers to execute arbitrary code by placing command-line options in the query string, related to lack of skipping a certain php_getopt for the 'd' case.

- [https://github.com/tryj/CVE-2012-1823---PHP-CGI---RCE](https://github.com/tryj/CVE-2012-1823---PHP-CGI---RCE) :  ![starts](https://img.shields.io/github/stars/tryj/CVE-2012-1823---PHP-CGI---RCE.svg) ![forks](https://img.shields.io/github/forks/tryj/CVE-2012-1823---PHP-CGI---RCE.svg)

