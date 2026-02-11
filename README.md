SRD → QA Test Case Automation (n8n + OpenAI)

 Overview
This project automates the generation of structured QA test cases from a Software Requirements Document (SRD/SRS) using n8n and OpenAI.

Instead of manually writing test cases, the workflow:
1. Reads an SRD (PDF)
2. Extracts requirement content
3. Uses OpenAI to generate structured test cases
4. Parses and validates JSON output
5. Exports formatted test cases to Excel (.xlsx)

---

 Architecture

SRD (PDF)  
→ Text Extraction  
→ OpenAI (Structured Test Case Generation)  
→ JSON Parsing (Code Node)  
→ Excel Export  

---

## 🛠 Tech Stack

- n8n (Self-hosted via Docker)
- Docker (Containerized local deployment with volume mounting)
- OpenAI API
- Excel (.xlsx) export
- GitHub for version control

---

Current Capabilities

- Dockerized n8n setup with persistent volume
- PDF ingestion from local file system
- AI-powered structured test case generation
- JSON validation and parsing
- Automated Excel export
- Incremental Git commits tracking project evolution

 Example Files

- `library_srs.pdf` → Sample input SRD
- `generated_test_cases.xlsx` → Sample AI-generated test cases
- `srd_to_testcases.json` → n8n workflow export


 Future Improvements

- Requirement chunking for better coverage
- Duplicate test case detection
- Traceability matrix generation
- Google Sheets integration
- Jira/TestRail integration
- Priority auto-assignment logic

---

 Philosophy

Built incrementally.  
Done > Perfect.  
Focused on automation architecture rather than prompt-only solutions.
