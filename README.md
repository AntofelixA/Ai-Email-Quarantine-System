🤖 AI Email Quarantine System    
An AI-powered Email Quarantine System designed to automatically analyze incoming emails, detect potential threats such as spam and phishing, and quarantine suspicious messages before they reach the inbox. This project adds an intelligent security layer to traditional email filtering systems.

📌 Project Overview    
Email remains one of the most common attack vectors for phishing, spam, and malware delivery. Traditional rule-based filters are often insufficient against evolving threats.    
The AI Email Quarantine System uses machine learning and heuristic analysis to:    
    •	Analyze email content        
    •	Detect malicious or suspicious patterns        
    •	Automatically quarantine risky emails        
    •	Reduce false positives        
    •	Improve overall email security        

✨ Key Features    
•	📧 Automatic Email Fetching    
    o	Connects to an email server using IMAP/POP3    
    o	Monitors incoming and unread emails    
•	🤖 AI-Based Email Analysis    
    o	Uses NLP and ML techniques to analyze email content    
    o	Detects spam, phishing, and suspicious behavior    
    o	Assigns a risk score to each email    
•	🚫 Email Quarantine    
    o	Suspicious emails are moved to a quarantine folder    
    o	Prevents malicious emails from reaching the inbox    
•	📊 Logging & Reporting    
    o	Logs email actions (safe / quarantined)    
    o	Displays analysis results for review    
•	⚙️ Configurable & Extendable    
    o	Easy to adjust thresholds and rules    
    o	Can be enhanced with additional AI models or APIs    

🏗️ System Architecture    
1.	Email Fetcher    
    o	Connects to the mail server    
    o	Retrieves incoming emails    
2.	AI Threat Analyzer    
    o	Scans email content, subject, sender, and links    
    o	Uses machine learning / heuristic logic    
3.	Decision Engine    
    o	Determines if an email is safe or suspicious    
4.	Quarantine Manager    
    o	Moves suspicious emails to quarantine    
    o	Logs the action    
5.	Monitoring & Logs    
    o	Maintains records of scanned and quarantined emails    

🛠️ Technologies Used    
•	Programming Language: Python    
•	Frontend: HTML, CSS
•	Framework: Flask
•	Database: MySQL
•	Email Protocols: IMAP 
•	Email Auth: SPF / DKIM validation
•	AI / ML: Machine Learning Model, TF-IDF(vectorization), Logistic Regression
•	Libraries:    
    o	flask
    o	imaplib    
    o	email    
    o	scikit-learn    
    o	logging    

📂 Project Structure
```text
AI-Email-Quarantine-System/
│
├── app/
│   ├── api/
│   │   ├── __init__.py
│   │   ├── auth.py
│   │   ├── dashboard.py
│   │   ├── email.py
│   │   ├── scanner.py
│   │   └── ...
│   │
│   ├── core/
│   │   ├── config.py
│   │   ├── security.py
│   │   └── ...
│   │
│   ├── database/
│   │   ├── db.py
│   │   ├── models.py
│   │   └── ...
│   │
│   ├── middleware/
│   │   └── ...
│   │
│   ├── ml/
│   │   ├── feature_engineering.py
│   │   ├── model.py
│   │   ├── predictor.py
│   │   └── ...
│   │
│   ├── services/
│   │   ├── email_service.py
│   │   ├── quarantine_service.py
│   │   └── ...
│   │
│   ├── static/
│   │   ├── css/
│   │   ├── js/
│   │   └── images/
│   │
│   ├── templates/
│   │   ├── dashboard.html
│   │   ├── login.html
│   │   └── ...
│   │
│   └── utils/
│       ├── __pycache__/
│       ├── helpers.py
│       ├── logger.py
│       └── __init__.py
│
├── config.py
├── run.py
│
├── ml_training/
│   └── Dataset(SpamAssasin-edited)...
│
├── scripts/
│   └── run_email_scan.py
│
├── .env.example
├── LICENSE
├── app.py
├── requirements.txt
├── test_env.py
└── README.md
``` 

🚀 How It Works    
1.	Connects to the email server    
2.	Fetches new/unread emails    
3.	Analyzes each email using AI models    
4.	Assigns a risk score    
5.	Quarantines emails above the risk threshold    
6.	Logs actions and results    

⚠️ Security Considerations    
•	Always use app-specific passwords for email access    
•	Do not expose credentials in source code    
•	Review the code before deploying in production    
•	Use only on email accounts you own or have permission to access    

🧪 Use Cases    
•	Spam and phishing detection    
•	Educational MCA (AI / cybersecurity)project        
•	Email security research    
•	Automated email filtering systems    

🔮 Future Enhancements        
•	Deep learning-based threat detection    
•	Integration with VirusTotal / external threat APIs        
•	Real-time alerts and notifications        
•	Multi-mailbox support    

   Screenshots

<p align="center">
  <img width="1005" height="464" alt="Homepage image" src="https://github.com/user-attachments/assets/2f06cb38-b6aa-4578-ad9f-bd5262cd3765" />
</p>

<p align="center">
  <b>Fig-1: Home Page of AI-Email Quarantine System </b>
</p>

<p align="center">
  <img width="1004" height="474" alt="Dashboard image" src="https://github.com/user-attachments/assets/ebbd5ec6-c5f4-48a4-8d09-e5ac442ad764" />
</p>

<p align="center">
  <b>Fig-2: SOC-style dashboard Page of AI-Email Quarantine System </b>
</p>

<p align="center">
  <img width="1005" height="480" alt="image" src="https://github.com/user-attachments/assets/9d681887-7318-4142-adf7-a5d743b0edb6" />
</p>

<p align="center">
  <b>Fig-3: User Interface Displaying Legitimate (Safe) Emails with ML-Based Risk Scores </b>
</p>

<p align="center">
  <img width="1005" height="483" alt="image" src="https://github.com/user-attachments/assets/bb0e0803-f43b-4787-820d-1c1d5f8ceec7" />
</p>

<p align="center">
  <b>Fig-4: Detailed View of a Safe Email with ML-Based Risk Score  </b>
</p>

<p align="center">
  <img width="692" height="976" alt="image" src="https://github.com/user-attachments/assets/17a55b58-b399-4d1c-b950-a30f36d5e17e" />
</p>

<p align="center">
  <b>Fig-5: Email Scan Report Generated in PDF Format  </b>
</p>

<p align="center">
  <img width="763" height="982" alt="image" src="https://github.com/user-attachments/assets/64d5daa5-6ade-4bae-aca9-9c7ebb29f193" />
</p>

<p align="center">
  <b>Fig-6: Email Scan Report Generated in DOCX Format  </b>
</p>

<p align="center">
  <img width="812" height="1022" alt="image" src="https://github.com/user-attachments/assets/f0e5e1ba-9f28-4fc8-a073-b20e8f8ec4f1" />
</p>

<p align="center">
  <b>Fig-7: Email Scan Report Generated in TXT Format  </b>
</p>

👤 Author    
Anto Felix A
GitHub: https://github.com/AntofelixA
LinkedIn: https://www.linkedin.com/in/anto-felix/

📜 License    
This project is open-source and intended for educational and research purposes.    
