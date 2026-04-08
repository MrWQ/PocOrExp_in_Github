# Update 2026-04-08
## CVE-2026-35616
 A improper access control vulnerability in Fortinet FortiClientEMS 7.4.5 through 7.4.6 may allow an unauthenticated attacker to execute unauthorized code or commands via crafted requests.

- [https://github.com/BishopFox/CVE-2026-35616-check](https://github.com/BishopFox/CVE-2026-35616-check) :  ![starts](https://img.shields.io/github/stars/BishopFox/CVE-2026-35616-check.svg) ![forks](https://img.shields.io/github/forks/BishopFox/CVE-2026-35616-check.svg)
- [https://github.com/fevar54/CVE-2026-35616-detector.py](https://github.com/fevar54/CVE-2026-35616-detector.py) :  ![starts](https://img.shields.io/github/stars/fevar54/CVE-2026-35616-detector.py.svg) ![forks](https://img.shields.io/github/forks/fevar54/CVE-2026-35616-detector.py.svg)
- [https://github.com/fevar54/forticlient_ems_cve_2026_35616_poc.py](https://github.com/fevar54/forticlient_ems_cve_2026_35616_poc.py) :  ![starts](https://img.shields.io/github/stars/fevar54/forticlient_ems_cve_2026_35616_poc.py.svg) ![forks](https://img.shields.io/github/forks/fevar54/forticlient_ems_cve_2026_35616_poc.py.svg)


## CVE-2026-35045
 Tandoor Recipes is an application for managing recipes, planning meals, and building shopping lists. Prior to 2.6.4, the PUT /api/recipe/batch_update/ endpoint in Tandoor Recipes allows any authenticated user within a Space to modify any recipe in that Space, including recipes marked as private by other users. This bypasses all object-level authorization checks enforced on standard single-recipe endpoints (PUT /api/recipe/{id}/), enabling forced exposure of private recipes, unauthorized self-grant of access via the shared list, and metadata tampering. This vulnerability is fixed in 2.6.4.

- [https://github.com/FilipeGaudard/CVE-2026-35045-PoC](https://github.com/FilipeGaudard/CVE-2026-35045-PoC) :  ![starts](https://img.shields.io/github/stars/FilipeGaudard/CVE-2026-35045-PoC.svg) ![forks](https://img.shields.io/github/forks/FilipeGaudard/CVE-2026-35045-PoC.svg)


## CVE-2026-34444
 Lupa integrates the runtimes of Lua or LuaJIT2 into CPython. In 2.6 and earlier, attribute_filter is not consistently applied when attributes are accessed through built-in functions like getattr and setattr. This allows an attacker to bypass the intended restrictions and eventually achieve arbitrary code execution.

- [https://github.com/redyank/CVE-2026-34444](https://github.com/redyank/CVE-2026-34444) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-34444.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-34444.svg)


## CVE-2026-33752
 curl_cffi is the a Python binding for curl. Prior to 0.15.0, curl_cffi does not restrict requests to internal IP ranges, and follows redirects automatically via the underlying libcurl. Because of this, an attacker-controlled URL can redirect requests to internal services such as cloud metadata endpoints. In addition, curl_cffi’s TLS impersonation feature can make these requests appear as legitimate browser traffic, which may bypass certain network controls. This vulnerability is fixed in 0.15.0.

- [https://github.com/redyank/CVE-2026-33752](https://github.com/redyank/CVE-2026-33752) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-33752.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-33752.svg)


## CVE-2026-33186
 gRPC-Go is the Go language implementation of gRPC. Versions prior to 1.79.3 have an authorization bypass resulting from improper input validation of the HTTP/2 `:path` pseudo-header. The gRPC-Go server was too lenient in its routing logic, accepting requests where the `:path` omitted the mandatory leading slash (e.g., `Service/Method` instead of `/Service/Method`). While the server successfully routed these requests to the correct handler, authorization interceptors (including the official `grpc/authz` package) evaluated the raw, non-canonical path string. Consequently, "deny" rules defined using canonical paths (starting with `/`) failed to match the incoming request, allowing it to bypass the policy if a fallback "allow" rule was present. This affects gRPC-Go servers that use path-based authorization interceptors, such as the official RBAC implementation in `google.golang.org/grpc/authz` or custom interceptors relying on `info.FullMethod` or `grpc.Method(ctx)`; AND that have a security policy contains specific "deny" rules for canonical paths but allows other requests by default (a fallback "allow" rule). The vulnerability is exploitable by an attacker who can send raw HTTP/2 frames with malformed `:path` headers directly to the gRPC server. The fix in version 1.79.3 ensures that any request with a `:path` that does not start with a leading slash is immediately rejected with a `codes.Unimplemented` error, preventing it from reaching authorization interceptors or handlers with a non-canonical path string. While upgrading is the most secure and recommended path, users can mitigate the vulnerability using one of the following methods: Use a validating interceptor (recommended mitigation); infrastructure-level normalization; and/or policy hardening.

- [https://github.com/JohannesLks/CVE-2026-33186](https://github.com/JohannesLks/CVE-2026-33186) :  ![starts](https://img.shields.io/github/stars/JohannesLks/CVE-2026-33186.svg) ![forks](https://img.shields.io/github/forks/JohannesLks/CVE-2026-33186.svg)


## CVE-2026-32945
 PJSIP is a free and open source multimedia communication library written in C. Versions 2.16 and below have a Heap-based Buffer Overflowvulnerability in the DNS parser's name length handler. Thisimpacts applications using PJSIP's built-in DNS resolver, such as those configured with pjsua_config.nameserver or UaConfig.nameserver in PJSUA/PJSUA2. It does not affect users who rely on the OS resolver (e.g., getaddrinfo()) by not configuring a nameserver, or those using an external resolver via pjsip_resolver_set_ext_resolver(). This issue is fixed in version 2.17. For users unable to upgrade, a workaround is to disable DNS resolution in the PJSIP config (by setting nameserver_count to zero) or to use an external resolver implementation instead.

- [https://github.com/JohannesLks/CVE-2026-32945](https://github.com/JohannesLks/CVE-2026-32945) :  ![starts](https://img.shields.io/github/stars/JohannesLks/CVE-2026-32945.svg) ![forks](https://img.shields.io/github/forks/JohannesLks/CVE-2026-32945.svg)


## CVE-2026-32746
 telnetd in GNU inetutils through 2.7 allows an out-of-bounds write in the LINEMODE SLC (Set Local Characters) suboption handler because add_slc does not check whether the buffer is full.

- [https://github.com/ekomsSavior/telnet_scan](https://github.com/ekomsSavior/telnet_scan) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/telnet_scan.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/telnet_scan.svg)


## CVE-2026-28858
 A buffer overflow was addressed with improved bounds checking. This issue is fixed in iOS 26.4 and iPadOS 26.4. A remote user may be able to cause unexpected system termination or corrupt kernel memory.

- [https://github.com/kaleth4/CVE-2026-28858](https://github.com/kaleth4/CVE-2026-28858) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-28858.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-28858.svg)


## CVE-2026-27654
 NGINX Open Source and NGINX Plus have a vulnerability in the ngx_http_dav_module module that might allow an attacker to trigger a buffer overflow to the NGINX worker process; this vulnerability may result in termination of the NGINX worker process or modification of source or destination file names outside the document root. This issue affects NGINX Open Source and NGINX Plus when the configuration file uses DAV module MOVE or COPY methods, prefix location (nonregular expression location configuration), and alias directives. The integrity impact is constrained because the NGINX worker process user has low privileges and does not have access to the entire system. Note: Software versions which have reached End of Technical Support (EoTS) are not evaluated.

- [https://github.com/JohannesLks/CVE-2026-27654](https://github.com/JohannesLks/CVE-2026-27654) :  ![starts](https://img.shields.io/github/stars/JohannesLks/CVE-2026-27654.svg) ![forks](https://img.shields.io/github/forks/JohannesLks/CVE-2026-27654.svg)


## CVE-2026-27135
 nghttp2 is an implementation of the Hypertext Transfer Protocol version 2 in C. Prior to version 1.68.1, the nghttp2 library stops reading the incoming data when user facing public API `nghttp2_session_terminate_session` or `nghttp2_session_terminate_session2` is called by the application. They might be called internally by the library when it detects the situation that is subject to connection error. Due to the missing internal state validation, the library keeps reading the rest of the data after one of those APIs is called. Then receiving a malformed frame that causes FRAME_SIZE_ERROR causes assertion failure. nghttp2 v1.68.1 adds missing state validation to avoid assertion failure. No known workarounds are available.

- [https://github.com/Zmo247/nghttp2-cve-2026-27135-patch](https://github.com/Zmo247/nghttp2-cve-2026-27135-patch) :  ![starts](https://img.shields.io/github/stars/Zmo247/nghttp2-cve-2026-27135-patch.svg) ![forks](https://img.shields.io/github/forks/Zmo247/nghttp2-cve-2026-27135-patch.svg)


## CVE-2026-24061
 telnetd in GNU Inetutils through 2.7 allows remote authentication bypass via a "-f root" value for the USER environment variable.

- [https://github.com/ekomsSavior/telnet_scan](https://github.com/ekomsSavior/telnet_scan) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/telnet_scan.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/telnet_scan.svg)


## CVE-2026-22812
 OpenCode is an open source AI coding agent. Prior to 1.0.216, OpenCode automatically starts an unauthenticated HTTP server that allows any local process (or any website via permissive CORS) to execute arbitrary shell commands with the user's privileges. This vulnerability is fixed in 1.0.216.

- [https://github.com/0xBlackash/CVE-2026-22812](https://github.com/0xBlackash/CVE-2026-22812) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-22812.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-22812.svg)


## CVE-2026-20687
 A use after free issue was addressed with improved memory management. This issue is fixed in iOS 18.7.7 and iPadOS 18.7.7, iOS 26.4 and iPadOS 26.4, macOS Sequoia 15.7.5, macOS Tahoe 26.4, tvOS 26.4, watchOS 26.4. An app may be able to cause unexpected system termination or write kernel memory.

- [https://github.com/zeroxjf/CVE-2026-20687-AppleJPEGDriver-UAF](https://github.com/zeroxjf/CVE-2026-20687-AppleJPEGDriver-UAF) :  ![starts](https://img.shields.io/github/stars/zeroxjf/CVE-2026-20687-AppleJPEGDriver-UAF.svg) ![forks](https://img.shields.io/github/forks/zeroxjf/CVE-2026-20687-AppleJPEGDriver-UAF.svg)


## CVE-2026-20637
 A use after free issue was addressed with improved memory management. This issue is fixed in iOS 18.7.7 and iPadOS 18.7.7, iOS 26.3 and iPadOS 26.3, macOS Sequoia 15.7.5, macOS Sonoma 14.8.5, macOS Tahoe 26.3, tvOS 26.3, visionOS 26.3, watchOS 26.3. An app may be able to cause unexpected system termination.

- [https://github.com/zeroxjf/CVE-2026-20637-AppleSEPKeyStore-UAF](https://github.com/zeroxjf/CVE-2026-20637-AppleSEPKeyStore-UAF) :  ![starts](https://img.shields.io/github/stars/zeroxjf/CVE-2026-20637-AppleSEPKeyStore-UAF.svg) ![forks](https://img.shields.io/github/forks/zeroxjf/CVE-2026-20637-AppleSEPKeyStore-UAF.svg)


## CVE-2026-3932
 Insufficient policy enforcement in PDF in Google Chrome on Android prior to 146.0.7680.71 allowed a remote attacker to bypass navigation restrictions via a crafted HTML page. (Chromium security severity: Medium)

- [https://github.com/sm1ee/CVE-2026-39324](https://github.com/sm1ee/CVE-2026-39324) :  ![starts](https://img.shields.io/github/stars/sm1ee/CVE-2026-39324.svg) ![forks](https://img.shields.io/github/forks/sm1ee/CVE-2026-39324.svg)


## CVE-2026-2266
 An improper neutralization of input vulnerability was identified in GitHub Enterprise Server that allowed DOM-based cross-site scripting via task list content. The task list content extraction logic did not properly re-encode browser-decoded text nodes before rendering, allowing user-supplied HTML to be injected into the page. An authenticated attacker could craft malicious task list items in issues or pull requests to execute arbitrary scripts in the context of another user's browser session. This vulnerability affected all versions of GitHub Enterprise Server prior to 3.20 and was fixed in versions 3.18.6 and 3.19.3. This vulnerability was reported via the GitHub Bug Bounty program.

- [https://github.com/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666](https://github.com/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666) :  ![starts](https://img.shields.io/github/stars/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666.svg) ![forks](https://img.shields.io/github/forks/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666.svg)


## CVE-2026-1668
 The web interface on multiple Omada switches does not adequately validate certain external inputs, which may lead to out-of-bound memory access when processing crafted requests.  Under specific conditions, this flaw may result in unintended command execution.brAn unauthenticated attacker with network access to the affected interface may cause memory corruption, service instability, or information disclosure.  Successful exploitation may allow remote code execution or denial-of-service.

- [https://github.com/tangrs/cve-2026-1668-poc](https://github.com/tangrs/cve-2026-1668-poc) :  ![starts](https://img.shields.io/github/stars/tangrs/cve-2026-1668-poc.svg) ![forks](https://img.shields.io/github/forks/tangrs/cve-2026-1668-poc.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-canary-15x.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg)


## CVE-2025-49844
 Redis is an open source, in-memory database that persists on disk. Versions 8.2.1 and below allow an authenticated user to use a specially crafted Lua script to manipulate the garbage collector, trigger a use-after-free and potentially lead to remote code execution. The problem exists in all versions of Redis with Lua scripting. This issue is fixed in version 8.2.2. To workaround this issue without patching the redis-server executable is to prevent users from executing Lua scripts. This can be done using ACL to restrict EVAL and EVALSHA commands.

- [https://github.com/dajneem23/CVE-2025-49844](https://github.com/dajneem23/CVE-2025-49844) :  ![starts](https://img.shields.io/github/stars/dajneem23/CVE-2025-49844.svg) ![forks](https://img.shields.io/github/forks/dajneem23/CVE-2025-49844.svg)


## CVE-2025-48734
 2.x are recommended to upgrade to version 2.0.0-M2, which fixes the issue.

- [https://github.com/h3raklez/CVE-2025-48734](https://github.com/h3raklez/CVE-2025-48734) :  ![starts](https://img.shields.io/github/stars/h3raklez/CVE-2025-48734.svg) ![forks](https://img.shields.io/github/forks/h3raklez/CVE-2025-48734.svg)


## CVE-2025-32433
 Erlang/OTP is a set of libraries for the Erlang programming language. Prior to versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20, a SSH server may allow an attacker to perform unauthenticated remote code execution (RCE). By exploiting a flaw in SSH protocol message handling, a malicious actor could gain unauthorized access to affected systems and execute arbitrary commands without valid credentials. This issue is patched in versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20. A temporary workaround involves disabling the SSH server or to prevent access via firewall rules.

- [https://github.com/ekomsSavior/POC_CVE-2025-32433](https://github.com/ekomsSavior/POC_CVE-2025-32433) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/POC_CVE-2025-32433.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/POC_CVE-2025-32433.svg)


## CVE-2025-30065
Users are recommended to upgrade to version 1.15.1, which fixes the issue.

- [https://github.com/micrictor/parquet-avro-rce](https://github.com/micrictor/parquet-avro-rce) :  ![starts](https://img.shields.io/github/stars/micrictor/parquet-avro-rce.svg) ![forks](https://img.shields.io/github/forks/micrictor/parquet-avro-rce.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/elshaheedy/CVE-2025-29927-Sigma-Rule](https://github.com/elshaheedy/CVE-2025-29927-Sigma-Rule) :  ![starts](https://img.shields.io/github/stars/elshaheedy/CVE-2025-29927-Sigma-Rule.svg) ![forks](https://img.shields.io/github/forks/elshaheedy/CVE-2025-29927-Sigma-Rule.svg)
- [https://github.com/MKIRAHMET/CVE-2025-29927-PoC](https://github.com/MKIRAHMET/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/MKIRAHMET/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/MKIRAHMET/CVE-2025-29927-PoC.svg)


## CVE-2025-24252
 A use-after-free issue was addressed with improved memory management. This issue is fixed in iOS 18.4 and iPadOS 18.4, iPadOS 17.7.6, macOS Sequoia 15.4, macOS Sonoma 14.7.5, macOS Ventura 13.7.5, tvOS 18.4, visionOS 2.4. An attacker on the local network may be able to corrupt process memory.

- [https://github.com/ekomsSavior/AirBorne-PoC](https://github.com/ekomsSavior/AirBorne-PoC) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/AirBorne-PoC.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/AirBorne-PoC.svg)


## CVE-2025-24132
 The issue was addressed with improved memory handling. This issue is fixed in AirPlay audio SDK 2.7.1 and AirPlay video SDK 3.6.0.126. An attacker on the local network may cause an unexpected app termination.

- [https://github.com/ekomsSavior/AirBorne-PoC](https://github.com/ekomsSavior/AirBorne-PoC) :  ![starts](https://img.shields.io/github/stars/ekomsSavior/AirBorne-PoC.svg) ![forks](https://img.shields.io/github/forks/ekomsSavior/AirBorne-PoC.svg)


## CVE-2025-23061
 Mongoose before 8.9.5 can improperly use a nested $where filter with a populate() match, leading to search injection. NOTE: this issue exists because of an incomplete fix for CVE-2024-53900.

- [https://github.com/amikanev/CVE-2025-23061-LAB](https://github.com/amikanev/CVE-2025-23061-LAB) :  ![starts](https://img.shields.io/github/stars/amikanev/CVE-2025-23061-LAB.svg) ![forks](https://img.shields.io/github/forks/amikanev/CVE-2025-23061-LAB.svg)


## CVE-2025-14847
 Mismatched length fields in Zlib compressed protocol headers may allow a read of uninitialized heap memory by an unauthenticated client. This issue affects all MongoDB Server v7.0 prior to 7.0.28 versions, MongoDB Server v8.0 versions prior to 8.0.17, MongoDB Server v8.2 versions prior to 8.2.3, MongoDB Server v6.0 versions prior to 6.0.27, MongoDB Server v5.0 versions prior to 5.0.32, MongoDB Server v4.4 versions prior to 4.4.30, MongoDB Server v4.2 versions greater than or equal to 4.2.0, MongoDB Server v4.0 versions greater than or equal to 4.0.0, and MongoDB Server v3.6 versions greater than or equal to 3.6.0.

- [https://github.com/dawnsmithcyber/azure-vulnerability-remediation-project](https://github.com/dawnsmithcyber/azure-vulnerability-remediation-project) :  ![starts](https://img.shields.io/github/stars/dawnsmithcyber/azure-vulnerability-remediation-project.svg) ![forks](https://img.shields.io/github/forks/dawnsmithcyber/azure-vulnerability-remediation-project.svg)


## CVE-2025-1974
 A security issue was discovered in Kubernetes where under certain conditions, an unauthenticated attacker with access to the pod network can achieve arbitrary code execution in the context of the ingress-nginx controller. This can lead to disclosure of Secrets accessible to the controller. (Note that in the default installation, the controller can access all Secrets cluster-wide.)

- [https://github.com/zsxen/CVE-2025-1974](https://github.com/zsxen/CVE-2025-1974) :  ![starts](https://img.shields.io/github/stars/zsxen/CVE-2025-1974.svg) ![forks](https://img.shields.io/github/forks/zsxen/CVE-2025-1974.svg)
- [https://github.com/zsxen/cve-2025-1974-lab](https://github.com/zsxen/cve-2025-1974-lab) :  ![starts](https://img.shields.io/github/stars/zsxen/cve-2025-1974-lab.svg) ![forks](https://img.shields.io/github/forks/zsxen/cve-2025-1974-lab.svg)


## CVE-2024-52301
 Laravel is a web application framework. When the register_argc_argv php directive is set to on , and users call any URL with a special crafted query string, they are able to change the environment used by the framework when handling the request. The vulnerability fixed in 6.20.45, 7.30.7, 8.83.28, 9.52.17, 10.48.23, and 11.31.0. The framework now ignores argv values for environment detection on non-cli SAPIs.

- [https://github.com/fckoo/nanwinata-CVE-2024-52301](https://github.com/fckoo/nanwinata-CVE-2024-52301) :  ![starts](https://img.shields.io/github/stars/fckoo/nanwinata-CVE-2024-52301.svg) ![forks](https://img.shields.io/github/forks/fckoo/nanwinata-CVE-2024-52301.svg)


## CVE-2024-38063
 Windows TCP/IP Remote Code Execution Vulnerability

- [https://github.com/cyberzeuspakistan/CVE-2024-38063-Research-Tool](https://github.com/cyberzeuspakistan/CVE-2024-38063-Research-Tool) :  ![starts](https://img.shields.io/github/stars/cyberzeuspakistan/CVE-2024-38063-Research-Tool.svg) ![forks](https://img.shields.io/github/forks/cyberzeuspakistan/CVE-2024-38063-Research-Tool.svg)


## CVE-2024-29988
 SmartScreen Prompt Security Feature Bypass Vulnerability

- [https://github.com/avitoriagomes/CVE-2024-29988](https://github.com/avitoriagomes/CVE-2024-29988) :  ![starts](https://img.shields.io/github/stars/avitoriagomes/CVE-2024-29988.svg) ![forks](https://img.shields.io/github/forks/avitoriagomes/CVE-2024-29988.svg)


## CVE-2024-3400
Cloud NGFW, Panorama appliances, and Prisma Access are not impacted by this vulnerability.

- [https://github.com/SimoesCTT/-CTT-PAN-OS-EXPLOIT-CVE-2024-340](https://github.com/SimoesCTT/-CTT-PAN-OS-EXPLOIT-CVE-2024-340) :  ![starts](https://img.shields.io/github/stars/SimoesCTT/-CTT-PAN-OS-EXPLOIT-CVE-2024-340.svg) ![forks](https://img.shields.io/github/forks/SimoesCTT/-CTT-PAN-OS-EXPLOIT-CVE-2024-340.svg)


## CVE-2023-50094
 reNgine before 2.1.2 allows OS Command Injection if an adversary has a valid session ID. The attack places shell metacharacters in an api/tools/waf_detector/?url= string. The commands are executed as root via subprocess.check_output.

- [https://github.com/Zierax/CVE-2023-50094_POC](https://github.com/Zierax/CVE-2023-50094_POC) :  ![starts](https://img.shields.io/github/stars/Zierax/CVE-2023-50094_POC.svg) ![forks](https://img.shields.io/github/forks/Zierax/CVE-2023-50094_POC.svg)


## CVE-2023-32749
 Pydio Cells allows users by default to create so-called external users in order to share files with them. By modifying the HTTP request sent when creating such an external user, it is possible to assign the new user arbitrary roles. By assigning all roles to a newly created user, access to all cells and non-personal workspaces is granted.

- [https://github.com/alaeddine03/CVE-2023-32749-PoC](https://github.com/alaeddine03/CVE-2023-32749-PoC) :  ![starts](https://img.shields.io/github/stars/alaeddine03/CVE-2023-32749-PoC.svg) ![forks](https://img.shields.io/github/forks/alaeddine03/CVE-2023-32749-PoC.svg)


## CVE-2023-27997
 A heap-based buffer overflow vulnerability [CWE-122] in FortiOS version 7.2.4 and below, version 7.0.11 and below, version 6.4.12 and below, version 6.0.16 and below and FortiProxy version 7.2.3 and below, version 7.0.9 and below, version 2.0.12 and below, version 1.2 all versions, version 1.1 all versions SSL-VPN may allow a remote attacker to execute arbitrary code or commands via specifically crafted requests.

- [https://github.com/george1-adel/CVE-2023-27997](https://github.com/george1-adel/CVE-2023-27997) :  ![starts](https://img.shields.io/github/stars/george1-adel/CVE-2023-27997.svg) ![forks](https://img.shields.io/github/forks/george1-adel/CVE-2023-27997.svg)


## CVE-2023-23946
 Git, a revision control system, is vulnerable to path traversal prior to versions 2.39.2, 2.38.4, 2.37.6, 2.36.5, 2.35.7, 2.34.7, 2.33.7, 2.32.6, 2.31.7, and 2.30.8. By feeding a crafted input to `git apply`, a path outside the working tree can be overwritten as the user who is running `git apply`. A fix has been prepared and will appear in v2.39.2, v2.38.4, v2.37.6, v2.36.5, v2.35.7, v2.34.7, v2.33.7, v2.32.6, v2.31.7, and v2.30.8. As a workaround, use `git apply --stat` to inspect a patch before applying; avoid applying one that creates a symbolic link and then creates a file beyond the symbolic link.

- [https://github.com/mararaEd/HTB-Snoopy-Writeup](https://github.com/mararaEd/HTB-Snoopy-Writeup) :  ![starts](https://img.shields.io/github/stars/mararaEd/HTB-Snoopy-Writeup.svg) ![forks](https://img.shields.io/github/forks/mararaEd/HTB-Snoopy-Writeup.svg)


## CVE-2023-20052
 This vulnerability is due to enabling XML entity substitution that may result in XML external entity injection. An attacker could exploit this vulnerability by submitting a crafted DMG file to be scanned by ClamAV on an affected device. A successful exploit could allow the attacker to leak bytes from any file that may be read by the ClamAV scanning process.

- [https://github.com/mararaEd/HTB-Snoopy-Writeup](https://github.com/mararaEd/HTB-Snoopy-Writeup) :  ![starts](https://img.shields.io/github/stars/mararaEd/HTB-Snoopy-Writeup.svg) ![forks](https://img.shields.io/github/forks/mararaEd/HTB-Snoopy-Writeup.svg)


## CVE-2023-6246
 A heap-based buffer overflow was found in the __vsyslog_internal function of the glibc library. This function is called by the syslog and vsyslog functions. This issue occurs when the openlog function was not called, or called with the ident argument set to NULL, and the program name (the basename of argv[0]) is bigger than 1024 bytes, resulting in an application crash or local privilege escalation. This issue affects glibc 2.36 and newer.

- [https://github.com/SimoesCTT/CTT-Vsyslog-Vortex-CVE-2023-6246](https://github.com/SimoesCTT/CTT-Vsyslog-Vortex-CVE-2023-6246) :  ![starts](https://img.shields.io/github/stars/SimoesCTT/CTT-Vsyslog-Vortex-CVE-2023-6246.svg) ![forks](https://img.shields.io/github/forks/SimoesCTT/CTT-Vsyslog-Vortex-CVE-2023-6246.svg)


## CVE-2018-13379
 An Improper Limitation of a Pathname to a Restricted Directory ("Path Traversal") in Fortinet FortiOS 6.0.0 to 6.0.4, 5.6.3 to 5.6.7 and 5.4.6 to 5.4.12 and FortiProxy 2.0.0, 1.2.0 to 1.2.8, 1.1.0 to 1.1.6, 1.0.0 to 1.0.7 under SSL VPN web portal allows an unauthenticated attacker to download system files via special crafted HTTP resource requests.

- [https://github.com/Zierax/CVE-2018-13379](https://github.com/Zierax/CVE-2018-13379) :  ![starts](https://img.shields.io/github/stars/Zierax/CVE-2018-13379.svg) ![forks](https://img.shields.io/github/forks/Zierax/CVE-2018-13379.svg)


## CVE-2017-11499
 Node.js v4.0 through v4.8.3, all versions of v5.x, v6.0 through v6.11.0, v7.0 through v7.10.0, and v8.0 through v8.1.3 was susceptible to hash flooding remote DoS attacks as the HashTable seed was constant across a given released version of Node.js. This was a result of building with V8 snapshots enabled by default which caused the initially randomized seed to be overwritten on startup.

- [https://github.com/dajneem23/CVE-2017-11499](https://github.com/dajneem23/CVE-2017-11499) :  ![starts](https://img.shields.io/github/stars/dajneem23/CVE-2017-11499.svg) ![forks](https://img.shields.io/github/forks/dajneem23/CVE-2017-11499.svg)


## CVE-2011-2523
 vsftpd 2.3.4 downloaded between 20110630 and 20110703 contains a backdoor which opens a shell on port 6200/tcp.

- [https://github.com/RinAliyeva/metasploitable2-vsftpd-exploitation](https://github.com/RinAliyeva/metasploitable2-vsftpd-exploitation) :  ![starts](https://img.shields.io/github/stars/RinAliyeva/metasploitable2-vsftpd-exploitation.svg) ![forks](https://img.shields.io/github/forks/RinAliyeva/metasploitable2-vsftpd-exploitation.svg)

