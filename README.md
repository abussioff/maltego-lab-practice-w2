# maltego-lab-practice-w2
<img width="621" height="482" alt="image" src="https://github.com/user-attachments/assets/c6f25fb9-712d-4418-875e-301c6f00c039" />
<img width="1720" height="879" alt="image" src="https://github.com/user-attachments/assets/84249d6c-d972-4279-b2eb-625c5aef19d9" />
<img width="1887" height="904" alt="image" src="https://github.com/user-attachments/assets/4add95ec-896f-42b8-9f16-9b8ce7e97388" />
<img width="1716" height="893" alt="image" src="https://github.com/user-attachments/assets/16c65217-0fe7-44fa-a455-8169ba4e8be3" />
<img width="1722" height="897" alt="image" src="https://github.com/user-attachments/assets/9a66a2b8-ab61-4b63-afae-64c6edc04126" />
<img width="1709" height="899" alt="image" src="https://github.com/user-attachments/assets/d76e0802-6372-4a71-af7f-6fda18a9cef2" />
<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/d6678adb-b547-4839-9186-e432f9b51ffb" />
<img width="907" height="550" alt="image" src="https://github.com/user-attachments/assets/bf555c37-daf4-4f0e-8964-6a0d0afaef71" />
<img width="1910" height="266" alt="image" src="https://github.com/user-attachments/assets/a2cba943-fa02-4d4e-98cd-b79e5cd2244b" />
<img width="940" height="188" alt="image" src="https://github.com/user-attachments/assets/1f7b1a0e-7855-4d2e-a322-38a78f8e81f7" />
<img width="1907" height="315" alt="image" src="https://github.com/user-attachments/assets/3daaaeaf-989e-49b3-bd61-e8328e76f304" />
<img width="1517" height="513" alt="image" src="https://github.com/user-attachments/assets/e4f07655-8869-45e2-8717-eb82a2a00b9a" />
<img width="1616" height="687" alt="image" src="https://github.com/user-attachments/assets/bfb94657-3455-4a40-b0ec-7f1c24b86bd6" />
<img width="1675" height="761" alt="image" src="https://github.com/user-attachments/assets/f3c8840b-f1fd-472a-8d3a-689fa6761beb" />
This reconnaissance assessment report synthesizes security findings collected from terminal enumeration activities targeting networkwalks.com and microsoft.com.

Target Infrastructure & DNS Analysis: networkwalks.com

Primary IP Address: 192.232.216.135

Domain Registrar: GoDaddy, LLC (Creation Date: Nov 6, 2019 | Expiry Date: Nov 6, 2027)

Name Servers: NS6135.HOSTGATOR.COM, NS6136.HOSTGATOR.COM

DNS Version Exposure: dnsrecon identified the running DNS server version as BIND 9.16.23-RH.

Mail & Service Configuration: MX record points directly to mail.networkwalks.com (192.232.216.135). Active SPF TXT records and cPanel email auto-discovery SRV records (cpanelemaildiscovery.cpanel.net) were enumerated.

Web Technology & Application Stack

Web Server Architecture: Apache web server operating alongside an Nginx reverse-proxy/caching layer (x-nginx-cache: WordPress).

CMS & Extensions: WordPress CMS (detected version 7.1 meta tag) utilizing WordPress Download Manager v3.3.58.

Frontend Libraries: Bootstrap v7.1, jQuery v3.7.1, Google Tag Manager.

Security & Headers: HTTP/2 200 response returning permissions-policy, referrer-policy, and HttpOnly security flags on session cookies (__wpdm_client). WAF detection scan was executed via wafw00f.

Subdomain Enumeration: microsoft.com

Harvested Subdomains: theHarvester successfully identified 13 unique hosts via the Baidu search engine, including azure.microsoft.com, developer.microsoft.com, hxd.research.microsoft.com, securitycopilot.microsoft.com, and support.serviceshub.microsoft.com.

Tool Configuration Notice: Secondary passive search modules (Censys, BuiltWith, Brave, CriminalIP, Bevigil) failed to execute due to unconfigured API keys in /etc/theHarvester/api-keys.yaml.

Key Recommendations

