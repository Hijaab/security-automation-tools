# Security Automation Toolkit

A Python-based cybersecurity toolkit that includes two core security utilities:

* Password strength analyzer and generator
* Phishing URL detection system

This project demonstrates practical implementations of cybersecurity fundamentals including password security analysis, phishing detection techniques, threat intelligence matching, and URL risk evaluation.

---

## Features

### Password Checker

* Analyzes password strength based on multiple security criteria
* Evaluates:

  * Length validation
  * Uppercase and lowercase character usage
  * Numeric digits
  * Special characters
  * Repeated character patterns
* Generates secure random passwords
* Provides actionable improvement suggestions
* Visual strength scoring system in terminal

---

### Phishing Detection System

* Detects malicious URLs using multiple validation layers:

  * Known phishing domain database
  * Known phishing URL dataset
  * Keyword-based detection rules
  * Domain similarity detection using Levenshtein distance
  * Google Safe Browsing API integration
* Supports bulk URL scanning
* Automatic URL normalization and validation

---

## Security Techniques Used

* Rule-based threat detection
* Pattern matching using regular expressions
* Fuzzy string matching for domain impersonation detection
* Threat intelligence dataset integration
* External security API validation
* Heuristic-based URL risk analysis

---

## Project Structure

```text id="struct001"
security-automation-tools/
│
├── phishing_detection/
│   ├── phishing_detection.py
│   ├── ALL-phishing-domains.txt
│   └── ALL-phishing-links.txt
│
├── password_checker/
│   └── password_checker.py
│
└── README.md
```

---

## Installation

### Clone the repository

```bash id="clone002"
git clone https://github.com/Hijaab/security-automation-tools.git
cd security-automation-tools
```

### Install dependencies

```bash id="install002"
pip install requests python-Levenshtein pyfiglet colorama
```

---

## Usage

### Password Checker

```bash id="run003"
python password_checker/password_checker.py
```

Provides:

* Password strength analysis
* Secure password generation

---

### Phishing Detection Tool

```bash id="run004"
python phishing_detection/phishing_detection.py
```

Supports:

* Single URL scanning
* Bulk URL scanning
* Safe vs phishing classification

---

## Example Output

### Password Strength Output

```text id="ex001"
Password Strength: Strong [███--]
Suggestions:
- Add special characters for improved security
```

---

### Phishing Detection Output

```text id="ex002"
Phishing detected: http://fake-login-paypal.com
Safe URL: https://google.com
```

---

## Security Capabilities

This toolkit demonstrates real-world cybersecurity techniques including:

* Threat intelligence matching
* Domain impersonation detection
* URL reputation analysis
* Password entropy evaluation
* Pattern-based threat detection

---

## Important Security Note

The Google Safe Browsing API key should not be hardcoded in production environments. It should be stored securely using environment variables.

Example:

```bash id="env002"
export API_KEY="your_api_key_here"
```

---

## Future Improvements

* Web-based dashboard for unified interface
* Machine learning-based phishing classification
* Real-time threat intelligence integration
* REST API using FastAPI
* Dockerized deployment
* Browser extension for live URL protection

---

## Learning Outcomes

This project demonstrates skills in:

* Cybersecurity fundamentals
* Secure coding practices
* Threat detection methodologies
* Python automation
* API integration
* CLI tool development

---

## Author

Hijaab Sikander

Cybersecurity | DevSecOps | AI Security Engineer

GitHub: https://github.com/Hijaab
LinkedIn: https://linkedin.com/in/hijaabsikander
