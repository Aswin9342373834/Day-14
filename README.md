# Day 14 — AI Job Red Flag Detector

## Overview
This task uses Claude as an AI Red Flag Detector to analyze a real job posting and its parent company, surfacing risks a typical job seeker might miss — unrealistic requirements, toxic workplace signals, fake/misleading remote claims, hiring risks, and company-level red flags.

## Job Analyzed
**Role:** Software Developer Intern
**Company:** BHAYAT NGO
**Location:** Remote (India)
**Stipend:** ₹60,000/year (₹5,000/month)
**Source:** Carried over from the Day 13 Job Discovery & Analysis Report (Indeed connector search results)

## Process
1. Used the Day 13 Job Discovery Report as the source job description, since a separate full JD/company info wasn't available.
2. Ran a web search to pull the full job posting text (via Glassdoor/Indeed listings) and independently verify BHAYAT NGO's actual organizational background.
3. Fed both the job posting details and verified company information into the Job Red Flag Detector prompt.
4. Generated a full risk analysis report: overall risk score, red flags with severity ratings, positive signals, risk breakdown table, final verdict, and 5 targeted interview questions.
5. Visualized the risk breakdown as a horizontal bar chart for quick reference.
6. Exported the full analysis as a formatted Word document.

## Key Result
**Overall Risk Score: 68/100 — Elevated Risk**
**Final Verdict: ⚠️ Apply with Caution**

The standout finding wasn't a buzzword (no "rockstar" or "hustle" language appeared anywhere) — it was a **structural mismatch**: BHAYAT NGO's verified public mission is literacy, handicraft training, and community welfare, with no documented technology division, yet it is advertising an enterprise-grade software role (Agile delivery, cloud deployment, RBAC, security best practices). That mismatch between stated organizational identity and job scope was the single biggest red flag — and it's the kind of signal a simple keyword scanner would never catch.

## Key Learnings
- Keyword-based red flag detection (scanning for "fast-paced," "rockstar," etc.) is insufficient on its own — this listing was clean of buzzwords but still high-risk.
- Cross-referencing a job posting against the hiring organization's own stated mission and public history is one of the most effective ways to catch quietly risky listings.
- A disclosed salary and individually-reasonable skill requirements don't guarantee a safe listing — hiring risk and company risk can still be elevated even when culture signals look fine.
- Independent verification of company information (beyond the job board itself) was essential and should be a standard step before applying anywhere unfamiliar.

## Files in This Folder
| File | Description |
|---|---|
| `Day14_Job_Red_Flag_Report.docx` | Full Word report: risk score, red flags, positive signals, risk breakdown, verdict, interview questions |
| `README.md` | This file — task summary and key learnings |
| Screenshots | Screenshots of the generated report and risk breakdown chart (added during upload) |

## Tools Used
- Claude (effort level: Low)
- Web search (for job posting verification and company background research)
- Claude's Visualizer (risk breakdown bar chart)
- Claude's document-creation skill (Word report generation)
