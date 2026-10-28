# Projects

## Cloud Active Directory and SOC Lab (Azure, Windows Server 2022)

I set up Azure virtual machines, virtual networks and resource groups. I promoted a server to Domain Controller with Active Directory, DNS, Kerberos and Group Policy.

I joined a client machine to the domain and checked that logins and DNS worked. I created 5 test user accounts in a custom Organizational Unit, with Domain Users and Remote Desktop Users group memberships, to copy a real company's access setup.

I fixed DNS problems, domain join failures and password policy errors. I read the Windows Security Event Logs on the Domain Controller to confirm user creation, password resets and logins.

## Tool Hire Shop Management System (Java)

I built a Java system for a tool hire shop using object-oriented design, with a multi-level class structure for tools, accessories and workwear.

It handles reservations and customers, including checks for availability across several days, prevention of double bookings, unique ID generation and saving data to files. I used structured exception handling and a dedicated test class throughout development.

The code is on GitHub: https://github.com/Mi-mi-zi/ToolItemReservation

## Week 1 Project: Ground Truth News Classification Evaluation
 I manually labelled 30 news headlines across World, Sports, Business and Sci/Tech categories, then evaluated AI-generated classifications against benchmark labels using agreement rates, Cohen's Kappa, confusion matrices and model evaluation techniques. I also compared prompt-engineered AI classification against a TF-IDF machine learning model and investigated the impact of data leakage on model performance.

Results:
Labelled 30 news articles
Achieved 83.3% agreement (25/30) between AI classifications and benchmark labels
Achieved Cohen's Kappa score of 0.777
Identified Business and Sci/Tech as the most commonly confused categories
Evaluated a TF-IDF model with 86.5% held-out accuracy on a larger dataset

## Week 2 project: Newsroom Triage app

Built a Python-based news classification application using FastAPI, Gradio, and Neon Postgres. The application classifies headlines into four categories, stores results in a database, provides confidence scores, exposes API endpoints, and evaluates performance against previously labelled data. The system was split into separate frontend and backend services communicating over HTTP.

Results:
Built 4 API endpoints: /classify, /runs, /score and /health
Migrated application data from SQLite to Neon Postgres
Evaluated the system against 30 labelled headlines
Baseline performance: 7/30 correct predictions, 23.3% accuracy, 0.1825 Cohen's Kappa
Discovered and fixed a scoring bug where invalid predictions were incorrectly excluded from Kappa calculations
