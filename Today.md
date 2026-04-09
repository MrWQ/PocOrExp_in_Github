# Update 2026-04-09
## CVE-2026-39371
 RedwoodSDK is a server-first React framework. From 1.0.0-beta.50 to 1.0.5, erver functions exported from "use server" files could be invoked via GET requests, bypassing their intended HTTP method. In cookie-authenticated applications, this allowed cross-site GET navigations to trigger state-changing functions, because browsers send SameSite=Lax cookies on top-level GET requests. This affected all server functions -- both serverAction() handlers and bare exported functions in "use server" files. This vulnerability is fixed in 1.0.6.

- [https://github.com/zebbernCVE/CVE-2026-39371](https://github.com/zebbernCVE/CVE-2026-39371) :  ![starts](https://img.shields.io/github/stars/zebbernCVE/CVE-2026-39371.svg) ![forks](https://img.shields.io/github/forks/zebbernCVE/CVE-2026-39371.svg)


## CVE-2026-39324
 Rack::Session is a session management implementation for Rack. From 2.0.0 to before 2.1.2, Rack::Session::Cookie incorrectly handles decryption failures when configured with secrets:. If cookie decryption fails, the implementation falls back to a default decoder instead of rejecting the cookie. This allows an unauthenticated attacker to supply a crafted session cookie that is accepted as valid session data without knowledge of any configured secret. Because this mechanism is used to load session state, an attacker can manipulate session contents and potentially gain unauthorized access. This vulnerability is fixed in 2.1.2.

- [https://github.com/sm1ee/CVE-2026-39324](https://github.com/sm1ee/CVE-2026-39324) :  ![starts](https://img.shields.io/github/stars/sm1ee/CVE-2026-39324.svg) ![forks](https://img.shields.io/github/forks/sm1ee/CVE-2026-39324.svg)


## CVE-2026-35492
 Kedro-Datasets is a Kendo plugin providing data connectors. Prior to 9.3.0, PartitionedDataset in kedro-datasets was vulnerable to path traversal. Partition IDs were concatenated directly with the dataset base path without validation. An attacker or malicious input containing .. components in a partition ID could cause files to be written outside the configured dataset directory, potentially overwriting arbitrary files on the filesystem. Users of PartitionedDataset with any storage backend (local filesystem, S3, GCS, etc.) are affected. This vulnerability is fixed in 9.3.0.

- [https://github.com/redyank/CVE-2026-35492](https://github.com/redyank/CVE-2026-35492) :  ![starts](https://img.shields.io/github/stars/redyank/CVE-2026-35492.svg) ![forks](https://img.shields.io/github/forks/redyank/CVE-2026-35492.svg)


## CVE-2026-34156
 NocoBase is an AI-powered no-code/low-code platform for building business applications and enterprise solutions. Prior to version 2.0.28, NocoBase's Workflow Script Node executes user-supplied JavaScript inside a Node.js vm sandbox with a custom require allowlist (controlled by WORKFLOW_SCRIPT_MODULES env var). However, the console object passed into the sandbox context exposes host-realm WritableWorkerStdio stream objects via console._stdout and console._stderr. An authenticated attacker can traverse the prototype chain to escape the sandbox and achieve Remote Code Execution as root. This issue has been patched in version 2.0.28.

- [https://github.com/franckboumendil/CVE-2026-34156](https://github.com/franckboumendil/CVE-2026-34156) :  ![starts](https://img.shields.io/github/stars/franckboumendil/CVE-2026-34156.svg) ![forks](https://img.shields.io/github/forks/franckboumendil/CVE-2026-34156.svg)


## CVE-2026-33017
 Langflow is a tool for building and deploying AI-powered agents and workflows. In versions prior to 1.9.0, the POST /api/v1/build_public_tmp/{flow_id}/flow endpoint allows building public flows without requiring authentication. When the optional data parameter is supplied, the endpoint uses attacker-controlled flow data (containing arbitrary Python code in node definitions) instead of the stored flow data from the database. This code is passed to exec() with zero sandboxing, resulting in unauthenticated remote code execution. This is distinct from CVE-2025-3248, which fixed /api/v1/validate/code by adding authentication. The build_public_tmp endpoint is designed to be unauthenticated (for public flows) but incorrectly accepts attacker-supplied flow data containing arbitrary executable code. This issue has been fixed in version 1.9.0.

- [https://github.com/masterwok/CVE-2026-33017-Langflow-POC](https://github.com/masterwok/CVE-2026-33017-Langflow-POC) :  ![starts](https://img.shields.io/github/stars/masterwok/CVE-2026-33017-Langflow-POC.svg) ![forks](https://img.shields.io/github/forks/masterwok/CVE-2026-33017-Langflow-POC.svg)


## CVE-2026-29059
 Windmill is an open-source developer platform for internal code: APIs, background jobs, workflows and UIs. Prior to version 1.603.3, an unauthenticated path traversal vulnerability exists in Windmill's get_log_file endpoint "(/api/w/{workspace}/jobs_u/get_log_file/{filename})". The filename parameter is concatenated into a file path without sanitization, allowing an attacker to read arbitrary files on the server using ../ sequences. This issue has been patched in version 1.603.3.

- [https://github.com/Chocapikk/Windfall](https://github.com/Chocapikk/Windfall) :  ![starts](https://img.shields.io/github/stars/Chocapikk/Windfall.svg) ![forks](https://img.shields.io/github/forks/Chocapikk/Windfall.svg)


## CVE-2026-25994
 PJSIP is a free and open source multimedia communication library written in C. In 2.16 and earlier, a buffer overflow vulnerability exists in PJNATH ICE Session when processing credentials with excessively long usernames.

- [https://github.com/VABISMO/cve-2026-25994_PJSIP](https://github.com/VABISMO/cve-2026-25994_PJSIP) :  ![starts](https://img.shields.io/github/stars/VABISMO/cve-2026-25994_PJSIP.svg) ![forks](https://img.shields.io/github/forks/VABISMO/cve-2026-25994_PJSIP.svg)


## CVE-2026-23696
 Windmill CE and EE versions 1.276.0 through 1.603.2 contain an SQL injection vulnerability in the folder ownership management functionality that allows authenticated attackers to inject SQL through the owner parameter. An attacker can use the injection to read sensitive data such as the JWT signing secret and administrative user identifiers, forge an administrative token, and then execute arbitrary code via the workflow execution endpoints.

- [https://github.com/Chocapikk/Windfall](https://github.com/Chocapikk/Windfall) :  ![starts](https://img.shields.io/github/stars/Chocapikk/Windfall.svg) ![forks](https://img.shields.io/github/forks/Chocapikk/Windfall.svg)


## CVE-2026-23524
 Laravel Reverb provides a real-time WebSocket communication backend for Laravel applications. In versions 1.6.3 and below, Reverb passes data from the Redis channel directly into PHP’s unserialize() function without restricting which classes can be instantiated, which leaves users vulnerable to Remote Code Execution. The exploitability of this vulnerability is increased because Redis servers are commonly deployed without authentication, but only affects Laravel Reverb when horizontal scaling is enabled (REVERB_SCALING_ENABLED=true). This issue has been fixed in version 1.7.0. As a workaround, require a strong password for Redis access and ensure the service is only accessible via a private network or local loopback, and/or set REVERB_SCALING_ENABLED=false to bypass the vulnerable logic entirely (if the environment uses only one Reverb node).

- [https://github.com/rockmelodies/CVE-2026-23524](https://github.com/rockmelodies/CVE-2026-23524) :  ![starts](https://img.shields.io/github/stars/rockmelodies/CVE-2026-23524.svg) ![forks](https://img.shields.io/github/forks/rockmelodies/CVE-2026-23524.svg)


## CVE-2026-22732
: from 5.7.0 through 5.7.21, from 5.8.0 through 5.8.23, from 6.3.0 through 6.3.14, from 6.4.0 through 6.4.14, from 6.5.0 through 6.5.8, from 7.0.0 through 7.0.3.

- [https://github.com/semgrep/cve-2026-22732-demo](https://github.com/semgrep/cve-2026-22732-demo) :  ![starts](https://img.shields.io/github/stars/semgrep/cve-2026-22732-demo.svg) ![forks](https://img.shields.io/github/forks/semgrep/cve-2026-22732-demo.svg)


## CVE-2026-22683
 Windmill versions 1.56.0 through 1.614.0 contain a missing authorization vulnerability that allows users with the Operator role to perform prohibited entity creation and modification actions via the backend API. Although Operators are documented and priced as unable to create or modify entities, the API does not enforce the Operator restriction on workspace endpoints, allowing an Operator to create and update scripts, flows, apps, and raw_apps. Since Operators can also execute scripts via the jobs API, this allows direct privilege escalation to remote code execution within the Windmill deployment. This vulnerability has existed since the introduction of the Operator role in version 1.56.0.

- [https://github.com/Chocapikk/Windfall](https://github.com/Chocapikk/Windfall) :  ![starts](https://img.shields.io/github/stars/Chocapikk/Windfall.svg) ![forks](https://img.shields.io/github/forks/Chocapikk/Windfall.svg)


## CVE-2026-22666
 Dolibarr ERP/CRM versions prior to 23.0.2 contain an authenticated remote code execution vulnerability in the dol_eval_standard() function that fails to apply forbidden string checks in whitelist mode and does not detect PHP dynamic callable syntax. Attackers with administrator privileges can inject malicious payloads through computed extrafields or other evaluation paths using PHP dynamic callable syntax to bypass validation and achieve arbitrary command execution via eval().

- [https://github.com/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666](https://github.com/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666) :  ![starts](https://img.shields.io/github/stars/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666.svg) ![forks](https://img.shields.io/github/forks/JivaSecurity/DOLIBARR-RCE-CVE-2026-22666.svg)


## CVE-2026-20841
 Improper neutralization of special elements used in a command ('command injection') in Windows Notepad App allows an unauthorized attacker to execute code locally.

- [https://github.com/whiskeylab/notepad_CVE_2026_20841](https://github.com/whiskeylab/notepad_CVE_2026_20841) :  ![starts](https://img.shields.io/github/stars/whiskeylab/notepad_CVE_2026_20841.svg) ![forks](https://img.shields.io/github/forks/whiskeylab/notepad_CVE_2026_20841.svg)


## CVE-2026-20131
Note: If the FMC management interface does not have public internet access, the attack surface that is associated with this vulnerability is reduced.

- [https://github.com/Hassan-Pouladi/Cisco-FMC-honeypot](https://github.com/Hassan-Pouladi/Cisco-FMC-honeypot) :  ![starts](https://img.shields.io/github/stars/Hassan-Pouladi/Cisco-FMC-honeypot.svg) ![forks](https://img.shields.io/github/forks/Hassan-Pouladi/Cisco-FMC-honeypot.svg)


## CVE-2026-5733
 Incorrect boundary conditions in the Graphics: WebGPU component. This vulnerability affects Firefox  149.0.2 and Thunderbird  149.0.2.

- [https://github.com/Lechansky/CVE-2026-5733](https://github.com/Lechansky/CVE-2026-5733) :  ![starts](https://img.shields.io/github/stars/Lechansky/CVE-2026-5733.svg) ![forks](https://img.shields.io/github/forks/Lechansky/CVE-2026-5733.svg)


## CVE-2026-5465
 The Booking for Appointments and Events Calendar – Amelia plugin for WordPress is vulnerable to Insecure Direct Object Reference in all versions up to, and including, 2.1.3. This is due to the `UpdateProviderCommandHandler` failing to validate changes to the `externalId` field when a Provider (Employee) user updates their own profile. The `externalId` maps directly to a WordPress user ID and is passed to `wp_set_password()` and `wp_update_user()` without authorization checks. This makes it possible for authenticated attackers, with Provider-level (Employee) access and above, to take over any WordPress account — including Administrator — by injecting an arbitrary `externalId` value when updating their own provider profile.

- [https://github.com/kaleth4/CVE-2026-5465](https://github.com/kaleth4/CVE-2026-5465) :  ![starts](https://img.shields.io/github/stars/kaleth4/CVE-2026-5465.svg) ![forks](https://img.shields.io/github/forks/kaleth4/CVE-2026-5465.svg)


## CVE-2026-5281
 Use after free in Dawn in Google Chrome prior to 146.0.7680.178 allowed a remote attacker who had compromised the renderer process to execute arbitrary code via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/TheMalwareGuardian/CVE-2026-5281](https://github.com/TheMalwareGuardian/CVE-2026-5281) :  ![starts](https://img.shields.io/github/stars/TheMalwareGuardian/CVE-2026-5281.svg) ![forks](https://img.shields.io/github/forks/TheMalwareGuardian/CVE-2026-5281.svg)


## CVE-2026-4800
Do not pass untrusted input as key names in options.imports. Only use developer-controlled, static key names.

- [https://github.com/SvenLie/next-rep-CVE-2026-4800](https://github.com/SvenLie/next-rep-CVE-2026-4800) :  ![starts](https://img.shields.io/github/stars/SvenLie/next-rep-CVE-2026-4800.svg) ![forks](https://img.shields.io/github/forks/SvenLie/next-rep-CVE-2026-4800.svg)


## CVE-2026-4406
 The Gravity Forms plugin for WordPress is vulnerable to Reflected Cross-Site Scripting via the `form_ids` parameter in the `gform_get_config` AJAX action in all versions up to, and including, 2.9.30. This is due to the `GFCommon::send_json()` method outputting JSON-encoded data wrapped in HTML comment delimiters using `echo` and `wp_die()`, which serves the response with a `Content-Type: text/html` header instead of `application/json`. The `wp_json_encode()` function does not HTML-encode angle brackets within JSON string values, allowing injected HTML/script tags in `form_ids` array values to be parsed and executed by the browser. The required `config_nonce` is generated with `wp_create_nonce('gform_config_ajax')` and is publicly embedded on every page that renders a Gravity Forms form, making it identical for all unauthenticated visitors within the same 12-hour nonce tick. This makes it possible for unauthenticated attackers to inject arbitrary web scripts in pages that execute if they can successfully trick a user into performing an action such as clicking on a link. This vulnerability cannot be exploited against users who are authenticated on the target system, but could be used to alter the target page.

- [https://github.com/Hann1bl3L3ct3r/CVE-2026-4406](https://github.com/Hann1bl3L3ct3r/CVE-2026-4406) :  ![starts](https://img.shields.io/github/stars/Hann1bl3L3ct3r/CVE-2026-4406.svg) ![forks](https://img.shields.io/github/forks/Hann1bl3L3ct3r/CVE-2026-4406.svg)


## CVE-2026-2962
 A vulnerability was found in D-Link DWR-M960 1.01.07. This vulnerability affects the function sub_460F30 of the file /boafrm/formDateReboot of the component Scheduled Reboot Configuration Endpoint. The manipulation of the argument submit-url results in stack-based buffer overflow. The attack may be performed from remote. The exploit has been made public and could be used.

- [https://github.com/kiyochii/CVE-2026-29628](https://github.com/kiyochii/CVE-2026-29628) :  ![starts](https://img.shields.io/github/stars/kiyochii/CVE-2026-29628.svg) ![forks](https://img.shields.io/github/forks/kiyochii/CVE-2026-29628.svg)


## CVE-2026-2699
 Customer Managed ShareFile Storage Zones Controller (SZC) allows an unauthenticated attacker to access restricted configuration pages. This leads to changing system configuration and potential remote code execution.

- [https://github.com/0xBlackash/CVE-2026-2699](https://github.com/0xBlackash/CVE-2026-2699) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2026-2699.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2026-2699.svg)


## CVE-2025-69515
 An issue in JXL 9 Inch Car Android Double Din Player Android v12.0 allows attackers to force the infotainment system into accepting falsified GPS signals as legitimate, resulting in the device reporting an incorrect or static location.

- [https://github.com/thorat-shubham/JXL_Infotainment_CVE-2025-69515](https://github.com/thorat-shubham/JXL_Infotainment_CVE-2025-69515) :  ![starts](https://img.shields.io/github/stars/thorat-shubham/JXL_Infotainment_CVE-2025-69515.svg) ![forks](https://img.shields.io/github/forks/thorat-shubham/JXL_Infotainment_CVE-2025-69515.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)


## CVE-2025-66034
 fontTools is a library for manipulating fonts, written in Python. In versions from 4.33.0 to before 4.60.2, the fonttools varLib (or python3 -m fontTools.varLib) script has an arbitrary file write vulnerability that leads to remote code execution when a malicious .designspace file is processed. The vulnerability affects the main() code path of fontTools.varLib, used by the fonttools varLib CLI and any code that invokes fontTools.varLib.main(). This issue has been patched in version 4.60.2.

- [https://github.com/jwsly12/CVE-2025-66034-htb-ctf](https://github.com/jwsly12/CVE-2025-66034-htb-ctf) :  ![starts](https://img.shields.io/github/stars/jwsly12/CVE-2025-66034-htb-ctf.svg) ![forks](https://img.shields.io/github/forks/jwsly12/CVE-2025-66034-htb-ctf.svg)


## CVE-2025-56015
 In GenieACS 1.2.13, an unauthenticated access vulnerability exists in the NBI API endpoint.

- [https://github.com/e1st/CVE-2025-56015](https://github.com/e1st/CVE-2025-56015) :  ![starts](https://img.shields.io/github/stars/e1st/CVE-2025-56015.svg) ![forks](https://img.shields.io/github/forks/e1st/CVE-2025-56015.svg)


## CVE-2025-55182
 A pre-authentication remote code execution vulnerability exists in React Server Components versions 19.0.0, 19.1.0, 19.1.1, and 19.2.0 including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints.

- [https://github.com/hexsh1dow/CVE-2025-55182](https://github.com/hexsh1dow/CVE-2025-55182) :  ![starts](https://img.shields.io/github/stars/hexsh1dow/CVE-2025-55182.svg) ![forks](https://img.shields.io/github/forks/hexsh1dow/CVE-2025-55182.svg)


## CVE-2025-48384
 Git is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals. When reading a config value, Git strips any trailing carriage return and line feed (CRLF). When writing a config entry, values with a trailing CR are not quoted, causing the CR to be lost when the config is later read. When initializing a submodule, if the submodule path contains a trailing CR, the altered path is read resulting in the submodule being checked out to an incorrect location. If a symlink exists that points the altered path to the submodule hooks directory, and the submodule contains an executable post-checkout hook, the script may be unintentionally executed after checkout. This vulnerability is fixed in v2.43.7, v2.44.4, v2.45.4, v2.46.4, v2.47.3, v2.48.2, v2.49.1, and v2.50.1.

- [https://github.com/sathish46-lab/CVE-2025-48384-submodule](https://github.com/sathish46-lab/CVE-2025-48384-submodule) :  ![starts](https://img.shields.io/github/stars/sathish46-lab/CVE-2025-48384-submodule.svg) ![forks](https://img.shields.io/github/forks/sathish46-lab/CVE-2025-48384-submodule.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-15467
OpenSSL 1.1.1 and 1.0.2 are not affected by this issue.

- [https://github.com/WostGit/cve-2025-15467-crash](https://github.com/WostGit/cve-2025-15467-crash) :  ![starts](https://img.shields.io/github/stars/WostGit/cve-2025-15467-crash.svg) ![forks](https://img.shields.io/github/forks/WostGit/cve-2025-15467-crash.svg)


## CVE-2025-14857
 An improper access control vulnerability exists in Semtech LoRa LR11xxx transceivers running early versions of firmware where the memory write command accessible via the physical SPI interface fails to enforce write protection on the program call stack. An attacker with physical access to the SPI interface can overwrite stack memory to hijack program control flow and achieve limited arbitrary code execution. However, the impact is limited to the active attack session: the device's secure boot mechanism prevents persistent firmware modification, the crypto engine isolates cryptographic keys from direct firmware access, and all modifications are lost upon device reboot or loss of physical access.

- [https://github.com/Ermensonx/CVE-2025-14857-MongoBleed](https://github.com/Ermensonx/CVE-2025-14857-MongoBleed) :  ![starts](https://img.shields.io/github/stars/Ermensonx/CVE-2025-14857-MongoBleed.svg) ![forks](https://img.shields.io/github/forks/Ermensonx/CVE-2025-14857-MongoBleed.svg)


## CVE-2025-13315
 Twonky Server 8.5.2 on Linux and Windows is vulnerable to an access control flaw. An unauthenticated attacker can bypass web service API authentication controls to leak a log file and read the administrator's username and encrypted password.

- [https://github.com/0xBlackash/CVE-2025-13315](https://github.com/0xBlackash/CVE-2025-13315) :  ![starts](https://img.shields.io/github/stars/0xBlackash/CVE-2025-13315.svg) ![forks](https://img.shields.io/github/forks/0xBlackash/CVE-2025-13315.svg)


## CVE-2025-9074
This can lead to execution of a wide range of privileged commands to the engine API, including controlling other containers, creating new ones, managing images etc. In some circumstances (e.g. Docker Desktop for Windows with WSL backend) it also allows mounting the host drive with the same privileges as the user running Docker Desktop.

- [https://github.com/chernandez321/CVE-2025-9074-docker-escape](https://github.com/chernandez321/CVE-2025-9074-docker-escape) :  ![starts](https://img.shields.io/github/stars/chernandez321/CVE-2025-9074-docker-escape.svg) ![forks](https://img.shields.io/github/forks/chernandez321/CVE-2025-9074-docker-escape.svg)


## CVE-2025-8088
     from ESET.

- [https://github.com/starfallreverie/winrar-exploit](https://github.com/starfallreverie/winrar-exploit) :  ![starts](https://img.shields.io/github/stars/starfallreverie/winrar-exploit.svg) ![forks](https://img.shields.io/github/forks/starfallreverie/winrar-exploit.svg)
- [https://github.com/shaheeryasirofficial/CVE-2025-8088](https://github.com/shaheeryasirofficial/CVE-2025-8088) :  ![starts](https://img.shields.io/github/stars/shaheeryasirofficial/CVE-2025-8088.svg) ![forks](https://img.shields.io/github/forks/shaheeryasirofficial/CVE-2025-8088.svg)


## CVE-2024-56426
 An issue was discovered in Samsung Mobile Processor and Wearable Processor Exynos 980, 990, 850, 1080, 2100, 1280, 2200, 1330, 1380, 1480, 2400, W920, W930, W1000. The lack of a length check leads to out-of-bounds writes via malformed USB packets to the target.

- [https://github.com/Creeeeger/CVE-2024-56426](https://github.com/Creeeeger/CVE-2024-56426) :  ![starts](https://img.shields.io/github/stars/Creeeeger/CVE-2024-56426.svg) ![forks](https://img.shields.io/github/forks/Creeeeger/CVE-2024-56426.svg)


## CVE-2024-40110
 Sourcecodester Poultry Farm Management System v1.0 contains an Unauthenticated Remote Code Execution (RCE) vulnerability via the productimage parameter at /farm/product.php.

- [https://github.com/thiagosmith/CVE-2024-40110](https://github.com/thiagosmith/CVE-2024-40110) :  ![starts](https://img.shields.io/github/stars/thiagosmith/CVE-2024-40110.svg) ![forks](https://img.shields.io/github/forks/thiagosmith/CVE-2024-40110.svg)


## CVE-2024-21413
 Microsoft Outlook Remote Code Execution Vulnerability

- [https://github.com/KartheekKandalam99/SVPT_CW_2](https://github.com/KartheekKandalam99/SVPT_CW_2) :  ![starts](https://img.shields.io/github/stars/KartheekKandalam99/SVPT_CW_2.svg) ![forks](https://img.shields.io/github/forks/KartheekKandalam99/SVPT_CW_2.svg)


## CVE-2023-42115
. Was ZDI-CAN-17434.

- [https://github.com/doaso/CVE-2023-42115](https://github.com/doaso/CVE-2023-42115) :  ![starts](https://img.shields.io/github/stars/doaso/CVE-2023-42115.svg) ![forks](https://img.shields.io/github/forks/doaso/CVE-2023-42115.svg)


## CVE-2023-39115
 install/aiz-uploader/upload in Campcodes Online Matrimonial Website System Script 3.3 allows XSS via a crafted SVG document.

- [https://github.com/0xrajdip/CVE-2023-39115](https://github.com/0xrajdip/CVE-2023-39115) :  ![starts](https://img.shields.io/github/stars/0xrajdip/CVE-2023-39115.svg) ![forks](https://img.shields.io/github/forks/0xrajdip/CVE-2023-39115.svg)


## CVE-2022-46364
 A SSRF vulnerability in parsing the href attribute of XOP:Include in MTOM requests in versions of Apache CXF before 3.5.5 and 3.4.10 allows an attacker to perform SSRF style attacks on webservices that take at least one parameter of any type. 

- [https://github.com/cybermaksxx/CVE-2022-46364-Proof-of-the-concept](https://github.com/cybermaksxx/CVE-2022-46364-Proof-of-the-concept) :  ![starts](https://img.shields.io/github/stars/cybermaksxx/CVE-2022-46364-Proof-of-the-concept.svg) ![forks](https://img.shields.io/github/forks/cybermaksxx/CVE-2022-46364-Proof-of-the-concept.svg)


## CVE-2021-4034
 A local privilege escalation vulnerability was found on polkit's pkexec utility. The pkexec application is a setuid tool designed to allow unprivileged users to run commands as privileged users according predefined policies. The current version of pkexec doesn't handle the calling parameters count correctly and ends trying to execute environment variables as commands. An attacker can leverage this by crafting environment variables in such a way it'll induce pkexec to execute arbitrary code. When successfully executed the attack can cause a local privilege escalation given unprivileged users administrative rights on the target machine.

- [https://github.com/hackingyseguridad/root](https://github.com/hackingyseguridad/root) :  ![starts](https://img.shields.io/github/stars/hackingyseguridad/root.svg) ![forks](https://img.shields.io/github/forks/hackingyseguridad/root.svg)


## CVE-2020-1938
 When using the Apache JServ Protocol (AJP), care must be taken when trusting incoming connections to Apache Tomcat. Tomcat treats AJP connections as having higher trust than, for example, a similar HTTP connection. If such connections are available to an attacker, they can be exploited in ways that may be surprising. In Apache Tomcat 9.0.0.M1 to 9.0.0.30, 8.5.0 to 8.5.50 and 7.0.0 to 7.0.99, Tomcat shipped with an AJP Connector enabled by default that listened on all configured IP addresses. It was expected (and recommended in the security guide) that this Connector would be disabled if not required. This vulnerability report identified a mechanism that allowed: - returning arbitrary files from anywhere in the web application - processing any file in the web application as a JSP Further, if the web application allowed file upload and stored those files within the web application (or the attacker was able to control the content of the web application by some other means) then this, along with the ability to process a file as a JSP, made remote code execution possible. It is important to note that mitigation is only required if an AJP port is accessible to untrusted users. Users wishing to take a defence-in-depth approach and block the vector that permits returning arbitrary files and execution as JSP may upgrade to Apache Tomcat 9.0.31, 8.5.51 or 7.0.100 or later. A number of changes were made to the default AJP Connector configuration in 9.0.31 to harden the default configuration. It is likely that users upgrading to 9.0.31, 8.5.51 or 7.0.100 or later will need to make small changes to their configurations.

- [https://github.com/With-fate/CVE-2020-1938](https://github.com/With-fate/CVE-2020-1938) :  ![starts](https://img.shields.io/github/stars/With-fate/CVE-2020-1938.svg) ![forks](https://img.shields.io/github/forks/With-fate/CVE-2020-1938.svg)
- [https://github.com/sangrok-jeon/CVE-2020-1938-Tomcat-AJP-Ghostcat--Analysis](https://github.com/sangrok-jeon/CVE-2020-1938-Tomcat-AJP-Ghostcat--Analysis) :  ![starts](https://img.shields.io/github/stars/sangrok-jeon/CVE-2020-1938-Tomcat-AJP-Ghostcat--Analysis.svg) ![forks](https://img.shields.io/github/forks/sangrok-jeon/CVE-2020-1938-Tomcat-AJP-Ghostcat--Analysis.svg)


## CVE-2018-9276
 An issue was discovered in PRTG Network Monitor before 18.2.39. An attacker who has access to the PRTG System Administrator web console with administrative privileges can exploit an OS command injection vulnerability (both on the server and on devices) by sending malformed parameters in sensor or notification management scenarios.

- [https://github.com/AC8999/PRTG-Network-Monitor-18.2.38---Authenticated-Remote-Code-Execution-CVE-2018-9276](https://github.com/AC8999/PRTG-Network-Monitor-18.2.38---Authenticated-Remote-Code-Execution-CVE-2018-9276) :  ![starts](https://img.shields.io/github/stars/AC8999/PRTG-Network-Monitor-18.2.38---Authenticated-Remote-Code-Execution-CVE-2018-9276.svg) ![forks](https://img.shields.io/github/forks/AC8999/PRTG-Network-Monitor-18.2.38---Authenticated-Remote-Code-Execution-CVE-2018-9276.svg)


## CVE-2017-5638
 The Jakarta Multipart parser in Apache Struts 2 2.3.x before 2.3.32 and 2.5.x before 2.5.10.1 has incorrect exception handling and error-message generation during file-upload attempts, which allows remote attackers to execute arbitrary commands via a crafted Content-Type, Content-Disposition, or Content-Length HTTP header, as exploited in the wild in March 2017 with a Content-Type header containing a #cmd= string.

- [https://github.com/AIPEACS/SC3010-Computer-Security](https://github.com/AIPEACS/SC3010-Computer-Security) :  ![starts](https://img.shields.io/github/stars/AIPEACS/SC3010-Computer-Security.svg) ![forks](https://img.shields.io/github/forks/AIPEACS/SC3010-Computer-Security.svg)

