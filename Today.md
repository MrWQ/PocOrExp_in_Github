# Update 2026-05-01
## CVE-2026-42167
 mod_sql in ProFTPD before 1.3.10rc1 allows remote attackers to execute arbitrary code via a username, in scenarios where there is logging of USER requests with an expansion such as %U, and the SQL backend allows commands (e.g., COPY TO PROGRAM).

- [https://github.com/dinosn/proftpd-CVE-2026-42167-analysis](https://github.com/dinosn/proftpd-CVE-2026-42167-analysis) :  ![starts](https://img.shields.io/github/stars/dinosn/proftpd-CVE-2026-42167-analysis.svg) ![forks](https://img.shields.io/github/forks/dinosn/proftpd-CVE-2026-42167-analysis.svg)


## CVE-2026-41940
 cPanel and WHM versions prior to 11.110.0.97, 11.118.0.63, 11.126.0.54, 11.132.0.29, 11.134.0.20, and 11.136.0.5 contain an authentication bypass vulnerability in the login flow that allows unauthenticated remote attackers to gain unauthorized access to the control panel.

- [https://github.com/Sachinart/CVE-2026-41940-cpanel-0day](https://github.com/Sachinart/CVE-2026-41940-cpanel-0day) :  ![starts](https://img.shields.io/github/stars/Sachinart/CVE-2026-41940-cpanel-0day.svg) ![forks](https://img.shields.io/github/forks/Sachinart/CVE-2026-41940-cpanel-0day.svg)
- [https://github.com/debugactiveprocess/cPanel-WHM-AuthBypass-Session-Checker](https://github.com/debugactiveprocess/cPanel-WHM-AuthBypass-Session-Checker) :  ![starts](https://img.shields.io/github/stars/debugactiveprocess/cPanel-WHM-AuthBypass-Session-Checker.svg) ![forks](https://img.shields.io/github/forks/debugactiveprocess/cPanel-WHM-AuthBypass-Session-Checker.svg)


## CVE-2026-41651
3. Late flag read at execution time (lines 2273–2277): The scheduler's idle callback reads cached_transaction_flags at dispatch time, not at authorization time. If flags were overwritten between authorization and execution, the backend sees the attacker's flags.

- [https://github.com/shibaaa204/Pack2TheRoot](https://github.com/shibaaa204/Pack2TheRoot) :  ![starts](https://img.shields.io/github/stars/shibaaa204/Pack2TheRoot.svg) ![forks](https://img.shields.io/github/forks/shibaaa204/Pack2TheRoot.svg)


## CVE-2026-40478
 Thymeleaf is a server-side Java template engine for web and standalone environments. Versions 3.1.3.RELEASE and prior contain a security bypass vulnerability in the the expression execution mechanisms. Although the library provides mechanisms to prevent expression injection, it fails to properly neutralize specific syntax patterns that allow for the execution of unauthorized expressions. If an application developer passes unvalidated user input directly to the template engine, an unauthenticated remote attacker can bypass the library's protections to achieve Server-Side Template Injection (SSTI). This issue has ben fixed in version 3.1.4.RELEASE.

- [https://github.com/bmvermeer/thymeleaf.CVE_2026_40478](https://github.com/bmvermeer/thymeleaf.CVE_2026_40478) :  ![starts](https://img.shields.io/github/stars/bmvermeer/thymeleaf.CVE_2026_40478.svg) ![forks](https://img.shields.io/github/forks/bmvermeer/thymeleaf.CVE_2026_40478.svg)


## CVE-2026-35414
 OpenSSH before 10.3 mishandles the authorized_keys principals option in uncommon scenarios involving a principals list in conjunction with a Certificate Authority that makes certain use of comma characters.

- [https://github.com/killercd/CVE-2026-35414](https://github.com/killercd/CVE-2026-35414) :  ![starts](https://img.shields.io/github/stars/killercd/CVE-2026-35414.svg) ![forks](https://img.shields.io/github/forks/killercd/CVE-2026-35414.svg)


## CVE-2026-34975
 Plunk is an open-source email platform built on top of AWS SES. Prior to 0.8.0, a CRLF header injection vulnerability was discovered in SESService.ts, where user-supplied values for from.name, subject, custom header keys/values, and attachment filenames were interpolated directly into raw MIME messages without sanitization. An authenticated API user could inject arbitrary email headers (e.g. Bcc, Reply-To) by embedding carriage return/line feed characters in these fields, enabling silent email forwarding, reply redirection, or sender spoofing. The fix adds input validation at the schema level to reject any of these fields containing \r or \n characters, consistent with the existing validation already applied to the contentId field. This vulnerability is fixed in 0.8.0.

- [https://github.com/romain-deperne/CVE-2026-34975](https://github.com/romain-deperne/CVE-2026-34975) :  ![starts](https://img.shields.io/github/stars/romain-deperne/CVE-2026-34975.svg) ![forks](https://img.shields.io/github/forks/romain-deperne/CVE-2026-34975.svg)


## CVE-2026-34940
 KubeAI is an AI inference operator for kubernetes. Prior to 0.23.2, the ollamaStartupProbeScript() function in internal/modelcontroller/engine_ollama.go constructs a shell command string using fmt.Sprintf with unsanitized model URL components (ref, modelParam). This shell command is executed via bash -c as a Kubernetes startup probe. An attacker who can create or update Model custom resources can inject arbitrary shell commands that execute inside model server pods. This vulnerability is fixed in 0.23.2.

- [https://github.com/romain-deperne/CVE-2026-34940](https://github.com/romain-deperne/CVE-2026-34940) :  ![starts](https://img.shields.io/github/stars/romain-deperne/CVE-2026-34940.svg) ![forks](https://img.shields.io/github/forks/romain-deperne/CVE-2026-34940.svg)


## CVE-2026-34160
 Chamilo LMS is an open-source learning management system. In versions prior to 2.0.0-RC.3, the PENS (Package Exchange Notification Services) plugin endpoint at public/plugin/Pens/pens.php is accessible without authentication and accepts a user-controlled package-url parameter that the server fetches using curl without filtering private or internal IP addresses, enabling unauthenticated Server-Side Request Forgery (SSRF). An attacker can exploit this to probe internal network services, access cloud metadata endpoints (such as 169.254.169.254) to steal IAM credentials and sensitive instance metadata, or trigger state-changing operations on internal services via the receipt and alerts callback parameters. No authentication is required to exploit either SSRF vector, significantly increasing the attack surface. This issue has been fixed in version 2.0.0-RC.3.

- [https://github.com/romain-deperne/CVE-2026-34160](https://github.com/romain-deperne/CVE-2026-34160) :  ![starts](https://img.shields.io/github/stars/romain-deperne/CVE-2026-34160.svg) ![forks](https://img.shields.io/github/forks/romain-deperne/CVE-2026-34160.svg)


## CVE-2026-33980
 Azure Data Explorer MCP Server is a Model Context Protocol (MCP) server that enables AI assistants to execute KQL queries and explore Azure Data Explorer (ADX/Kusto) databases through standardized interfaces. Versions up to and including 0.1.1 contain KQL (Kusto Query Language) injection vulnerabilities in three MCP tool handlers: `get_table_schema`, `sample_table_data`, and `get_table_details`. The `table_name` parameter is interpolated directly into KQL queries via f-strings without any validation or sanitization, allowing an attacker (or a prompt-injected AI agent) to execute arbitrary KQL queries against the Azure Data Explorer cluster. Commit 0abe0ee55279e111281076393e5e966335fffd30 patches the issue.

- [https://github.com/romain-deperne/CVE-2026-33980](https://github.com/romain-deperne/CVE-2026-33980) :  ![starts](https://img.shields.io/github/stars/romain-deperne/CVE-2026-33980.svg) ![forks](https://img.shields.io/github/forks/romain-deperne/CVE-2026-33980.svg)


## CVE-2026-33715
 Chamilo LMS is an open-source learning management system. In version 2.0-RC.2, the file public/main/inc/ajax/install.ajax.php is accessible without authentication on fully installed instances because, unlike other AJAX endpoints, it does not include the global.inc.php file that performs authentication and installation-completed checks. Its test_mailer action accepts an arbitrary Symfony Mailer DSN string from POST data and uses it to connect to an attacker-specified SMTP server, enabling Server-Side Request Forgery (SSRF) into internal networks via the SMTP protocol. An unauthenticated attacker can also abuse this to weaponize the Chamilo server as an open email relay for phishing and spam campaigns, with emails appearing to originate from the server's IP address. Additionally, error responses from failed SMTP connections may disclose information about internal network topology and running services. This issue has been fixed in version 2.0.0-RC.3.

- [https://github.com/romain-deperne/CVE-2026-33715](https://github.com/romain-deperne/CVE-2026-33715) :  ![starts](https://img.shields.io/github/stars/romain-deperne/CVE-2026-33715.svg) ![forks](https://img.shields.io/github/forks/romain-deperne/CVE-2026-33715.svg)


## CVE-2026-32247
 Graphiti is a framework for building and querying temporal context graphs for AI agents. Graphiti versions before 0.28.2 contained a Cypher injection vulnerability in shared search-filter construction for non-Kuzu backends. Attacker-controlled label values supplied through SearchFilters.node_labels were concatenated directly into Cypher label expressions without validation. In MCP deployments, this was exploitable not only through direct untrusted access to the Graphiti MCP server, but also through prompt injection against an LLM client that could be induced to call search_nodes with attacker-controlled entity_types values. The MCP server mapped entity_types to SearchFilters.node_labels, which then reached the vulnerable Cypher construction path. Affected backends included Neo4j, FalkorDB, and Neptune. Kuzu was not affected by the label-injection issue because it used parameterized label handling rather than string-interpolated Cypher labels. This issue was mitigated in 0.28.2.

- [https://github.com/romain-deperne/CVE-2026-32247](https://github.com/romain-deperne/CVE-2026-32247) :  ![starts](https://img.shields.io/github/stars/romain-deperne/CVE-2026-32247.svg) ![forks](https://img.shields.io/github/forks/romain-deperne/CVE-2026-32247.svg)


## CVE-2026-31431
AD directly.

- [https://github.com/theori-io/copy-fail-CVE-2026-31431](https://github.com/theori-io/copy-fail-CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/theori-io/copy-fail-CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/theori-io/copy-fail-CVE-2026-31431.svg)
- [https://github.com/rootsecdev/cve_2026_31431](https://github.com/rootsecdev/cve_2026_31431) :  ![starts](https://img.shields.io/github/stars/rootsecdev/cve_2026_31431.svg) ![forks](https://img.shields.io/github/forks/rootsecdev/cve_2026_31431.svg)
- [https://github.com/badsectorlabs/copyfail-go](https://github.com/badsectorlabs/copyfail-go) :  ![starts](https://img.shields.io/github/stars/badsectorlabs/copyfail-go.svg) ![forks](https://img.shields.io/github/forks/badsectorlabs/copyfail-go.svg)
- [https://github.com/Theori-lO/copy-fail-CVE-2026-31431](https://github.com/Theori-lO/copy-fail-CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/Theori-lO/copy-fail-CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/Theori-lO/copy-fail-CVE-2026-31431.svg)
- [https://github.com/Alfredooe/CVE-2026-31431](https://github.com/Alfredooe/CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/Alfredooe/CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/Alfredooe/CVE-2026-31431.svg)
- [https://github.com/tgies/copy-fail-c](https://github.com/tgies/copy-fail-c) :  ![starts](https://img.shields.io/github/stars/tgies/copy-fail-c.svg) ![forks](https://img.shields.io/github/forks/tgies/copy-fail-c.svg)
- [https://github.com/mhdgning131/CVE-2026-31431_poc](https://github.com/mhdgning131/CVE-2026-31431_poc) :  ![starts](https://img.shields.io/github/stars/mhdgning131/CVE-2026-31431_poc.svg) ![forks](https://img.shields.io/github/forks/mhdgning131/CVE-2026-31431_poc.svg)
- [https://github.com/ZephrFish/CopyFail-CVE-2026-31431](https://github.com/ZephrFish/CopyFail-CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/ZephrFish/CopyFail-CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/ZephrFish/CopyFail-CVE-2026-31431.svg)
- [https://github.com/Crihexe/copy-fail-tiny-elf-CVE-2026-31431](https://github.com/Crihexe/copy-fail-tiny-elf-CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/Crihexe/copy-fail-tiny-elf-CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/Crihexe/copy-fail-tiny-elf-CVE-2026-31431.svg)
- [https://github.com/painoob/Copy-Fail-Exploit-CVE-2026-31431](https://github.com/painoob/Copy-Fail-Exploit-CVE-2026-31431) :  ![starts](https://img.shields.io/github/stars/painoob/Copy-Fail-Exploit-CVE-2026-31431.svg) ![forks](https://img.shields.io/github/forks/painoob/Copy-Fail-Exploit-CVE-2026-31431.svg)


## CVE-2026-30824
 Flowise is a drag & drop user interface to build a customized large language model flow. Prior to version 3.0.13, the NVIDIA NIM router (/api/v1/nvidia-nim/*) is whitelisted in the global authentication middleware, allowing unauthenticated access to privileged container management and token generation endpoints. This issue has been patched in version 3.0.13.

- [https://github.com/dylvie/CVE-2026-30824-Flowise-NVIDIA-NIM-Authentication](https://github.com/dylvie/CVE-2026-30824-Flowise-NVIDIA-NIM-Authentication) :  ![starts](https://img.shields.io/github/stars/dylvie/CVE-2026-30824-Flowise-NVIDIA-NIM-Authentication.svg) ![forks](https://img.shields.io/github/forks/dylvie/CVE-2026-30824-Flowise-NVIDIA-NIM-Authentication.svg)


## CVE-2026-27825
 MCP Atlassian is a Model Context Protocol (MCP) server for Atlassian products (Confluence and Jira). Prior to version 0.17.0, the `confluence_download_attachment` MCP tool accepts a `download_path` parameter that is written to without any directory boundary enforcement. An attacker who can call this tool and supply or access a Confluence attachment with malicious content can write arbitrary content to any path the server process has write access to. Because the attacker controls both the write destination and the written content (via an uploaded Confluence attachment), this constitutes for arbitrary code execution (for example, writing a valid cron entry to `/etc/cron.d/` achieves code execution within one scheduler cycle with no server restart required). Version 0.17.0 fixes the issue.

- [https://github.com/romain-deperne/CVE-2026-27825](https://github.com/romain-deperne/CVE-2026-27825) :  ![starts](https://img.shields.io/github/stars/romain-deperne/CVE-2026-27825.svg) ![forks](https://img.shields.io/github/forks/romain-deperne/CVE-2026-27825.svg)


## CVE-2026-7401
 A vulnerability was detected in SourceCodester CET Automated Grading System with AI Predictive Analytics 1.0. This vulnerability affects unknown code of the file /index.php?action=register of the component Registration. The manipulation of the argument student_id/full_name/section/username results in cross site scripting. The attack can be launched remotely. The exploit is now public and may be used.

- [https://github.com/Xmyronn/CVE-2026-7401-XSS](https://github.com/Xmyronn/CVE-2026-7401-XSS) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-7401-XSS.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-7401-XSS.svg)


## CVE-2026-7394
 A vulnerability was determined in SourceCodester Pizzafy Ecommerce System 1.0. Affected by this vulnerability is an unknown functionality of the file /admin/view_order.php of the component GET Parameter Handler. Executing a manipulation of the argument ID can lead to sql injection. The attack may be performed from remote. The exploit has been publicly disclosed and may be utilized.

- [https://github.com/Xmyronn/CVE-2026-7394-SQLI](https://github.com/Xmyronn/CVE-2026-7394-SQLI) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-7394-SQLI.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-7394-SQLI.svg)


## CVE-2026-7393
 A vulnerability was found in SourceCodester Pizzafy Ecommerce System 1.0. Affected is the function save_menu of the file /admin/admin_class_novo.php of the component File Extension Handler. Performing a manipulation of the argument img results in unrestricted upload. The attack is possible to be carried out remotely. The exploit has been made public and could be used.

- [https://github.com/Xmyronn/CVE-2026-7393-RCE](https://github.com/Xmyronn/CVE-2026-7393-RCE) :  ![starts](https://img.shields.io/github/stars/Xmyronn/CVE-2026-7393-RCE.svg) ![forks](https://img.shields.io/github/forks/Xmyronn/CVE-2026-7393-RCE.svg)


## CVE-2026-6849
This issue affects Pardus OS My Computer: from =0.7.5 before 0.8.0.

- [https://github.com/osmancanvural/CVE-2026-6849](https://github.com/osmancanvural/CVE-2026-6849) :  ![starts](https://img.shields.io/github/stars/osmancanvural/CVE-2026-6849.svg) ![forks](https://img.shields.io/github/forks/osmancanvural/CVE-2026-6849.svg)


## CVE-2026-6644
Affected products and versions include: from ADM 4.1.0 through ADM 4.3.3.RR42 as well as from ADM 5.0.0 through ADM 5.1.2.REO1.

- [https://github.com/uky007/CVE-2026-6644](https://github.com/uky007/CVE-2026-6644) :  ![starts](https://img.shields.io/github/stars/uky007/CVE-2026-6644.svg) ![forks](https://img.shields.io/github/forks/uky007/CVE-2026-6644.svg)


## CVE-2026-3910
 Inappropriate implementation in V8 in Google Chrome prior to 146.0.7680.75 allowed a remote attacker to execute arbitrary code inside a sandbox via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/5o1z/CVE-2026-3910](https://github.com/5o1z/CVE-2026-3910) :  ![starts](https://img.shields.io/github/stars/5o1z/CVE-2026-3910.svg) ![forks](https://img.shields.io/github/forks/5o1z/CVE-2026-3910.svg)


## CVE-2026-3854
 An improper neutralization of special elements vulnerability was identified in GitHub Enterprise Server that allowed an attacker with push access to a repository to achieve remote code execution on the instance. During a git push operation, user-supplied push option values were not properly sanitized before being included in internal service headers. Because the internal header format used a delimiter character that could also appear in user input, an attacker could inject additional metadata fields through crafted push option values. This vulnerability was reported via the GitHub Bug Bounty program and has been fixed in GitHub Enterprise Server versions 3.14.25, 3.15.20, 3.16.16, 3.17.13, 3.18.7 and 3.19.4.

- [https://github.com/lysophavin18/CVE-2026-3854-PoC](https://github.com/lysophavin18/CVE-2026-3854-PoC) :  ![starts](https://img.shields.io/github/stars/lysophavin18/CVE-2026-3854-PoC.svg) ![forks](https://img.shields.io/github/forks/lysophavin18/CVE-2026-3854-PoC.svg)
- [https://github.com/simondankelmann/cve-2026-3854-test](https://github.com/simondankelmann/cve-2026-3854-test) :  ![starts](https://img.shields.io/github/stars/simondankelmann/cve-2026-3854-test.svg) ![forks](https://img.shields.io/github/forks/simondankelmann/cve-2026-3854-test.svg)


## CVE-2026-3696
 A vulnerability was found in Totolink N300RH 6..1c.1353_B20190305. The affected element is the function setWiFiWpsConfig of the file /cgi-bin/cstecgi.cgi of the component CGI Handler. Performing a manipulation results in os command injection. The attack can be initiated remotely. The exploit has been made public and could be used.

- [https://github.com/kirubel-cve/CVE-2026-36960](https://github.com/kirubel-cve/CVE-2026-36960) :  ![starts](https://img.shields.io/github/stars/kirubel-cve/CVE-2026-36960.svg) ![forks](https://img.shields.io/github/forks/kirubel-cve/CVE-2026-36960.svg)


## CVE-2026-3695
 A vulnerability has been found in SourceCodester Modern Image Gallery App 1.0. Impacted is an unknown function of the file /delete.php. Such manipulation of the argument filename leads to path traversal. It is possible to launch the attack remotely. The exploit has been disclosed to the public and may be used.

- [https://github.com/kirubel-cve/CVE-2026-36958](https://github.com/kirubel-cve/CVE-2026-36958) :  ![starts](https://img.shields.io/github/stars/kirubel-cve/CVE-2026-36958.svg) ![forks](https://img.shields.io/github/forks/kirubel-cve/CVE-2026-36958.svg)
- [https://github.com/kirubel-cve/CVE-2026-36956](https://github.com/kirubel-cve/CVE-2026-36956) :  ![starts](https://img.shields.io/github/stars/kirubel-cve/CVE-2026-36956.svg) ![forks](https://img.shields.io/github/forks/kirubel-cve/CVE-2026-36956.svg)
- [https://github.com/kirubel-cve/CVE-2026-36959](https://github.com/kirubel-cve/CVE-2026-36959) :  ![starts](https://img.shields.io/github/stars/kirubel-cve/CVE-2026-36959.svg) ![forks](https://img.shields.io/github/forks/kirubel-cve/CVE-2026-36959.svg)
- [https://github.com/kirubel-cve/CVE-2026-36957](https://github.com/kirubel-cve/CVE-2026-36957) :  ![starts](https://img.shields.io/github/stars/kirubel-cve/CVE-2026-36957.svg) ![forks](https://img.shields.io/github/forks/kirubel-cve/CVE-2026-36957.svg)


## CVE-2025-67779
 It was found that the fix addressing CVE-2025-55184 in React Server Components was incomplete and does not prevent a denial of service attack in a specific case. React Server Components versions 19.0.2, 19.1.3 and 19.2.2 are affected, allowing unsafe deserialization of payloads from HTTP requests to Server Function endpoints. This can cause an infinite loop that hangs the server process and may prevent future HTTP requests from being served.

- [https://github.com/Theori-lO/reactguard](https://github.com/Theori-lO/reactguard) :  ![starts](https://img.shields.io/github/stars/Theori-lO/reactguard.svg) ![forks](https://img.shields.io/github/forks/Theori-lO/reactguard.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-git-dep.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-berry.svg)


## CVE-2025-61984
 ssh in OpenSSH before 10.1 allows control characters in usernames that originate from certain possibly untrusted sources, potentially leading to code execution when a ProxyCommand is used. The untrusted sources are the command line and %-sequence expansion of a configuration file. (A configuration file that provides a complete literal username is not categorized as an untrusted source.)

- [https://github.com/Ogrizok-SOC/evil-repo](https://github.com/Ogrizok-SOC/evil-repo) :  ![starts](https://img.shields.io/github/stars/Ogrizok-SOC/evil-repo.svg) ![forks](https://img.shields.io/github/forks/Ogrizok-SOC/evil-repo.svg)


## CVE-2025-56537
 A stored cross-site scripting (XSS) vulnerability in opennebula v6.10.0.1 and fixed in v.7.0 allows attackers to execute arbitrary web scripts or HTML via injecting a crafted payload into the virtual network template parameter.

- [https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56537](https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56537) :  ![starts](https://img.shields.io/github/stars/MarkArtamonov/OpenNebula-CVE-2025-56537.svg) ![forks](https://img.shields.io/github/forks/MarkArtamonov/OpenNebula-CVE-2025-56537.svg)


## CVE-2025-56536
 A stored cross-site scripting (XSS) vulnerability in opennebula v6.10.0.1 allows attackers to execute arbitrary web scripts or HTML via injecting a crafted payload into the user information parameter.

- [https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56536](https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56536) :  ![starts](https://img.shields.io/github/stars/MarkArtamonov/OpenNebula-CVE-2025-56536.svg) ![forks](https://img.shields.io/github/forks/MarkArtamonov/OpenNebula-CVE-2025-56536.svg)


## CVE-2025-56535
 A cross-site scripting (XSS) vulnerability in opennebula v6.10.0.1 allows attackers to execute arbitrary web scripts or HTML via injecting a crafted payload into the zone attribute parameter.

- [https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56535](https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56535) :  ![starts](https://img.shields.io/github/stars/MarkArtamonov/OpenNebula-CVE-2025-56535.svg) ![forks](https://img.shields.io/github/forks/MarkArtamonov/OpenNebula-CVE-2025-56535.svg)


## CVE-2025-56534
 A cross-site scripting (XSS) vulnerability in the custom authenticator driver of opennebula v6.10.0.1 allows attackers to execute arbitrary web scripts or HTML via a crafted payload.

- [https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56534](https://github.com/MarkArtamonov/OpenNebula-CVE-2025-56534) :  ![starts](https://img.shields.io/github/stars/MarkArtamonov/OpenNebula-CVE-2025-56534.svg) ![forks](https://img.shields.io/github/forks/MarkArtamonov/OpenNebula-CVE-2025-56534.svg)


## CVE-2025-55184
 A pre-authentication denial of service vulnerability exists in React Server Components versions 19.0.0, 19.0.1 19.1.0, 19.1.1, 19.1.2, 19.2.0 and 19.2.1, including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. The vulnerable code unsafely deserializes payloads from HTTP requests to Server Function endpoints, which can cause an infinite loop that hangs the server process and may prevent future HTTP requests from being served.

- [https://github.com/Theori-lO/reactguard](https://github.com/Theori-lO/reactguard) :  ![starts](https://img.shields.io/github/stars/Theori-lO/reactguard.svg) ![forks](https://img.shields.io/github/forks/Theori-lO/reactguard.svg)


## CVE-2025-55183
 An information leak vulnerability exists in specific configurations of React Server Components versions 19.0.0, 19.0.1 19.1.0, 19.1.1, 19.1.2, 19.2.0 and 19.2.1, including the following packages: react-server-dom-parcel, react-server-dom-turbopack, and react-server-dom-webpack. A specifically crafted HTTP request sent to a vulnerable Server Function may unsafely return the source code of any Server Function. Exploitation requires the existence of a Server Function which explicitly or implicitly exposes a stringified argument.

- [https://github.com/Theori-lO/reactguard](https://github.com/Theori-lO/reactguard) :  ![starts](https://img.shields.io/github/stars/Theori-lO/reactguard.svg) ![forks](https://img.shields.io/github/forks/Theori-lO/reactguard.svg)


## CVE-2025-14180
 In PHP versions 8.1.* before 8.1.34, 8.2.* before 8.2.30, 8.3.* before 8.3.29, 8.4.* before 8.4.16, 8.5.* before 8.5.1 when using the PDO PostgreSQL driver with PDO::ATTR_EMULATE_PREPARES enabled, an invalid character sequence (such as \x99) in a prepared statement parameter may cause the quoting function PQescapeStringConn to return NULL, leading to a null pointer dereference in pdo_parse_params() function. This may lead to crashes (segmentation fault) and affect the availability of the target server.

- [https://github.com/gl1tch0x1/PHP_8.1.x_Exploit](https://github.com/gl1tch0x1/PHP_8.1.x_Exploit) :  ![starts](https://img.shields.io/github/stars/gl1tch0x1/PHP_8.1.x_Exploit.svg) ![forks](https://img.shields.io/github/forks/gl1tch0x1/PHP_8.1.x_Exploit.svg)


## CVE-2025-14178
 In PHP versions:8.1.* before 8.1.34, 8.2.* before 8.2.30, 8.3.* before 8.3.29, 8.4.* before 8.4.16, 8.5.* before 8.5.1, a heap buffer overflow occurs in array_merge() when the total element count of packed arrays exceeds 32-bit limits or HT_MAX_SIZE, due to an integer overflow in the precomputation of element counts using zend_hash_num_elements(). This may lead to memory corruption or crashes and affect the integrity and availability of the target server.

- [https://github.com/gl1tch0x1/PHP_8.1.x_Exploit](https://github.com/gl1tch0x1/PHP_8.1.x_Exploit) :  ![starts](https://img.shields.io/github/stars/gl1tch0x1/PHP_8.1.x_Exploit.svg) ![forks](https://img.shields.io/github/forks/gl1tch0x1/PHP_8.1.x_Exploit.svg)


## CVE-2025-14177
 In PHP versions:8.1.* before 8.1.34, 8.2.* before 8.2.30, 8.3.* before 8.3.29, 8.4.* before 8.4.16, 8.5.* before 8.5.1, the getimagesize() function may leak uninitialized heap memory into the APPn segments (e.g., APP1) when reading images in multi-chunk mode (such as via php://filter). This occurs due to a bug in php_read_stream_all_chunks() that overwrites the buffer without advancing the pointer, leaving tail bytes uninitialized. This may lead to information disclosure of sensitive heap data and affect the confidentiality of the target server.

- [https://github.com/gl1tch0x1/PHP_8.1.x_Exploit](https://github.com/gl1tch0x1/PHP_8.1.x_Exploit) :  ![starts](https://img.shields.io/github/stars/gl1tch0x1/PHP_8.1.x_Exploit.svg) ![forks](https://img.shields.io/github/forks/gl1tch0x1/PHP_8.1.x_Exploit.svg)


## CVE-2025-5184
 A vulnerability was found in Summer Pearl Group Vacation Rental Management Platform up to 1.0.1. It has been classified as problematic. Affected is an unknown function of the component HTTP Response Header Handler. The manipulation leads to information disclosure. It is possible to launch the attack remotely. Upgrading to version 1.0.2 is able to address this issue. It is recommended to upgrade the affected component.

- [https://github.com/JohnPerifanis/cryptpad-cve-2025-51846-advisory](https://github.com/JohnPerifanis/cryptpad-cve-2025-51846-advisory) :  ![starts](https://img.shields.io/github/stars/JohnPerifanis/cryptpad-cve-2025-51846-advisory.svg) ![forks](https://img.shields.io/github/forks/JohnPerifanis/cryptpad-cve-2025-51846-advisory.svg)


## CVE-2024-29988
 SmartScreen Prompt Security Feature Bypass Vulnerability

- [https://github.com/dinhthihanhle1989-max/CVE-2024-29988](https://github.com/dinhthihanhle1989-max/CVE-2024-29988) :  ![starts](https://img.shields.io/github/stars/dinhthihanhle1989-max/CVE-2024-29988.svg) ![forks](https://img.shields.io/github/forks/dinhthihanhle1989-max/CVE-2024-29988.svg)


## CVE-2024-8503
 An unauthenticated attacker can leverage a time-based SQL injection vulnerability in VICIdial to enumerate database records. By default, VICIdial stores plaintext credentials within the database.

- [https://github.com/Machine-farmer/vicidial-cve-2024-8503-blind-sqli-poc](https://github.com/Machine-farmer/vicidial-cve-2024-8503-blind-sqli-poc) :  ![starts](https://img.shields.io/github/stars/Machine-farmer/vicidial-cve-2024-8503-blind-sqli-poc.svg) ![forks](https://img.shields.io/github/forks/Machine-farmer/vicidial-cve-2024-8503-blind-sqli-poc.svg)


## CVE-2024-6485
 A security vulnerability has been discovered in bootstrap that could enable Cross-Site Scripting (XSS) attacks. The vulnerability is associated with the data-loading-text attribute within the button plugin. This vulnerability can be exploited by injecting malicious JavaScript code into the attribute, which would then be executed when the button's loading state is triggered.

- [https://github.com/harley-ghostie/bootstrap_cve_2024_6485](https://github.com/harley-ghostie/bootstrap_cve_2024_6485) :  ![starts](https://img.shields.io/github/stars/harley-ghostie/bootstrap_cve_2024_6485.svg) ![forks](https://img.shields.io/github/forks/harley-ghostie/bootstrap_cve_2024_6485.svg)


## CVE-2023-46604
which fixes this issue.

- [https://github.com/Navya240/intel471-threat-hunting-cve-2023-46604](https://github.com/Navya240/intel471-threat-hunting-cve-2023-46604) :  ![starts](https://img.shields.io/github/stars/Navya240/intel471-threat-hunting-cve-2023-46604.svg) ![forks](https://img.shields.io/github/forks/Navya240/intel471-threat-hunting-cve-2023-46604.svg)


## CVE-2023-45471
 The QAD Search Server is vulnerable to Stored Cross-Site Scripting (XSS) in versions up to, and including, 1.0.0.315 due to insufficient checks on indexes. This makes it possible for unauthenticated attackers to create a new index and inject a malicious web script into its name, that will execute whenever a user accesses the search page.

- [https://github.com/aptx0x/CVE-2023-45471](https://github.com/aptx0x/CVE-2023-45471) :  ![starts](https://img.shields.io/github/stars/aptx0x/CVE-2023-45471.svg) ![forks](https://img.shields.io/github/forks/aptx0x/CVE-2023-45471.svg)


## CVE-2023-38831
 RARLAB WinRAR before 6.23 allows attackers to execute arbitrary code when a user attempts to view a benign file within a ZIP archive. The issue occurs because a ZIP archive may include a benign file (such as an ordinary .JPG file) and also a folder that has the same name as the benign file, and the contents of the folder (which may include executable content) are processed during an attempt to access only the benign file. This was exploited in the wild in April through October 2023.

- [https://github.com/lightningspeed221/Winrar-Exploit-CVE-2023-38831](https://github.com/lightningspeed221/Winrar-Exploit-CVE-2023-38831) :  ![starts](https://img.shields.io/github/stars/lightningspeed221/Winrar-Exploit-CVE-2023-38831.svg) ![forks](https://img.shields.io/github/forks/lightningspeed221/Winrar-Exploit-CVE-2023-38831.svg)


## CVE-2023-28121
 An issue in WooCommerce Payments plugin for WordPress (versions 5.6.1 and lower) allows an unauthenticated attacker to send requests on behalf of an elevated user, like administrator. This allows a remote, unauthenticated attacker to gain admin access on a site that has the affected version of the plugin activated.

- [https://github.com/luisdevpentest/-CVE-2023-28121-WordPress-Privilege-Escalation](https://github.com/luisdevpentest/-CVE-2023-28121-WordPress-Privilege-Escalation) :  ![starts](https://img.shields.io/github/stars/luisdevpentest/-CVE-2023-28121-WordPress-Privilege-Escalation.svg) ![forks](https://img.shields.io/github/forks/luisdevpentest/-CVE-2023-28121-WordPress-Privilege-Escalation.svg)


## CVE-2023-4842
 The Social Sharing Plugin - Social Warfare plugin for WordPress is vulnerable to Stored Cross-Site Scripting via 'social_warfare' shortcode in versions up to, and including, 4.4.3 due to insufficient input sanitization and output escaping on user supplied attributes. This makes it possible for authenticated attackers with contributor-level and above permissions to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page.

- [https://github.com/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest](https://github.com/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest) :  ![starts](https://img.shields.io/github/stars/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest.svg) ![forks](https://img.shields.io/github/forks/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest.svg)


## CVE-2022-32250
 net/netfilter/nf_tables_api.c in the Linux kernel through 5.18.1 allows a local user (able to create user/net namespaces) to escalate privileges to root because an incorrect NFT_STATEFUL_EXPR check leads to a use-after-free.

- [https://github.com/Theori-lO/CVE-2022-32250-exploit](https://github.com/Theori-lO/CVE-2022-32250-exploit) :  ![starts](https://img.shields.io/github/stars/Theori-lO/CVE-2022-32250-exploit.svg) ![forks](https://img.shields.io/github/forks/Theori-lO/CVE-2022-32250-exploit.svg)


## CVE-2022-26717
 A use after free issue was addressed with improved memory management. This issue is fixed in tvOS 15.5, watchOS 8.6, iOS 15.5 and iPadOS 15.5, macOS Monterey 12.4, Safari 15.5, iTunes 12.12.4 for Windows. Processing maliciously crafted web content may lead to arbitrary code execution.

- [https://github.com/Theori-lO/CVE-2022-26717-Safari-WebGL-Exploit](https://github.com/Theori-lO/CVE-2022-26717-Safari-WebGL-Exploit) :  ![starts](https://img.shields.io/github/stars/Theori-lO/CVE-2022-26717-Safari-WebGL-Exploit.svg) ![forks](https://img.shields.io/github/forks/Theori-lO/CVE-2022-26717-Safari-WebGL-Exploit.svg)


## CVE-2020-0162
 In parseSampleAuxiliaryInformationOffsets of MPEG4Extractor.cpp, there is possible resource exhaustion due to improper input validation. This could lead to remote denial of service with no additional execution privileges needed. User interaction is needed for exploitation.Product: AndroidVersions: Android-10Android ID: A-124526959

- [https://github.com/Pazhanivelmani/av_CVE-2020-0162_A10r33](https://github.com/Pazhanivelmani/av_CVE-2020-0162_A10r33) :  ![starts](https://img.shields.io/github/stars/Pazhanivelmani/av_CVE-2020-0162_A10r33.svg) ![forks](https://img.shields.io/github/forks/Pazhanivelmani/av_CVE-2020-0162_A10r33.svg)


## CVE-2019-9978
 The social-warfare plugin before 3.5.3 for WordPress has stored XSS via the wp-admin/admin-post.php?swp_debug=load_options swp_url parameter, as exploited in the wild in March 2019. This affects Social Warfare and Social Warfare Pro.

- [https://github.com/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest](https://github.com/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest) :  ![starts](https://img.shields.io/github/stars/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest.svg) ![forks](https://img.shields.io/github/forks/B4ntGrim/Vuln_Exploitation_MegaQuagga_Pentest.svg)
- [https://github.com/B4ntGrim/Vuln_Remediation_MegaQuagga](https://github.com/B4ntGrim/Vuln_Remediation_MegaQuagga) :  ![starts](https://img.shields.io/github/stars/B4ntGrim/Vuln_Remediation_MegaQuagga.svg) ![forks](https://img.shields.io/github/forks/B4ntGrim/Vuln_Remediation_MegaQuagga.svg)


## CVE-2019-9511
 Some HTTP/2 implementations are vulnerable to window size manipulation and stream prioritization manipulation, potentially leading to a denial of service. The attacker requests a large amount of data from a specified resource over multiple streams. They manipulate window size and stream priority to force the server to queue the data in 1-byte chunks. Depending on how efficiently this data is queued, this can consume excess CPU, memory, or both.

- [https://github.com/harley-ghostie/CVE-2019-9511_Priority-Churn-Data-Dribble](https://github.com/harley-ghostie/CVE-2019-9511_Priority-Churn-Data-Dribble) :  ![starts](https://img.shields.io/github/stars/harley-ghostie/CVE-2019-9511_Priority-Churn-Data-Dribble.svg) ![forks](https://img.shields.io/github/forks/harley-ghostie/CVE-2019-9511_Priority-Churn-Data-Dribble.svg)


## CVE-2018-14847
 MikroTik RouterOS through 6.42 allows unauthenticated remote attackers to read arbitrary files and remote authenticated attackers to write arbitrary files due to a directory traversal vulnerability in the WinBox interface.

- [https://github.com/TheMalwareGuardian/CVE-2018-14847](https://github.com/TheMalwareGuardian/CVE-2018-14847) :  ![starts](https://img.shields.io/github/stars/TheMalwareGuardian/CVE-2018-14847.svg) ![forks](https://img.shields.io/github/forks/TheMalwareGuardian/CVE-2018-14847.svg)

