# Course Evaluation Score Extractor

A browser-based tool for UVM faculty to extract and compare mean scores from Blue course evaluation PDF reports. No installation or server required — everything runs locally in your browser.

---

## How to Use

### 1. Select Your Course Type

Before uploading any files, choose the course type that matches your evaluation PDFs:

- **Sole Instructor / Course Coordinator** — for courses with 21 instructor questions
- **Co-Instructor** — for courses with 12 instructor questions

> The course type selector locks once files are loaded. Click **Clear All** to switch types.

### 2. Upload PDF Files

Drag and drop one or more Blue evaluation PDF files onto the upload zone, or click **Choose PDF files** to browse. You can upload multiple PDFs to compare courses side by side.

Each file is processed immediately. A checkmark indicates success; an exclamation mark indicates an error (e.g., wrong course type or unreadable file). Valid files are displayed even if some files fail.

### 3. Read the Results Table

- Each **column** represents one course, labeled with the course code and instructor name extracted from the filename.
- Each **row** represents one evaluation question, showing the mean score per course.
- The bottom rows show:
  - **Survey Completion** — number of responses out of total enrollment and the completion rate
  - **Teaching Effectiveness Score** — average of key teaching questions (see below)

### 4. Toggle Question Rows

Click **Hide Original Question Scores** to collapse the individual question rows and show only the summary rows. Click **Show Original Question Scores** to expand them again.

### 5. Remove Files

Click the **×** next to any file in the file list to remove it. The table updates immediately to reflect the remaining files.

### 6. Clear and Start Over

Click **Clear All** to remove all files and reset the tool, including unlocking the course type selector.

---

## Score Color Legend

| Color | Range | Meaning |
|-------|-------|---------|
| Green | 4.25 – 5.00 | Excellent |
| Blue  | 3.50 – 4.25 | Good |
| Red   | below 3.50  | Needs attention |

---

## Teaching Effectiveness Score

This is a composite score calculated as the average of key teaching questions:

- **Sole Instructor / Course Coordinator:** average of Q1, Q4, Q7, Q10, Q16, Q19
- **Co-Instructor:** average of Q1, Q3, Q6, Q7, Q10, Q11

---

## File Naming Convention

The tool extracts the course name and instructor name automatically from the PDF filename. For best results, ensure your Blue export filenames follow this format:

```
Any text (COURSE CODE) FirstName LastName ...
```

Example: `Fall 2024 (KINE 2250) Jane Doe_Section1.pdf` → displays as **KINE 2250 — Jane Doe**

---

## Notes

- All processing happens in your browser. No data is uploaded to any server.
- Only Blue-format course evaluation PDFs from UVM are supported.
- If a file shows an error, check that the correct course type is selected before uploading.