Hide Server Banners: Obfuscate the BIND DNS version banner (9.16.23-RH) to prevent adversary targeted exploit profiling.

Component Patching: Maintain strict update schedules for WordPress plugins like WordPress Download Manager to mitigate known application vulnerabilities.

API Configuration: Populate API keys within theHarvester configuration file to expand passive intelligence coverage across external attack surfaces.



Maltego Setup & OSINT Reconnaissance Technical Report 🚀
This technical report provides an end-to-end operational walkthrough of installing Maltego Graph Desktop (v4.12.1), setting up authentication credentials, initializing the workspace environment, and conducting Open Source Intelligence (OSINT) recon transforms on specified target entities.

1. Executive Summary 📌
The objective of this procedure was to deploy Maltego Graph Desktop, configure user access via an institutional account, and validate system functionality by running OSINT queries against real-world targets. The deployment succeeded without errors, enabling automated relationship mapping across domain infrastructure and individual digital footprints.

2. Software Installation & System Setup ⚙️
Installation Package: Initiated the installer for Maltego Graph Desktop (v4.12.1) on the Windows workstation environment.

Installer Wizard: Navigated through standard software installation steps, defining application binary paths and registry entries.

Post-Install Configuration: Selected default configurations at the final wizard screen, leaving shortcut generation and Java runtime customization at recommended parameters.

3. Authentication & Data Hub Configuration 🔑
Configuration Launch: Triggered the internal "Configure Maltego" setup wizard upon first application launch.

Browser Authentication Loop: Selected web-based authentication to link the local desktop client with online cloud services.

Credential Input: Successfully authenticated using the student account (mabushov@std.beu.edu.az) through the Maltego ID SSO portal.

License Activation: Activated a desktop license valid through September 19, 2026, enabling full access to core transformation engines.

Data Hub Catalog: Loaded the central Data Hub tab featuring 65 default hub items across critical security categories, including Breaches & Leaks, Infrastructure, Malware, Social Media, and Threat Intelligence (TTPs).

4. Workspace & Entity Palette Initialization 🛠️
Graph Canvas Creation: Generated a primary graph file (New Graph (1)) to visual-map relationships between target entities.

Palette Navigation: Loaded core built-in schemas, including Infrastructure, Personal identifiers, Tracking identifiers, and Cryptocurrency objects (such as Bitcoin/Bitcoin Cash addresses, blocks, and transaction nodes).

5. OSINT Reconnaissance Workflows 🔍
Task A: Domain Infrastructure & Communication Mapping 🌐

Target Entity: networkwalks.com (Domain Entity)

Objective: Identify administrative and operational contact email addresses tied directly to the domain name.

Executed Transform: [Utilities] To Email Addresses [Search Engine]

Execution Timestamp: August 20, 2026 – 11:06 PM

Operational Log: Consumed 10 API credits (190 credits remaining). Query completed in 15.642 seconds.

Discovered Intelligence: Successfully identified and linked the primary email endpoint: info@networkwalks.com.

Task B: Individual Identity & Digital Footprint Reconnaissance 👤

Target Entity: Waqas Karim CCIE (Person Entity)

Objective: Map the public web footprint, associated profiles, and external media references for the targeted identity.

Executed Transform: [Utilities] Search Web [Search Engine]

Execution Timestamp: August 20, 2026 – 11:17 PM

Operational Log: Consumed 32 API credits (160 credits remaining). Query completed in 7.738 seconds.

Discovered Intelligence: Generated a star-topology graph yielding 23 web nodes (www entities) connected across 10 primary link branches, highlighting profiles across public platforms such as LinkedIn and YouTube.

6. Technical Performance Metrics 📊
Environment Platform: Maltego Graph (Desktop) Version 4.12.1

Active Account: mabushov@std.beu.edu.az

License Expiration: September 19, 2026

Total Queries Run: 2 Transform Operations

Total API Credits Consumed: 42 Credits (160 Credits remaining in current period)

Total Extracted Entities: 25 unique graphical nodes (1 Email node, 23 Web page nodes, originating from Domain and Person root nodes)

Graph Structure: Successfully validated node creation, manual transform triggering, log output tracking, and hierarchical layout view.
