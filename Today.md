# Update 2026-04-28
## CVE-2026-41242
 protobufjs compiles protobuf definitions into JavaScript (JS) functions. In versions prior to 8.0.1 and 7.5.5, attackers can inject arbitrary code in the "type" fields of protobuf definitions, which will then execute during object decoding using that definition. Versions 8.0.1 and 7.5.5 patch the issue.

- [https://github.com/4chech/CVE-2026-41242](https://github.com/4chech/CVE-2026-41242) :  ![starts](https://img.shields.io/github/stars/4chech/CVE-2026-41242.svg) ![forks](https://img.shields.io/github/forks/4chech/CVE-2026-41242.svg)


## CVE-2026-39987
 marimo is a reactive Python notebook. Prior to 0.23.0, Marimo has a Pre-Auth RCE vulnerability. The terminal WebSocket endpoint /terminal/ws lacks authentication validation, allowing an unauthenticated attacker to obtain a full PTY shell and execute arbitrary system commands. Unlike other WebSocket endpoints (e.g., /ws) that correctly call validate_auth() for authentication, the /terminal/ws endpoint only checks the running mode and platform support before accepting connections, completely skipping authentication verification. This vulnerability is fixed in 0.23.0.

- [https://github.com/Dhiaelhak-Rached/CVE-2026-39987-lab-or-marimo-cve-lab](https://github.com/Dhiaelhak-Rached/CVE-2026-39987-lab-or-marimo-cve-lab) :  ![starts](https://img.shields.io/github/stars/Dhiaelhak-Rached/CVE-2026-39987-lab-or-marimo-cve-lab.svg) ![forks](https://img.shields.io/github/forks/Dhiaelhak-Rached/CVE-2026-39987-lab-or-marimo-cve-lab.svg)


## CVE-2026-29057
 Next.js is a React framework for building full-stack web applications. Starting in version 9.5.0 and prior to versions 15.5.13 and 16.1.7, when Next.js rewrites proxy traffic to an external backend, a crafted `DELETE`/`OPTIONS` request using `Transfer-Encoding: chunked` could trigger request boundary disagreement between the proxy and backend. This could allow request smuggling through rewritten routes. An attacker could smuggle a second request to unintended backend routes (for example, internal/admin endpoints), bypassing assumptions that only the configured rewrite destination/path is reachable. This does not impact applications hosted on providers that handle rewrites at the CDN level, such as Vercel.  The vulnerability originated in an upstream library vendored by Next.js. It is fixed in Next.js 15.5.13 and 16.1.7 by updating that dependency’s behavior so `content-length: 0` is added only when both `content-length` and `transfer-encoding` are absent, and `transfer-encoding` is no longer removed in that code path. If upgrading is not immediately possible, block chunked `DELETE`/`OPTIONS` requests on rewritten routes at the edge/proxy, and/or enforce authentication/authorization on backend routes.

- [https://github.com/Nayekah/Next.js-Proof-of-Concept](https://github.com/Nayekah/Next.js-Proof-of-Concept) :  ![starts](https://img.shields.io/github/stars/Nayekah/Next.js-Proof-of-Concept.svg) ![forks](https://img.shields.io/github/forks/Nayekah/Next.js-Proof-of-Concept.svg)


## CVE-2026-27978
 Next.js is a React framework for building full-stack web applications. Starting in version 16.0.1 and prior to version 16.1.7, `origin: null` was treated as a "missing" origin during Server Action CSRF validation. As a result, requests from opaque contexts (such as sandboxed iframes) could bypass origin verification instead of being validated as cross-origin requests. An attacker could induce a victim browser to submit Server Actions from a sandboxed context, potentially executing state-changing actions with victim credentials (CSRF). This is fixed in version 16.1.7 by treating `'null'` as an explicit origin value and enforcing host/origin checks unless `'null'` is explicitly allowlisted in `experimental.serverActions.allowedOrigins`. If upgrading is not immediately possible, add CSRF tokens for sensitive Server Actions, prefer `SameSite=Strict` on sensitive auth cookies, and/or do not allow `'null'` in `serverActions.allowedOrigins` unless intentionally required and additionally protected.

- [https://github.com/Nayekah/Next.js-Proof-of-Concept](https://github.com/Nayekah/Next.js-Proof-of-Concept) :  ![starts](https://img.shields.io/github/stars/Nayekah/Next.js-Proof-of-Concept.svg) ![forks](https://img.shields.io/github/forks/Nayekah/Next.js-Proof-of-Concept.svg)


## CVE-2026-21877
 n8n is an open source workflow automation platform. In versions 0.121.2 and below, an authenticated attacker may be able to execute malicious code using the n8n service. This could result in full compromise and can impact both self-hosted and n8n Cloud instances. This issue is fixed in version 1.121.3. Administrators can reduce exposure by disabling the Git node and limiting access for untrusted users, but upgrading to the latest version is recommended.

- [https://github.com/monkeontheroof/cve-2026-21877-rce](https://github.com/monkeontheroof/cve-2026-21877-rce) :  ![starts](https://img.shields.io/github/stars/monkeontheroof/cve-2026-21877-rce.svg) ![forks](https://img.shields.io/github/forks/monkeontheroof/cve-2026-21877-rce.svg)


## CVE-2026-7028
 A security flaw has been discovered in CodeAstro Online Job Portal 1.0. The affected element is an unknown function of the file /admin/jobs-admins/delete-jobs.php of the component All Jobs Page. Performing a manipulation of the argument ID results in sql injection. The attack is possible to be carried out remotely. The exploit has been released to the public and may be used for attacks.

- [https://github.com/Xmyronn/CVE-2026-7028-SQLI](https://github.com/Xmyronn/CVE-2026-7028-SQLI) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-7028-SQLI.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-7028-SQLI.svg)


## CVE-2026-7020
 A security flaw has been discovered in Ollama up to 0.20.2. This affects the function digestToPath of the file x/imagegen/transfer/transfer.go of the component Tensor Model Transfer Handler. The manipulation of the argument digest results in path traversal. The attack may be performed from remote. This attack is characterized by high complexity. The exploitability is reported as difficult. The exploit has been released to the public and may be used for attacks. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/davidrxchester/CVE-2026-7020](https://github.com/davidrxchester/CVE-2026-7020) :  ![starts](https://img.shields.io/github/stars/davidrxchester/CVE-2026-7020.svg) ![forks](https://img.shields.io/github/forks/davidrxchester/CVE-2026-7020.svg)


## CVE-2026-1207
Django would like to thank Tarek Nakkouch for reporting this issue.

- [https://github.com/sw0rd1ight/CVE-2026-1207](https://github.com/sw0rd1ight/CVE-2026-1207) :  ![starts](https://img.shields.io/github/stars/sw0rd1ight/CVE-2026-1207.svg) ![forks](https://img.shields.io/github/forks/sw0rd1ight/CVE-2026-1207.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg)


## CVE-2025-60787
 MotionEye v0.43.1b4 and before is vulnerable to OS Command Injection in configuration parameters such as image_file_name. Unsanitized user input is written to Motion configuration files, allowing remote authenticated attackers with admin access to achieve code execution when Motion is restarted.

- [https://github.com/Revnin/CCTV-MACHINE](https://github.com/Revnin/CCTV-MACHINE) :  ![starts](https://img.shields.io/github/stars/Revnin/CCTV-MACHINE.svg) ![forks](https://img.shields.io/github/forks/Revnin/CCTV-MACHINE.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-29631
 Gardyn Home Kit firmware before master.619, Home Kit Mobile Application before 2.11.0, and Home Kit Cloud API before 2.12.2026 allow command injection through vulnerable methods that do not sanitize input before passing content to the operating system for execution. The vulnerability may allow an attacker to execute arbitrary operating system commands on a target Home Kit.

- [https://github.com/mselbrede/gardyn](https://github.com/mselbrede/gardyn) :  ![starts](https://img.shields.io/github/stars/mselbrede/gardyn.svg) ![forks](https://img.shields.io/github/forks/mselbrede/gardyn.svg)


## CVE-2025-29630
 DO NOT USE THIS CANDIDATE NUMBER. ConsultIDs: none. Reason: This candidate was withdrawn by its CNA. Further investigation showed that it was not a security issue; there is no indication that an applicable SSH private key has ever been compromised. Notes: none.

- [https://github.com/mselbrede/gardyn](https://github.com/mselbrede/gardyn) :  ![starts](https://img.shields.io/github/stars/mselbrede/gardyn.svg) ![forks](https://img.shields.io/github/forks/mselbrede/gardyn.svg)


## CVE-2025-29629
 Gardyn Home Kit firmware before master.619, Home Kit Mobile Application before 2.11.0, and Home Kit Cloud API before 2.12.2026 use weak default credentials for secure shell access. This may result in attackers gaining access to exposed Gardyn Home Kits.

- [https://github.com/mselbrede/gardyn](https://github.com/mselbrede/gardyn) :  ![starts](https://img.shields.io/github/stars/mselbrede/gardyn.svg) ![forks](https://img.shields.io/github/forks/mselbrede/gardyn.svg)


## CVE-2025-29628
 A Gardyn Azure IoT Hub connection string is downloaded over an insecure HTTP connection in Gardyn Home Kit firmware before master.619, Home Kit Mobile Application before 2.11.0, and Home Kit Cloud API before 2.12.2026 leaving the string vulnerable to interception and modification through a Man-in-the-Middle attack. This may result in the attacker capturing device credentials or taking control of vulnerable home kits.

- [https://github.com/mselbrede/gardyn](https://github.com/mselbrede/gardyn) :  ![starts](https://img.shields.io/github/stars/mselbrede/gardyn.svg) ![forks](https://img.shields.io/github/forks/mselbrede/gardyn.svg)


## CVE-2025-8061
 A potential insufficient access control vulnerability was reported in the Lenovo Dispatcher 3.0 and Dispatcher 3.1 drivers used by some Lenovo consumer notebooks that could allow an authenticated local user to execute code with elevated privileges. The Lenovo Dispatcher 3.2 driver is not affected. This vulnerability does not affect systems when the Windows feature Core Isolation Memory Integrity is enabled. Lenovo systems preloaded with Windows 11 have this feature enabled by default.

- [https://github.com/vxqs/Lenovo-CVE-2025-8061](https://github.com/vxqs/Lenovo-CVE-2025-8061) :  ![starts](https://img.shields.io/github/stars/vxqs/Lenovo-CVE-2025-8061.svg) ![forks](https://img.shields.io/github/forks/vxqs/Lenovo-CVE-2025-8061.svg)


## CVE-2024-51482
 ZoneMinder is a free, open source closed-circuit television software application. ZoneMinder v1.37.* = 1.37.64 is vulnerable to boolean-based SQL Injection in function of web/ajax/event.php. This is fixed in 1.37.65.

- [https://github.com/Revnin/CCTV-MACHINE](https://github.com/Revnin/CCTV-MACHINE) :  ![starts](https://img.shields.io/github/stars/Revnin/CCTV-MACHINE.svg) ![forks](https://img.shields.io/github/forks/Revnin/CCTV-MACHINE.svg)


## CVE-2024-3273
 ** UNSUPPORTED WHEN ASSIGNED ** A vulnerability, which was classified as critical, was found in D-Link DNS-320L, DNS-325, DNS-327L and DNS-340L up to 20240403. Affected is an unknown function of the file /cgi-bin/nas_sharing.cgi of the component HTTP GET Request Handler. The manipulation of the argument system leads to command injection. It is possible to launch the attack remotely. The exploit has been disclosed to the public and may be used. The identifier of this vulnerability is VDB-259284. NOTE: This vulnerability only affects products that are no longer supported by the maintainer. NOTE: Vendor was contacted early and confirmed immediately that the product is end-of-life. It should be retired and replaced.

- [https://github.com/askhatov21/Best-Practices-Cybersecurity-Otanata-Project](https://github.com/askhatov21/Best-Practices-Cybersecurity-Otanata-Project) :  ![starts](https://img.shields.io/github/stars/askhatov21/Best-Practices-Cybersecurity-Otanata-Project.svg) ![forks](https://img.shields.io/github/forks/askhatov21/Best-Practices-Cybersecurity-Otanata-Project.svg)


## CVE-2022-23636
 Wasmtime is an open source runtime for WebAssembly & WASI. Prior to versions 0.34.1 and 0.33.1, there exists a bug in the pooling instance allocator in Wasmtime's runtime where a failure to instantiate an instance for a module that defines an `externref` global will result in an invalid drop of a `VMExternRef` via an uninitialized pointer. A number of conditions listed in the GitHub Security Advisory must be true in order for an instance to be vulnerable to this issue. Maintainers believe that the effective impact of this bug is relatively small because the usage of `externref` is still uncommon and without a resource limiter configured on the `Store`, which is not the default configuration, it is only possible to trigger the bug from an error returned by `mprotect` or `VirtualAlloc`. Note that on Linux with the `uffd` feature enabled, it is only possible to trigger the bug from a resource limiter as the call to `mprotect` is skipped. The bug has been fixed in 0.34.1 and 0.33.1 and users are encouraged to upgrade as soon as possible. If it is not possible to upgrade to version 0.34.1 or 0.33.1 of the `wasmtime` crate, it is recommend that support for the reference types proposal be disabled by passing `false` to `Config::wasm_reference_types`. Doing so will prevent modules that use `externref` from being loaded entirely.

- [https://github.com/cyhe50/cve-2022-23636-poc](https://github.com/cyhe50/cve-2022-23636-poc) :  ![starts](https://img.shields.io/github/stars/cyhe50/cve-2022-23636-poc.svg) ![forks](https://img.shields.io/github/forks/cyhe50/cve-2022-23636-poc.svg)


## CVE-2022-22965
 A Spring MVC or Spring WebFlux application running on JDK 9+ may be vulnerable to remote code execution (RCE) via data binding. The specific exploit requires the application to run on Tomcat as a WAR deployment. If the application is deployed as a Spring Boot executable jar, i.e. the default, it is not vulnerable to the exploit. However, the nature of the vulnerability is more general, and there may be other ways to exploit it.

- [https://github.com/Aur3ns/Block-Spring4Shell](https://github.com/Aur3ns/Block-Spring4Shell) :  ![starts](https://img.shields.io/github/stars/Aur3ns/Block-Spring4Shell.svg) ![forks](https://img.shields.io/github/forks/Aur3ns/Block-Spring4Shell.svg)

