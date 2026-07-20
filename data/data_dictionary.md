# Data Dictionary: Hospital Patient Outcomes Dataset

This document provides a detailed description of each column in the `patient_data.csv` dataset, which is used for the Hospital Patient Outcomes Dashboard project.

| Column Name      | Data Type | Description                                                               | Possible Values / Format                                  |
| :--------------- | :-------- | :------------------------------------------------------------------------ | :-------------------------------------------------------- |
| `Patient_ID`     | Text      | Unique identifier assigned to each patient.                               | `PAT001`, `PAT002`, etc.                                  |
| `Admission_Date` | Date      | The date when the patient was admitted to the hospital.                   | `YYYY-MM-DD` (e.g., `2025-01-15`)                         |
| `Discharge_Date` | Date      | The date when the patient was discharged from the hospital.               | `YYYY-MM-DD` (e.g., `2025-01-20`)                         |
| `Age`            | Integer   | The age of the patient in years at the time of admission.                 | `1` to `90`                                               |
| `Gender`         | Text      | The self-reported gender of the patient.                                  | `Male`, `Female`, `Other`                                 |
| `Department`     | Text      | The hospital department where the patient was primarily admitted.         | `Cardiology`, `Emergency`, `General Medicine`, `Orthopedics`, `Pediatrics`, `Surgery` |
| `Diagnosis`      | Text      | The primary medical diagnosis for which the patient was admitted.         | e.g., `Heart Failure`, `Fracture`, `Pneumonia`            |
| `Admission_Type` | Text      | The category describing how the patient was admitted to the hospital.     | `Emergency`, `Elective`, `Urgent`                         |
| `Length_of_Stay` | Integer   | The total number of days the patient stayed in the hospital.              | Calculated from `Discharge_Date` - `Admission_Date`       |
| `Outcome`        | Text      | The patient's condition or status upon discharge.                         | `Recovered`, `Improved`, `Referred`, `Unknown`            |
| `Readmission`    | Text      | Indicates whether the patient was readmitted to the hospital within 30 days of discharge. | `Yes`, `No`                                               |
