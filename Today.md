# Update 2026-04-06
## CVE-2026-35616
 A improper access control vulnerability in Fortinet FortiClientEMS 7.4.5 through 7.4.6 may allow an unauthenticated attacker to execute unauthorized code or commands via crafted requests.

- [https://github.com/0xBlackash/CVE-2026-35616](https://github.com/0xBlackash/CVE-2026-35616) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-35616.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-35616.svg)
- [https://github.com/z3r0h3ro/CVE-2026-35616-poc](https://github.com/z3r0h3ro/CVE-2026-35616-poc) :  ![starts](https://img.shields.io/github/stars/z3r0h3ro/CVE-2026-35616-poc.svg) ![forks](https://img.shields.io/github/forks/z3r0h3ro/CVE-2026-35616-poc.svg)


## CVE-2026-33701
 OpenTelemetry Java Instrumentation provides OpenTelemetry auto-instrumentation and instrumentation libraries for Java. In versions prior to 2.26.1, the RMI instrumentation registered a custom endpoint that deserialized incoming data without applying serialization filters. On JDK version 16 and earlier, an attacker with network access to a JMX or RMI port on an instrumented JVM could exploit this to potentially achieve remote code execution. All three of the following conditions must be true to exploit this vulnerability: First, OpenTelemetry Java instrumentation is attached as a Java agent (`-javaagent`) on Java 16 or earlier. Second, JMX/RMI port has been explicitly configured via `-Dcom.sun.management.jmxremote.port` and is network-reachable. Third, gadget-chain-compatible library is present on the classpath. This results in arbitrary remote code execution with the privileges of the user running the instrumented JVM. For JDK = 17, no action is required, but upgrading is strongly encouraged. For JDK  17, upgrade to version 2.26.1 or later. As a workaround, set the system property `-Dotel.instrumentation.rmi.enabled=false` to disable the RMI integration.

- [https://github.com/pl4tyz/CVE-2026-33701-Unsafe-Deserialization-in-OpenTelemetry-Java-Agent-RMI-Instrumentation](https://github.com/pl4tyz/CVE-2026-33701-Unsafe-Deserialization-in-OpenTelemetry-Java-Agent-RMI-Instrumentation) :  ![starts](https://img.shields.io/github/stars/pl4tyz/CVE-2026-33701-Unsafe-Deserialization-in-OpenTelemetry-Java-Agent-RMI-Instrumentation.svg) ![forks](https://img.shields.io/github/forks/pl4tyz/CVE-2026-33701-Unsafe-Deserialization-in-OpenTelemetry-Java-Agent-RMI-Instrumentation.svg)


## CVE-2026-33579
 OpenClaw before 2026.3.28 contains a privilege escalation vulnerability in the /pair approve command path that fails to forward caller scopes into the core approval check. A caller with pairing privileges but without admin privileges can approve pending device requests asking for broader scopes including admin access by exploiting the missing scope validation in extensions/device-pair/index.ts and src/infra/device-pairing.ts.

- [https://github.com/atalovesyou/openclaw-security-checker](https://github.com/atalovesyou/openclaw-security-checker) :  ![starts](https://img.shields.io/github/stars/atalovesyou/openclaw-security-checker.svg) ![forks](https://img.shields.io/github/forks/atalovesyou/openclaw-security-checker.svg)


## CVE-2026-33331
 oRPC is an tool that helps build APIs that are end-to-end type-safe and adhere to OpenAPI standards. Prior to version 1.13.9, a stored cross-site scripting (XSS) vulnerability exists in the OpenAPI documentation generation of orpc. If an attacker can control any field within the OpenAPI specification (such as info.description), they can break out of the JSON context and execute arbitrary JavaScript when a user views the generated API documentation. This issue has been patched in version 1.13.9.

- [https://github.com/abhayclasher/CVE-2026-33331](https://github.com/abhayclasher/CVE-2026-33331) :  ![starts](https://img.shields.io/github/stars/abhayclasher/CVE-2026-33331.svg) ![forks](https://img.shields.io/github/forks/abhayclasher/CVE-2026-33331.svg)


## CVE-2026-3557
The specific flaw exists within the hap_pair_verify_handler function of the hk_hap service, which listens on TCP port 8080 by default. The issue results from the lack of proper validation of the length of user-supplied data prior to copying it to a heap-based buffer. An attacker can leverage this vulnerability to execute code in the context of root. Was ZDI-CAN-28337.

- [https://github.com/Rickidevs/CVE-2026-35570](https://github.com/Rickidevs/CVE-2026-35570) :  ![starts](https://img.shields.io/github/stars/Rickidevs/CVE-2026-35570.svg) ![forks](https://img.shields.io/github/forks/Rickidevs/CVE-2026-35570.svg)


## CVE-2026-3549
 Heap Overflow in TLS 1.3 ECH parsing. An integer underflow existed in ECH extension parsing logic when calculating a buffer length, which resulted in writing beyond the bounds of an allocated buffer. Note that in wolfSSL, ECH is off by default, and the ECH standard is still evolving.

- [https://github.com/redyank/CVE-2026-35492](https://github.com/redyank/CVE-2026-35492) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-35492.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-35492.svg)


## CVE-2026-3502
 TrueConf Client downloads application update code and applies it without performing verification. An attacker who is able to influence the update delivery path can substitute a tampered update payload. If the payload is executed or installed by the updater, this may result in arbitrary code execution in the context of the updating process or user.

- [https://github.com/fevar54/CVE-2026-3502-Scanner---TrueConf-Vulnerability-Detection-Tool](https://github.com/fevar54/CVE-2026-3502-Scanner---TrueConf-Vulnerability-Detection-Tool) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-3502-Scanner---TrueConf-Vulnerability-Detection-Tool.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-3502-Scanner---TrueConf-Vulnerability-Detection-Tool.svg)
- [https://github.com/fevar54/CVE-2026-3502---TrueConf-Client-Update-Hijacking-PoC](https://github.com/fevar54/CVE-2026-3502---TrueConf-Client-Update-Hijacking-PoC) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-3502---TrueConf-Client-Update-Hijacking-PoC.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-3502---TrueConf-Client-Update-Hijacking-PoC.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg)


## CVE-2025-55183
 An information leak vulnerability exists in specific configurations of React Server Components versions 19.0.0, 19.0.1 19.1.0, 19.1.1, 19.1.2, 19.2.0 and 19.2.1, including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. A specifically crafted HTTP request sent to a vulnerable Server Function may unsafely return the source code of any Server Function. Exploitation requires the existence of a Server Function which explicitly or implicitly exposes a stringified argument.

- [https://github.com/omaidnebari/RSC-Scanner-POC](https://github.com/omaidnebari/RSC-Scanner-POC) :  ![starts](https://img.shields.io/github/stars/omaidnebari/RSC-Scanner-POC.svg) ![forks](https://img.shields.io/github/forks/omaidnebari/RSC-Scanner-POC.svg)


## CVE-2025-43407
 This issue was addressed with improved entitlements. This issue is fixed in iOS 26.1 and iPadOS 26.1, macOS Sequoia 15.7.2, macOS Sonoma 14.8.2, macOS Tahoe 26.1, tvOS 26.1, visionOS 26.1. An app may be able to break out of its sandbox.

- [https://github.com/mranonymous234/Sandbox-Escape-iOS-18.0-26.0](https://github.com/mranonymous234/Sandbox-Escape-iOS-18.0-26.0) :  ![starts](https://img.shields.io/github/stars/mranonymous234/Sandbox-Escape-iOS-18.0-26.0.svg) ![forks](https://img.shields.io/github/forks/mranonymous234/Sandbox-Escape-iOS-18.0-26.0.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/MKIRAHMET/CVE-2025-29927-PoC](https://github.com/MKIRAHMET/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/MKIRAHMET/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/MKIRAHMET/CVE-2025-29927-PoC.svg)
- [https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927](https://github.com/sn1p3rt3s7/NextJS_CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/sn1p3rt3s7/NextJS_CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/sn1p3rt3s7/NextJS_CVE-2025-29927.svg)


## CVE-2025-27237
 In Zabbix Agent and Agent 2 on Windows, the OpenSSL configuration file is loaded from a path writable by low-privileged users, allowing malicious modification and potential local privilege escalation by injecting a DLL.

- [https://github.com/HackingLZ/CVE-2025-27237](https://github.com/HackingLZ/CVE-2025-27237) :  ![starts](https://img.shields.io/github/stars/HackingLZ/CVE-2025-27237.svg) ![forks](https://img.shields.io/github/forks/HackingLZ/CVE-2025-27237.svg)


## CVE-2024-49138
 Windows Common Log File System Driver Elevation of Privilege Vulnerability

- [https://github.com/vettrivel007/CVE-2024-49138](https://github.com/vettrivel007/CVE-2024-49138) :  ![starts](https://img.shields.io/github/stars/vettrivel007/CVE-2024-49138.svg) ![forks](https://img.shields.io/github/forks/vettrivel007/CVE-2024-49138.svg)


## CVE-2024-21413
 Microsoft Outlook Remote Code Execution Vulnerability

- [https://github.com/pedro-lucas-melo/Estudo-de-Caso-CVE-2024-21413](https://github.com/pedro-lucas-melo/Estudo-de-Caso-CVE-2024-21413) :  ![starts](https://img.shields.io/github/stars/pedro-lucas-melo/Estudo-de-Caso-CVE-2024-21413.svg) ![forks](https://img.shields.io/github/forks/pedro-lucas-melo/Estudo-de-Caso-CVE-2024-21413.svg)


## CVE-2024-7344
 Howyar UEFI Application "Reloader"  (32-bit and 64-bit)  is vulnerable to execution of unsigned software in a hardcoded path.

- [https://github.com/mkmk435/DanilaBagroot](https://github.com/mkmk435/DanilaBagroot) :  ![starts](https://img.shields.io/github/stars/mkmk435/DanilaBagroot.svg) ![forks](https://img.shields.io/github/forks/mkmk435/DanilaBagroot.svg)


## CVE-2024-3400
Cloud NGFW, Panorama appliances, and Prisma Access are not impacted by this vulnerability.

- [https://github.com/HackingLZ/panrapidcheck](https://github.com/HackingLZ/panrapidcheck) :  ![starts](https://img.shields.io/github/stars/HackingLZ/panrapidcheck.svg) ![forks](https://img.shields.io/github/forks/HackingLZ/panrapidcheck.svg)


## CVE-2024-3094
Through a series of complex obfuscations, the liblzma build process extracts a prebuilt object file from a disguised test file existing in the source code, which is then used to modify specific functions in the liblzma code. This results in a modified liblzma library that can be used by any software linked against this library, intercepting and modifying the data interaction with this library.

- [https://github.com/ElinaNotElina/cve-2024-3094-analysis](https://github.com/ElinaNotElina/cve-2024-3094-analysis) :  ![starts](https://img.shields.io/github/stars/ElinaNotElina/cve-2024-3094-analysis.svg) ![forks](https://img.shields.io/github/forks/ElinaNotElina/cve-2024-3094-analysis.svg)


## CVE-2023-45777
 In checkKeyIntentParceledCorrectly of AccountManagerService.java, there is a possible way to launch arbitrary activities using system privileges due to Parcel Mismatch. This could lead to local escalation of privilege with no additional execution privileges needed. User interaction is not needed for exploitation.

- [https://github.com/B-D-APL/silver-succotash](https://github.com/B-D-APL/silver-succotash) :  ![starts](https://img.shields.io/github/stars/B-D-APL/silver-succotash.svg) ![forks](https://img.shields.io/github/forks/B-D-APL/silver-succotash.svg)


## CVE-2023-3262
 The Dataprobe iBoot PDU running firmware version 1.43.03312023 or earlier uses hard-coded credentials for all interactions with the internal Postgres database.A malicious agent with the ability to execute operating system commands on the device can leverage this vulnerability to read, modify, or delete arbitrary database records.

- [https://github.com/z3usx01/CVE-2023-2640-3262-PoC](https://github.com/z3usx01/CVE-2023-2640-3262-PoC) :  ![starts](https://img.shields.io/github/stars/z3usx01/CVE-2023-2640-3262-PoC.svg) ![forks](https://img.shields.io/github/forks/z3usx01/CVE-2023-2640-3262-PoC.svg)


## CVE-2023-2640
 On Ubuntu kernels carrying both c914c0e27eb0 and "UBUNTU: SAUCE: overlayfs: Skip permission checking for trusted.overlayfs.* xattrs", an unprivileged user may set privileged extended attributes on the mounted files, leading them to be set on the upper files without the appropriate security checks.

- [https://github.com/z3usx01/CVE-2023-2640-3262-PoC](https://github.com/z3usx01/CVE-2023-2640-3262-PoC) :  ![starts](https://img.shields.io/github/stars/z3usx01/CVE-2023-2640-3262-PoC.svg) ![forks](https://img.shields.io/github/forks/z3usx01/CVE-2023-2640-3262-PoC.svg)


## CVE-2022-27666
 A heap buffer overflow flaw was found in IPsec ESP transformation code in net/ipv4/esp4.c and net/ipv6/esp6.c. This flaw allows a local attacker with a normal user privilege to overwrite kernel heap objects and may cause a local privilege escalation threat.

- [https://github.com/ngtuonghung/CVE-2022-27666](https://github.com/ngtuonghung/CVE-2022-27666) :  ![starts](https://img.shields.io/github/stars/ngtuonghung/CVE-2022-27666.svg) ![forks](https://img.shields.io/github/forks/ngtuonghung/CVE-2022-27666.svg)


## CVE-2018-15473
 OpenSSH through 7.7 is prone to a user enumeration vulnerability due to not delaying bailout for an invalid authenticating user until after the packet containing the request has been fully parsed, related to auth2-gss.c, auth2-hostbased.c, and auth2-pubkey.c.

- [https://github.com/kaktus5454/CVE-2018-15473](https://github.com/kaktus5454/CVE-2018-15473) :  ![starts](https://img.shields.io/github/stars/kaktus5454/CVE-2018-15473.svg) ![forks](https://img.shields.io/github/forks/kaktus5454/CVE-2018-15473.svg)


## CVE-2017-11882
 Microsoft Office 2007 Service Pack 3, Microsoft Office 2010 Service Pack 2, Microsoft Office 2013 Service Pack 1, and Microsoft Office 2016 allow an attacker to run arbitrary code in the context of the current user by failing to properly handle objects in memory, aka "Microsoft Office Memory Corruption Vulnerability". This CVE ID is unique from CVE-2017-11884.

- [https://github.com/pixelofapicture/001-Malware-Analysis-CVE-2017-11882](https://github.com/pixelofapicture/001-Malware-Analysis-CVE-2017-11882) :  ![starts](https://img.shields.io/github/stars/pixelofapicture/001-Malware-Analysis-CVE-2017-11882.svg) ![forks](https://img.shields.io/github/forks/pixelofapicture/001-Malware-Analysis-CVE-2017-11882.svg)


## CVE-2017-5638
 The Jakarta Multipart parser in Apache Struts 2 2.3.x before 2.3.32 and 2.5.x before 2.5.10.1 has incorrect exception handling and error-message generation during file-upload attempts, which allows remote attackers to execute arbitrary commands via a crafted Content-Type, Content-Disposition, or Content-Length HTTP header, as exploited in the wild in March 2017 with a Content-Type header containing a #cmd= string.

- [https://github.com/AIPEAC/SC3010-Computer-Security](https://github.com/AIPEAC/SC3010-Computer-Security) :  ![starts](https://img.shields.io/github/stars/AIPEAC/SC3010-Computer-Security.svg) ![forks](https://img.shields.io/github/forks/AIPEAC/SC3010-Computer-Security.svg)


## CVE-2011-2523
 vsftpd 2.3.4 downloaded between 20110630 and 20110703 contains a backdoor which opens a shell on port 6200/tcp.

- [https://github.com/Dahalsamir/CVE-2011-2523-exploit](https://github.com/Dahalsamir/CVE-2011-2523-exploit) :  ![starts](https://img.shields.io/github/stars/Dahalsamir/CVE-2011-2523-exploit.svg) ![forks](https://img.shields.io/github/forks/Dahalsamir/CVE-2011-2523-exploit.svg)


## CVE-2007-1260
 Stack-based buffer overflow in the connectHandle function in server.cpp in WebMod 0.48 allows remote attackers to execute arbitrary code via a long string in the Content-Length HTTP header.

- [https://github.com/thecybermind/w48crash](https://github.com/thecybermind/w48crash) :  ![starts](https://img.shields.io/github/stars/thecybermind/w48crash.svg) ![forks](https://img.shields.io/github/forks/thecybermind/w48crash.svg)

