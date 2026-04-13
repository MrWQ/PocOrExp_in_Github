# Update 2026-04-13
## CVE-2026-33229
 XWiki Platform is a generic wiki platform offering runtime services for applications built on top of it. Prior to 17.4.8 and 17.10.1, an improperly protected scripting API allows any user with script right to bypass the sandboxing of the Velocity scripting API and execute, e.g., arbitrary Python scripts, allowing full access to the XWiki instance and thereby compromising the confidentiality, integrity and availability of the whole instance. Note that script right already constitutes a high level of access that we don't recommend giving to untrusted users. This vulnerability is fixed in 17.4.8 and 17.10.1.

- [https://github.com/azefzafyoussef/CVE-2026-33229](https://github.com/azefzafyoussef/CVE-2026-33229) :  ![starts](https://img.shields.io/github/stars/azefzafyoussef/CVE-2026-33229.svg) ![forks](https://img.shields.io/github/forks/azefzafyoussef/CVE-2026-33229.svg)


## CVE-2026-31900
 Black is the uncompromising Python code formatter. Black provides a GitHub action for formatting code. This action supports an option, use_pyproject: true, for reading the version of Black to use from the repository pyproject.toml. A malicious pull request could edit pyproject.toml to use a direct URL reference to a malicious repository. This could lead to arbitrary code execution in the context of the GitHub Action. Attackers could then gain access to secrets or permissions available in the context of the action. Version 26.3.0 fixes this vulnerability.

- [https://github.com/Batosay1337Lab/cve-2026-31900-lab](https://github.com/Batosay1337Lab/cve-2026-31900-lab) :  ![starts](https://img.shields.io/github/stars/Batosay1337Lab/cve-2026-31900-lab.svg) ![forks](https://img.shields.io/github/forks/Batosay1337Lab/cve-2026-31900-lab.svg)


## CVE-2026-27621
 TypiCMS is a multilingual content management system based on the Laravel framework. A Stored Cross-Site Scripting (XSS) vulnerability exists in the file upload module of TypiCMS prior to version 16.1.7. The application allows users with file upload permissions to upload SVG files. While there is a MIME type validation, the content of the SVG file is not sanitized. An attacker can upload a specially crafted SVG file containing malicious JavaScript code. When another user (such as an administrator) views or accesses this file through the application, the script executes in their browser, leading to a compromise of that user's session. The issue is exacerbated by a bug in the SVG parsing logic, which can cause a 500 error if the uploaded SVG does not contain a `viewBox` attribute. However, this does not mitigate the XSS vulnerability, as an attacker can easily include a valid `viewBox` attribute in their malicious payload. Version 16.1.7 of TypiCMS Core fixes the issue.

- [https://github.com/lukasz-rybak/CVE-2026-27621](https://github.com/lukasz-rybak/CVE-2026-27621) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-27621.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-27621.svg)


## CVE-2026-25514
 FacturaScripts is open-source enterprise resource planning and accounting software. Prior to version 2025.81, FacturaScripts contains a critical SQL injection vulnerability in the autocomplete functionality that allows authenticated attackers to extract sensitive data from the database including user credentials, configuration settings, and all stored business data. The vulnerability exists in the CodeModel::all() method where user-supplied parameters are directly concatenated into SQL queries without sanitization or parameterized binding. This issue has been patched in version 2025.81.

- [https://github.com/lukasz-rybak/CVE-2026-25514](https://github.com/lukasz-rybak/CVE-2026-25514) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-25514.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-25514.svg)


## CVE-2026-25513
 FacturaScripts is open-source enterprise resource planning and accounting software. Prior to version 2025.81, FacturaScripts contains a critical SQL injection vulnerability in the REST API that allows authenticated API users to execute arbitrary SQL queries through the sort parameter. The vulnerability exists in the ModelClass::getOrderBy() method where user-supplied sorting parameters are directly concatenated into the SQL ORDER BY clause without validation or sanitization. This affects all API endpoints that support sorting functionality. This issue has been patched in version 2025.81.

- [https://github.com/lukasz-rybak/CVE-2026-25513](https://github.com/lukasz-rybak/CVE-2026-25513) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-25513.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-25513.svg)


## CVE-2026-24419
 OpenSTAManager is an open source management software for technical assistance and invoicing. OpenSTAManager v2.9.8 and earlier contain a critical Error-Based SQL Injection vulnerability in the Prima Nota (Journal Entry) module's add.php file. The application fails to validate that comma-separated values from the id_documenti GET parameter are integers before using them in SQL IN() clauses, allowing attackers to inject arbitrary SQL commands and extract sensitive data through XPATH error messages.

- [https://github.com/lukasz-rybak/CVE-2026-24419](https://github.com/lukasz-rybak/CVE-2026-24419) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-24419.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-24419.svg)


## CVE-2026-24418
 OpenSTAManager is an open source management software for technical assistance and invoicing. OpenSTAManager v2.9.8 and earlier contain a critical Error-Based SQL Injection vulnerability in the bulk operations handler for the Scadenzario (Payment Schedule) module. The application fails to validate that elements of the id_records array are integers before using them in an SQL IN() clause, allowing attackers to inject arbitrary SQL commands and extract sensitive data through XPATH error messages.

- [https://github.com/lukasz-rybak/CVE-2026-24418](https://github.com/lukasz-rybak/CVE-2026-24418) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-24418.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-24418.svg)


## CVE-2026-24417
 OpenSTAManager is an open source management software for technical assistance and invoicing. OpenSTAManager v2.9.8 and earlier contain a critical Time-Based Blind SQL Injection vulnerability in the global search functionality. The application fails to properly sanitize the term parameter before using it in SQL LIKE clauses across multiple module-specific search handlers, allowing attackers to inject arbitrary SQL commands and extract sensitive data through time-based Boolean inference.

- [https://github.com/lukasz-rybak/CVE-2026-24417](https://github.com/lukasz-rybak/CVE-2026-24417) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-24417.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-24417.svg)


## CVE-2026-24416
 OpenSTAManager is an open source management software for technical assistance and invoicing. OpenSTAManager v2.9.8 and earlier contain a critical Time-Based Blind SQL Injection vulnerability in the article pricing completion handler. The application fails to properly sanitize the idarticolo parameter before using it in SQL queries, allowing attackers to inject arbitrary SQL commands and extract sensitive data through time-based Boolean inference.

- [https://github.com/lukasz-rybak/CVE-2026-24416](https://github.com/lukasz-rybak/CVE-2026-24416) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-24416.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-24416.svg)


## CVE-2026-24415
 OpenSTAManager is an open source management software for technical assistance and invoicing. OpenSTAManager v2.9.8 and earlier contains Reflected XSS vulnerabilities in invoice/order/contract modification modals. The application fails to properly sanitize user-supplied input from the righe GET parameter before reflecting it in HTML output.The $_GET['righe'] parameter is directly echoed into the HTML value attribute without any sanitization using htmlspecialchars() or equivalent functions. This allows an attacker to break out of the attribute context and inject arbitrary HTML/JavaScript.

- [https://github.com/lukasz-rybak/CVE-2026-24415](https://github.com/lukasz-rybak/CVE-2026-24415) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-24415.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-24415.svg)


## CVE-2026-23869
 A denial of service vulnerability exists in React Server Components, affecting the following packages: react-server-dom-parcel, react-server-dom-turbopack and react-server-dom-webpack (versions 19.0.0 through 19.0.4, 19.1.0 through 19.1.5, and 19.2.0 through 19.2.4). The vulnerability is triggered by sending specially crafted HTTP requests to Server Function endpoints.The payload of the HTTP request causes excessive CPU usage for up to a minute ending in a thrown error that is catchable.

- [https://github.com/cybertechajju/CVE-2026-23869-Exploit](https://github.com/cybertechajju/CVE-2026-23869-Exploit) :  ![starts](https://img.shields.io/github/stars/cybertechajju/CVE-2026-23869-Exploit.svg) ![forks](https://img.shields.io/github/forks/cybertechajju/CVE-2026-23869-Exploit.svg)


## CVE-2026-23499
 Saleor is an e-commerce platform. Starting in version 3.0.0 and prior to versions 3.20.108, 3.21.43, and 3.22.27, Saleor allowed authenticated staff users or Apps to upload arbitrary files, including malicious HTML and SVG files containing Javascript. Depending on the deployment strategy, these files may be served from the same domain as the dashboard without any restrictions leading to the execution of malicious scripts in the context of the user's browser. Malicious staff members could craft script injections to target other staff members, possibly stealing their access and/or refresh tokens. Users are vulnerable if they host the media files inside the same domain as the dashboard, e.g., dashboard is at `example.com/dashboard/` and media are under `example.com/media/`. They are not impact if media files are hosted in a different domain, e.g., `media.example.com`. Users are impacted if they do not return a `Content-Disposition: attachment` header for the media files. Saleor Cloud users are not impacted. This issue has been patched in versions: 3.22.27, 3.21.43, and 3.20.108. Some workarounds are available for those unable to upgrade. Configure the servers hosting the media files (e.g., CDN or reverse proxy) to return the Content-Disposition: attachment header. This instructs browsers to download the file instead of rendering them in the browser. Prevent the servers from returning HTML and SVG files. Set-up a `Content-Security-Policy` for media files, such as `Content-Security-Policy: default-src 'none'; base-uri 'none'; frame-ancestors 'none'; form-action 'none';`.

- [https://github.com/lukasz-rybak/CVE-2026-23499](https://github.com/lukasz-rybak/CVE-2026-23499) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-23499.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-23499.svg)


## CVE-2026-23498
 Shopware is an open commerce platform. From 6.7.0.0 to before 6.7.6.1, a regression of CVE-2023-2017 leads to an array and array crafted PHP Closure not checked being against allow list for the map(...) override. This vulnerability is fixed in 6.7.6.1.

- [https://github.com/lukasz-rybak/CVE-2026-23498](https://github.com/lukasz-rybak/CVE-2026-23498) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-23498.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-23498.svg)


## CVE-2026-23491
 InvoicePlane is a self-hosted open source application for managing invoices, clients, and payments. A path traversal vulnerability exists in the `get_file` method of the `Guest` module's `Get` controller in InvoicePlane up to and including through 1.6.3. The vulnerability allows unauthenticated attackers to read arbitrary files on the server by manipulating the input filename. This leads to the disclosure of sensitive information, including configuration files with database credentials. Version 1.6.4 fixes the issue.

- [https://github.com/lukasz-rybak/CVE-2026-23491](https://github.com/lukasz-rybak/CVE-2026-23491) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-23491.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-23491.svg)


## CVE-2026-22849
 Saleor is an e-commerce platform. Starting in version 3.0.0 and prior to versions 3.20.108, 3.21.43, and 3.22.27, Saleor was allowing users to modify rich text fields with HTML without running any backend HTML cleaners thus allowing malicious actors to perform stored XSS attacks on dashboards and storefronts. Malicious staff members could craft script injections to target other staff members, possibly stealing their access and/or refresh tokens. This issue has been patched in versions 3.22.27, 3.21.43, and 3.20.108. In case of inability to upgrade straight away, a possible workaround is to use client-side cleaner.

- [https://github.com/lukasz-rybak/CVE-2026-22849](https://github.com/lukasz-rybak/CVE-2026-22849) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-22849.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-22849.svg)


## CVE-2026-22557
 A malicious actor with access to the network could exploit a Path Traversal vulnerability found in the UniFi Network Application to access files on the underlying system that could be manipulated to access an underlying account.

- [https://github.com/ThePotatoOfDoom/CVE-2026-22557-PoC](https://github.com/ThePotatoOfDoom/CVE-2026-22557-PoC) :  ![starts](https://img.shields.io/github/stars/ThePotatoOfDoom/CVE-2026-22557-PoC.svg) ![forks](https://img.shields.io/github/forks/ThePotatoOfDoom/CVE-2026-22557-PoC.svg)


## CVE-2026-22243
 EGroupware is a Web based groupware server written in PHP. A SQL Injection vulnerability exists in the core components of EGroupware prior to versions 23.1.20260113 and 26.0.20260113, specifically in the `Nextmatch` filter processing. The flaw allows authenticated attackers to inject arbitrary SQL commands into the `WHERE` clause of database queries. This is achieved by exploiting a PHP type juggling issue where JSON decoding converts numeric strings into integers, bypassing the `is_int()` security check used by the application. Versions 23.1.20260113 and 26.0.20260113 patch the vulnerability.

- [https://github.com/lukasz-rybak/CVE-2026-22243](https://github.com/lukasz-rybak/CVE-2026-22243) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-22243.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-22243.svg)


## CVE-2026-21857
 REDAXO is a PHP-based content management system. Prior to version 5.20.2, authenticated users with backup permissions can read arbitrary files within the webroot via path traversal in the Backup addon's file export functionality. The Backup addon does not validate the `EXPDIR` POST parameter against the UI-generated allowlist of permitted directories. An attacker can supply relative paths containing `../` sequences (or even absolute paths inside the document root) to include any readable file in the generated `.tar.gz` archive. Version 5.20.2 fixes this issue.

- [https://github.com/lukasz-rybak/CVE-2026-21857](https://github.com/lukasz-rybak/CVE-2026-21857) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-21857.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-21857.svg)


## CVE-2026-4350
 The Perfmatters plugin for WordPress is vulnerable to arbitrary file deletion via path traversal in all versions up to, and including, 2.5.9.1. This is due to the `PMCS::action_handler()` method processing the `$_GET['delete']` parameter without any sanitization, authorization check, or nonce verification. The unsanitized filename is concatenated with the storage directory path and passed to `unlink()`. This makes it possible for authenticated attackers, with Subscriber-level access and above, to delete arbitrary files on the server by using `../` path traversal sequences, including `wp-config.php` which would force WordPress into the installation wizard and allow full site takeover.

- [https://github.com/whyiamsobusy/CVE-2026-4350](https://github.com/whyiamsobusy/CVE-2026-4350) :  ![starts](https://img.shields.io/github/stars/whyiamsobusy/CVE-2026-4350.svg) ![forks](https://img.shields.io/github/forks/whyiamsobusy/CVE-2026-4350.svg)


## CVE-2026-3986
 The Calculated Fields Form plugin for WordPress is vulnerable to Stored Cross-Site Scripting via the form settings in all versions up to, and including, 5.4.5.0. This is due to insufficient capability checks on the form settings save handler and insufficient input sanitization of the `fcontent` field in `fhtml` field types. This makes it possible for authenticated attackers, with Contributor-level access and above, to inject arbitrary web scripts in pages that will execute whenever a user accesses an injected page.

- [https://github.com/abhayclasher/CVE-2026-39866](https://github.com/abhayclasher/CVE-2026-39866) :  ![starts](https://img.shields.io/github/stars/abhayclasher/CVE-2026-39866.svg) ![forks](https://img.shields.io/github/forks/abhayclasher/CVE-2026-39866.svg)


## CVE-2026-2350
 Tanium addressed an insertion of sensitive information into log file vulnerability in Interact and TDS.

- [https://github.com/lukasz-rybak/CVE-2026-23500](https://github.com/lukasz-rybak/CVE-2026-23500) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-23500.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-23500.svg)


## CVE-2026-1434
This issue was fixed in 4.6.7.

- [https://github.com/lukasz-rybak/CVE-2026-1434](https://github.com/lukasz-rybak/CVE-2026-1434) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2026-1434.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2026-1434.svg)


## CVE-2025-69216
 OpenSTAManager is an open source management software for technical assistance and invoicing. In 2.9.8 and earlier, an authenticated SQL injection vulnerability in OpenSTAManager's Scadenzario (Payment Schedule) print template allows any authenticated user to extract sensitive data from the database, including admin credentials, customer information, and financial records. The vulnerability exists in templates/scadenzario/init.php, where the id_anagrafica parameter is directly concatenated into an SQL query without proper sanitization. The vulnerability enables complete database read access through error-based SQL injection techniques.

- [https://github.com/lukasz-rybak/CVE-2025-69216](https://github.com/lukasz-rybak/CVE-2025-69216) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-69216.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-69216.svg)


## CVE-2025-69215
 OpenSTAManager is an open source management software for technical assistance and invoicing. In version 2.9.8 and prior, there is a SQL Injection vulnerability in the Stampe Module. At time of publication, no known patch exists.

- [https://github.com/lukasz-rybak/CVE-2025-69215](https://github.com/lukasz-rybak/CVE-2025-69215) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-69215.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-69215.svg)


## CVE-2025-69214
 OpenSTAManager is an open source management software for technical assistance and invoicing. In 2.9.8 and earlier, an SQL Injection vulnerability exists in the ajax_select.php endpoint when handling the componenti operation. An authenticated attacker can inject malicious SQL code through the options[matricola] parameter.

- [https://github.com/lukasz-rybak/CVE-2025-69214](https://github.com/lukasz-rybak/CVE-2025-69214) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-69214.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-69214.svg)


## CVE-2025-69213
 OpenSTAManager is an open source management software for technical assistance and invoicing. In version 2.9.8 and prior, a SQL Injection vulnerability exists in the ajax_complete.php endpoint when handling the get_sedi operation. An authenticated attacker can inject malicious SQL code through the idanagrafica parameter, leading to unauthorized database access. At time of publication, no known patch exists.

- [https://github.com/lukasz-rybak/CVE-2025-69213](https://github.com/lukasz-rybak/CVE-2025-69213) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-69213.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-69213.svg)


## CVE-2025-69212
 OpenSTAManager is an open source management software for technical assistance and invoicing. In 2.9.8 and earlier, a critical OS Command Injection vulnerability exists in the P7M (signed XML) file decoding functionality. An authenticated attacker can upload a ZIP file containing a .p7m file with a malicious filename to execute arbitrary system commands on the server.

- [https://github.com/lukasz-rybak/CVE-2025-69212](https://github.com/lukasz-rybak/CVE-2025-69212) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-69212.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-69212.svg)


## CVE-2025-68400
 ChurchCRM is an open-source church management system. A SQL Injection vulnerability exists in the legacy endpoint `/Reports/ConfirmReportEmail.php` in ChurchCRM prior to version 6.5.3. Although the feature was removed from the UI, the file remains deployed and reachable directly via URL. This is a classic case of *dead but reachable code*. Any authenticated user - including one with zero assigned permissions - can exploit SQL injection through the `familyId` parameter. Version 6.5.3 fixes the issue.

- [https://github.com/lukasz-rybak/CVE-2025-68400](https://github.com/lukasz-rybak/CVE-2025-68400) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-68400.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-68400.svg)


## CVE-2025-67876
 ChurchCRM is an open-source church management system. A stored cross-site scripting (XSS) vulnerability exists in ChurchCRM versions 6.4.0 and prior that allows a low-privilege user with the “Manage Groups” permission to inject persistent JavaScript into group role names. The payload is saved in the database and executed whenever any user (including administrators) views a page that displays that role, such as GroupView.php or PersonView.php. This allows full session hijacking and account takeover. As of time of publication, no known patched versions are available.

- [https://github.com/lukasz-rybak/CVE-2025-67876](https://github.com/lukasz-rybak/CVE-2025-67876) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-67876.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-67876.svg)


## CVE-2025-67875
 ChurchCRM is an open-source church management system. A privilege escalation vulnerability exists in ChurchCRM prior to version 6.5.3. An authenticated user with specific mid-level permissions ("Edit Records" and "Manage Properties and Classifications") can inject a persistent Cross-Site Scripting (XSS) payload into an administrator's profile. The payload executes when the administrator views their own profile page, allowing the attacker to hijack the administrator's session, perform administrative actions, and achieve a full account takeover. This vulnerability is a combination of two separate flaws: an Insecure Direct Object Reference (IDOR) that allows any user to view any other user's profile, and a Broken Access Control vulnerability that allows a user with general edit permissions to modify any other user's record properties. Version 6.5.3 fixes the issue.

- [https://github.com/lukasz-rybak/CVE-2025-67875](https://github.com/lukasz-rybak/CVE-2025-67875) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-67875.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-67875.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478](https://github.com/lincemorado97/CVE-2025-55182_CVE-2025-66478) :  ![starts](https://img.shields.io/github/stars/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg) ![forks](https://img.shields.io/github/forks/lincemorado97/CVE-2025-55182_CVE-2025-66478.svg)


## CVE-2025-66204
 WBCE CMS is a content management system. Version 1.6.4 contains a brute-force protection bypass where an attacker can indefinitely reset the counter by modifying `X-Forwarded-For` on each request, gaining unlimited password guessing attempts, effectively bypassing all brute-force protection. The application fully trusts the `X-Forwarded-For` header without validating it or restricting its usage. This issue is fixed in version 1.6.5.

- [https://github.com/lukasz-rybak/CVE-2025-66204](https://github.com/lukasz-rybak/CVE-2025-66204) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-66204.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-66204.svg)


## CVE-2025-66024
 The XWiki blog application allows users of the XWiki platform to create and manage blog posts. Versions prior to 9.15.7 are vulnerable to Stored Cross-Site Scripting (XSS) via the Blog Post Title. The vulnerability arises because the post title is injected directly into the HTML title tag without proper escaping. An attacker with permissions to create or edit blog posts can inject malicious JavaScript into the title field. This script will execute in the browser of any user (including administrators) who views the blog post. This leads to potential session hijacking or privilege escalation. The vulnerability has been patched in the blog application version 9.15.7 by adding missing escaping. No known workarounds are available.

- [https://github.com/lukasz-rybak/CVE-2025-66024](https://github.com/lukasz-rybak/CVE-2025-66024) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-66024.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-66024.svg)


## CVE-2025-65950
 WBCE CMS is a content management system. In versions 1.6.4 and below, the user management module allows a low-privileged authenticated user with permissions to modify users to execute arbitrary SQL queries. This can be escalated to a full database compromise, data exfiltration, effectively bypassing all security controls. The vulnerability exists in the admin/users/save.php script, which handles updates to user profiles. The script improperly processes the groups[] parameter sent from the user edit form. This issue is fixed in version 1.6.5.

- [https://github.com/lukasz-rybak/CVE-2025-65950](https://github.com/lukasz-rybak/CVE-2025-65950) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-65950.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-65950.svg)


## CVE-2025-65094
 WBCE CMS is a content management system. Prior to version 1.6.4, a low-privileged user in WBCE CMS can escalate their privileges to the Administrators group by manipulating the groups[] parameter in the /admin/users/save.php request. The UI restricts users to assigning only their existing group, but server-side validation is missing, allowing attackers to overwrite their group membership and obtain full administrative access. This results in a complete compromise of the CMS. This issue has been patched in version 1.6.4.

- [https://github.com/lukasz-rybak/CVE-2025-65094](https://github.com/lukasz-rybak/CVE-2025-65094) :  ![starts](https://img.shields.io/github/stars/lukasz-rybak/CVE-2025-65094.svg) ![forks](https://img.shields.io/github/forks/lukasz-rybak/CVE-2025-65094.svg)


## CVE-2025-59528
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5, Flowise is vulnerable to remote code execution. The CustomMCP node allows users to input configuration settings for connecting to an external MCP server. This node parses the user-provided mcpServerConfig string to build the MCP server configuration. However, during this process, it executes JavaScript code without any security validation. Specifically, inside the convertToValidJSONString function, user input is directly passed to the Function() constructor, which evaluates and executes the input as JavaScript code. Since this runs with full Node.js runtime privileges, it can access dangerous modules such as child_process and fs. This issue has been patched in version 3.0.6.

- [https://github.com/Kamigold/Flowise-RCE](https://github.com/Kamigold/Flowise-RCE) :  ![starts](https://img.shields.io/github/stars/Kamigold/Flowise-RCE.svg) ![forks](https://img.shields.io/github/forks/Kamigold/Flowise-RCE.svg)
- [https://github.com/AzureADTrent/CVE-2025-58434-59528](https://github.com/AzureADTrent/CVE-2025-58434-59528) :  ![starts](https://img.shields.io/github/stars/AzureADTrent/CVE-2025-58434-59528.svg) ![forks](https://img.shields.io/github/forks/AzureADTrent/CVE-2025-58434-59528.svg)
- [https://github.com/CVETeam/FlowiseAI-Critical-KillChain](https://github.com/CVETeam/FlowiseAI-Critical-KillChain) :  ![starts](https://img.shields.io/github/stars/CVETeam/FlowiseAI-Critical-KillChain.svg) ![forks](https://img.shields.io/github/forks/CVETeam/FlowiseAI-Critical-KillChain.svg)


## CVE-2025-58434
 Flowise is a drag & drop user interface to build a customized large language model flow. In version 3.0.5 and earlier, the `forgot-password` endpoint in Flowise returns sensitive information including a valid password reset `tempToken` without authentication or verification. This enables any attacker to generate a reset token for arbitrary users and directly reset their password, leading to a complete account takeover (ATO). This vulnerability applies to both the cloud service (`cloud.flowiseai.com`) and self-hosted/local Flowise deployments that expose the same API. Commit 9e178d68873eb876073846433a596590d3d9c863 in version 3.0.6 secures password reset endpoints. Several recommended remediation steps are available. Do not return reset tokens or sensitive account details in API responses. Tokens must only be delivered securely via the registered email channel. Ensure `forgot-password` responds with a generic success message regardless of input, to avoid user enumeration. Require strong validation of the `tempToken` (e.g., single-use, short expiry, tied to request origin, validated against email delivery). Apply the same fixes to both cloud and self-hosted/local deployments. Log and monitor password reset requests for suspicious activity. Consider multi-factor verification for sensitive accounts.

- [https://github.com/AzureADTrent/CVE-2025-58434-59528](https://github.com/AzureADTrent/CVE-2025-58434-59528) :  ![starts](https://img.shields.io/github/stars/AzureADTrent/CVE-2025-58434-59528.svg) ![forks](https://img.shields.io/github/forks/AzureADTrent/CVE-2025-58434-59528.svg)
- [https://github.com/Kamigold/Flowise-RCE](https://github.com/Kamigold/Flowise-RCE) :  ![starts](https://img.shields.io/github/stars/Kamigold/Flowise-RCE.svg) ![forks](https://img.shields.io/github/forks/Kamigold/Flowise-RCE.svg)
- [https://github.com/CVETeam/FlowiseAI-Critical-KillChain](https://github.com/CVETeam/FlowiseAI-Critical-KillChain) :  ![starts](https://img.shields.io/github/stars/CVETeam/FlowiseAI-Critical-KillChain.svg) ![forks](https://img.shields.io/github/forks/CVETeam/FlowiseAI-Critical-KillChain.svg)


## CVE-2025-49113
 Roundcube Webmail before 1.5.10 and 1.6.x before 1.6.11 allows remote code execution by authenticated users because the _from parameter in a URL is not validated in program/actions/settings/upload.php, leading to PHP Object Deserialization.

- [https://github.com/mooder1/CVE-2025-49113](https://github.com/mooder1/CVE-2025-49113) :  ![starts](https://img.shields.io/github/stars/mooder1/CVE-2025-49113.svg) ![forks](https://img.shields.io/github/forks/mooder1/CVE-2025-49113.svg)


## CVE-2025-32433
 Erlang/OTP is a set of libraries for the Erlang programming language. Prior to versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20, a SSH server may allow an attacker to perform unauthenticated remote code execution (RCE). By exploiting a flaw in SSH protocol message handling, a malicious actor could gain unauthorized access to affected systems and execute arbitrary commands without valid credentials. This issue is patched in versions OTP-27.3.3, OTP-26.2.5.11, and OTP-25.3.2.20. A temporary workaround involves disabling the SSH server or to prevent access via firewall rules.

- [https://github.com/l1nuxkid/CVE-2025-32433-exploit](https://github.com/l1nuxkid/CVE-2025-32433-exploit) :  ![starts](https://img.shields.io/github/stars/l1nuxkid/CVE-2025-32433-exploit.svg) ![forks](https://img.shields.io/github/forks/l1nuxkid/CVE-2025-32433-exploit.svg)


## CVE-2025-8110
 Improper Symbolic link handling in the PutContents API in Gogs allows Local Execution of Code.

- [https://github.com/Ghxstsec/CVE-2025-8110](https://github.com/Ghxstsec/CVE-2025-8110) :  ![starts](https://img.shields.io/github/stars/Ghxstsec/CVE-2025-8110.svg) ![forks](https://img.shields.io/github/forks/Ghxstsec/CVE-2025-8110.svg)
- [https://github.com/3jee/CVE-2025-8110](https://github.com/3jee/CVE-2025-8110) :  ![starts](https://img.shields.io/github/stars/3jee/CVE-2025-8110.svg) ![forks](https://img.shields.io/github/forks/3jee/CVE-2025-8110.svg)
- [https://github.com/kayl22/cve-2025-8110-GOGS-RCE](https://github.com/kayl22/cve-2025-8110-GOGS-RCE) :  ![starts](https://img.shields.io/github/stars/kayl22/cve-2025-8110-GOGS-RCE.svg) ![forks](https://img.shields.io/github/forks/kayl22/cve-2025-8110-GOGS-RCE.svg)


## CVE-2023-21563
 BitLocker Security Feature Bypass Vulnerability

- [https://github.com/c-sprinks/bitlocker-bypass-research](https://github.com/c-sprinks/bitlocker-bypass-research) :  ![starts](https://img.shields.io/github/stars/c-sprinks/bitlocker-bypass-research.svg) ![forks](https://img.shields.io/github/forks/c-sprinks/bitlocker-bypass-research.svg)


## CVE-2023-4911
 A buffer overflow was discovered in the GNU C Library's dynamic loader ld.so while processing the GLIBC_TUNABLES environment variable. This issue could allow a local attacker to use maliciously crafted GLIBC_TUNABLES environment variables when launching binaries with SUID permission to execute code with elevated privileges.

- [https://github.com/0xMOGA/CVE-2023-4911-Lab](https://github.com/0xMOGA/CVE-2023-4911-Lab) :  ![starts](https://img.shields.io/github/stars/0xMOGA/CVE-2023-4911-Lab.svg) ![forks](https://img.shields.io/github/forks/0xMOGA/CVE-2023-4911-Lab.svg)


## CVE-2019-15947
 In Bitcoin Core 0.18.0, bitcoin-qt stores wallet.dat data unencrypted in memory. Upon a crash, it may dump a core file. If a user were to mishandle a core file, an attacker can reconstruct the user's wallet.dat file, including their private keys, via a grep "6231 0500" command.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2018-17336
 UDisks 2.8.0 has a format string vulnerability in udisks_log in udiskslogging.c, allowing attackers to obtain sensitive information (stack contents), cause a denial of service (memory corruption), or possibly have unspecified other impact via a malformed filesystem label, as demonstrated by %d or %n substrings.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2017-5816
 A Remote Code Execution vulnerability in HPE Intelligent Management Center (iMC) PLAT version 7.3 E0504P04 was found.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2016-10401
 ZyXEL PK5001Z devices have zyad5001 as the su password, which makes it easier for remote attackers to obtain root access if a non-root account password is known (or a non-root default account exists within an ISP's deployment of these devices).

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)


## CVE-2010-2626
 index.pl in Miyabi CGI Tools SEO Links 1.02 allows remote attackers to execute arbitrary commands via shell metacharacters in the fn command. NOTE: some of these details are obtained from third party information.

- [https://github.com/oxasploits/oxasploits](https://github.com/oxasploits/oxasploits) :  ![starts](https://img.shields.io/github/stars/oxasploits/oxasploits.svg) ![forks](https://img.shields.io/github/forks/oxasploits/oxasploits.svg)

