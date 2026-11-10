# Requirements Specification

## Functional Requirements
1. **Scope Filtering**: Filter only students who have 3rd Semester results out of the 79 total fetched student rolls (exactly 33 students).
2. **Class Overview KPIs**:
   - Total Students with 3rd Semester result (33).
   - Passed Count (17) & Average GPA.
   - Referred Count for 2 Subjects (2 students).
   - Referred Count for 3 Subjects (1 student).
   - Referred Count for 4 Subjects (3 students).
   - Total Drop Out Count (students with >= 4 referred subjects = 11 students).
3. **Student Result Cards**:
   - Display Roll number prominently.
   - Display Status: Passed (with GPA in green) or Referred (with failed count in amber/red).
   - If failed subjects >= 4, clearly display **"⚠️ Drop Out"** status badge.
   - List failed subject codes and full subject names.
4. **Search & Filter**:
   - Real-time roll number search.
   - Filter chips: All, Passed, 2 Subjects Referred, 3 Subjects Referred, 4 Subjects Referred, Drop Out.
5. **Student Detail Modal**:
   - View complete historical academic record across 1st, 2nd, and 3rd semesters.
6. **Print View**:
   - Clean printer-friendly stylesheet for printing or saving to PDF.

## Non-Functional Requirements
1. Zero server dependency (client-side bundled data for instant 0ms load).
2. Works offline once loaded.
3. Mobile-first responsive layout (smartphones, tablets, desktop).
