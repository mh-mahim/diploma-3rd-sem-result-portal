# Active Task: Diploma 3rd Semester Result Portal - Data Correction, Sorting & Local Server

## Status
- **Current Phase**: Local Execution & Verified
- **Active Task**: Local Server Running at http://localhost:3000

## Live Checklist
- [x] Investigate discrepancy in refer subjects and refer counts:
  - Identified that previously 1st and 2nd semester backlogs (e.g., Math-I, Physics-I, Chemistry, Circuits-I) were erroneously aggregated into 3rd semester referred subject counts.
  - Corrected originSemester mapping across all 20 syllabus subjects (Regulation 2022).
  - Explicitly isolated 3rd semester subjects (`25922`, `25931`, `26731`, `26831`, `26832`, `28511`).
- [x] Recalculate true 3rd semester statistics:
  - Total 3rd Semester Appeared: 33 students
  - Passed: 17 students
  - 1 Subject Referred: 7 students (Rolls: 214087, 214091, 214109, 214118, 214124, 214129, 214132)
  - 2 Subjects Referred: 3 students (Rolls: 214126, 214131, 214172)
  - 3 Subjects Referred: 2 students (Rolls: 214084, 214110)
  - 4 Subjects Referred (Drop Out): 1 student (Roll: 214083)
  - Total Drop Out (>= 4 subjects in 3rd Sem): 4 students (Rolls: 214083, 214101, 214167, 214170)
  - Prior semester backlogs displayed separately without corrupting 3rd semester counts.
- [x] Implement multi-attribute sorting system:
  - Sort by Roll Number (Ascending / Descending)
  - Sort by GPA (Highest to Lowest / Lowest to Highest)
  - Sort by 3rd Sem Referred Subjects Count (Low to High / High to Low)
  - Sort by Status (Passed first / Drop Out first)
- [x] Dual Display Modes:
  - Responsive Card Grid View
  - Full BTEB Sheet Table View (displaying Sem 1, Sem 2, Sem 3 alongside 3rd sem subjects and prior backlogs)
  - Scope Toggle: "৩য় সেমিস্টার পরীক্ষার্থী (৩৩)" vs "পুরো ব্যাচের শিক্ষার্থী (৭৯)"
- [x] Start local server daemon on `http://localhost:3000` (serving directly without GitHub sync as requested).

## Blockers
- None. Server is actively listening on port 3000.
