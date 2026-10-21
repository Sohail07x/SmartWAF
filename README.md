# SmartWAF — Machine Learning-Based Web Application Firewall Prototype

SmartWAF is a learning and demonstration project that explores how machine learning can help classify potentially suspicious web requests. It combines a Python/Flask web application with a Random Forest classifier built using scikit-learn.

> **Project status:** Tested prototype for learning and demonstration. It is not a production-ready web application firewall, and its detection performance and security have not been independently validated.

## Project goals

- Explore a machine-learning approach to classifying web requests.
- Demonstrate how request features can be passed to a trained classifier.
- Connect a Python backend, a model, and a simple web interface.
- Learn about web-security patterns such as SQL injection and cross-site scripting (XSS).

## Technologies

- **Python** — application logic
- **Flask** — web application/backend
- **scikit-learn** — machine-learning workflow
- **Random Forest** — classification model
- **HTML and CSS** — user interface
- **Git and GitHub** — version control and project hosting

## How it works

1. A request or sample input is submitted to the application.
2. The application derives a set of manually designed features from the input.
3. The trained Random Forest model classifies the feature representation.
4. The prototype displays or records the resulting classification as part of its demonstration workflow.

The project explores patterns associated with SQL injection and XSS. These classifications should be treated as experimental signals, not as proof that a request is safe or malicious.

## Features explored

- Feature-based classification of web-request inputs
- A Flask-based backend
- A simple web interface/dashboard
- Demonstration of allow/block decisions for classified requests
- A small labelled sample dataset for experimentation

## Repository contents

The repository includes the project materials and a `smartwaf.zip` archive. Extract the archive to inspect the application files before running the project.

## Running the project

The application files are provided in the `smartwaf.zip` archive. Because the exact Python environment and dependencies may vary, inspect the extracted files for the dependency list and application entry point before running it. Use an isolated Python virtual environment and install only the dependencies required by the project.

Do not expose the prototype to the public internet or use it as the only security control for a real application.

## Limitations and responsible use

- The project uses a small dataset and manually designed features; results may not generalize to real-world traffic.
- Model accuracy, false-positive rate, and false-negative rate have not been independently benchmarked.
- The prototype has not been validated as a production reverse proxy or as a complete security layer.
- A request classified as benign may still be malicious, and a suspicious classification may be a false positive.
- This project is for educational experimentation. Use established security controls, testing, and expert review for real systems.

## Learning outcomes

This project provided hands-on exploration of connecting a machine-learning classifier to a web application, designing request features, using Flask, and considering the limitations of ML-based security detection.

## Author's contribution

The implementation was developed through a combination of personal coding, AI-assisted development, tutorials, and existing learning resources. The project is presented as a learning prototype, with its scope and limitations stated explicitly.

## Future improvements

- Add reproducible installation and run instructions after validating the environment.
- Build a larger, more representative labelled dataset.
- Evaluate precision, recall, false positives, and false negatives on held-out data.
- Add tests, input validation, and clearer logging.
- Document the threat model and compare the approach with established security tools.

---

**Disclaimer:** SmartWAF is an educational prototype, not a substitute for a professionally configured Web Application Firewall (WAF), secure coding practices, or security testing.