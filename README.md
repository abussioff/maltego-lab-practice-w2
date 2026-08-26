# maltego-lab-practice-w2
<img width="621" height="482" alt="image" src="https://github.com/user-attachments/assets/c6f25fb9-712d-4418-875e-301c6f00c039" />
<img width="1720" height="879" alt="image" src="https://github.com/user-attachments/assets/84249d6c-d972-4279-b2eb-625c5aef19d9" />
<img width="1887" height="904" alt="image" src="https://github.com/user-attachments/assets/4add95ec-896f-42b8-9f16-9b8ce7e97388" />
<img width="1716" height="893" alt="image" src="https://github.com/user-attachments/assets/16c65217-0fe7-44fa-a455-8169ba4e8be3" />
<img width="1722" height="897" alt="image" src="https://github.com/user-attachments/assets/9a66a2b8-ab61-4b63-afae-64c6edc04126" />
<img width="1709" height="899" alt="image" src="https://github.com/user-attachments/assets/d76e0802-6372-4a71-af7f-6fda18a9cef2" />
<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/d6678adb-b547-4839-9186-e432f9b51ffb" />

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
