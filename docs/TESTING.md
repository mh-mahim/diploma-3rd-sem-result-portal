# Testing Strategy & Verification Checklist

## Test Cases

### 1. Data Integrity Test
- [x] Exactly 33 students with semester 3 results are identified.
- [x] Passed count equals 17 students.
- [x] Referred count equals 16 students.
- [x] Exactly 2 students with 2 subjects referred (214124, 214129).
- [x] Exactly 1 student with 3 subjects referred (214087).
- [x] Exactly 3 students with 4 subjects referred (214110, 214126, 214172).
- [x] Exactly 11 students with >= 4 subjects referred flagged as Drop Out.

### 2. Functional & UI Verification
- [ ] Roll search filters cards instantaneously with zero lag.
- [ ] Clicking filter chips shows exact subsets.
- [ ] Modal correctly displays previous semesters (1st and 2nd).
- [ ] Responsive test across iPhone (390px), Tablet (768px), and Desktop (1280px).
