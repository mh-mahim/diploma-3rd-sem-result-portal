# Changelog

## [1.1.0] - 2026-11-10
### Fixed
- **Refer Subject Separation**: Separated 3rd semester subjects (`25922`, `25931`, `26731`, `26831`, `26832`, `28511`) from 1st and 2nd semester accumulated backlogs (`25911`, `25912`, `25913`, `25921`, `26721`, `26811`, `26821`).
- **Refer Count Accuracy**:
  - 2 subjects referred in 3rd Sem: Exactly 3 students (`214126`, `214131`, `214172`).
  - 3 subjects referred in 3rd Sem: Exactly 2 students (`214084`, `214110`).
  - 4 subjects referred in 3rd Sem (Drop Out): Exactly 1 student (`214083`).
  - Total Drop Out (>= 4 subjects in 3rd Sem): Exactly 4 students (`214083`, `214101`, `214167`, `214170`).
- **False Drop Out Corrections**: Fixed Rolls `214126`, `214172`, `214110` who were previously misclassified as Drop Out due to backlog aggregation.

### Added
- **Dynamic Sorting System**:
  - Sort by Roll Number (Ascending / Descending)
  - Sort by GPA (Highest to Lowest / Lowest to Highest)
  - Sort by 3rd Sem Referred Subject Count (Fewest to Most / Most to Fewest)
  - Sort by Status (Passed first / Drop Out first)
- **Dual Display Modes**:
  - Detailed Card Grid View
  - Full BTEB Sheet Table View (with 1st, 2nd, 3rd semester columns)
- **Scope Selector**: Switch between 3rd Semester appeared (33 students) and Full Class batch (79 students).
- **Local Server Execution**: Local server daemon running on port 3000.
