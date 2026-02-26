SRS → QA Test Case Automation (n8n + OpenAI)

 Overview
This project automates the generation of structured QA test cases from a Software Requirements Document (SRD/SRS) using n8n and OpenAI.

Instead of manually writing test cases, the workflow:
1. Reads an SRS (PDF)
2. Extracts requirement content
3. Uses Openrouter and OpenAI to generate structured test cases
4. Parses and validates JSON output
5. Exports formatted test cases to Excel (.xlsx)

---

 Architecture

SRS (PDF)  
→ Text Extraction  
→ openrouter based,OpenAI (Structured Test Case Generation)  
→ JSON Parsing (Code Node) and flattening
→ Excel export to sheets

---

 Tech Stack

- n8n (Self-hosted via Node)
- OpenAI API
- Openrouter
- Google cloud
- Google drive
- Google sheets
- Excel (.xlsx) export
- GitHub for version control

---

Current Capabilities

- node based n8n setup with persistent volume
- PDF ingestion from local file system
- AI-powered structured test case generation
- JSON validation and parsing
- Automated Excel export to sheets
- Incremental Git commits tracking project evolution

 Example Files

- `srs-sample 1.pdf` → Sample input SRD
- `generated_test_cases.xlsx` → Sample AI-generated test cases
- `Test Agent.json` → n8n workflow export


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
