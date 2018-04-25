#UF_B_STDNT_TERM

**Description:**
UF_B_STDNT_TERM is a bridge table for the student's academic career enrollment terms. This only provides the term enrollment information bridge to the UF_D_TERM table based on the Academic Career program status of ACTIVE.  Join from fact to bridge based on PERSON_SID and where TERM_CD between the Effective Term and End Effective Term on the fact. Can bridge outwards to UF_D_TERM for term information based on TERM_SID. Additional attributes are on the bridge for information relative to the enrollment career term.					

| Column Name        | Data Type    | Data Length | Precision | Description                                                                                                                          | 
|--------------------|--------------|-------------|-----------|--------------------------------------------------------------------------------------------------------------------------------------| 
| PERSON_SID         | NUMBER       | 10          | 0         | Person surrogate identification                                                                                                      | 
| ACAD_CAR_SID       | NUMBER       | 10          | 0         | Academic Career surrogate identification                                                                                             | 
| INSTITUTION_SID    | NUMBER       | 10          | 0         | Institution surrogate identification                                                                                                 | 
| STDNT_CAR_NBR      | NUMBER       |             | 0         | Student Career Number - Generated for multiple programs in the same academic career                                                  | 
| TERM_SID           | NUMBER       | 10          | 0         | Term surrogate identification                                                                                                        | 
| STRM               | VARCHAR2     | 4           |           | PeopleSoft Term Value                                                                                                                | 
| TERM_BEG_DT_SID    | NUMBER       | 10          | 0         | Term begin date surrogate identification                                                                                             | 
| TERM_END_DT_SID    | NUMBER       | 10          | 0         | Term end date surrogate identification                                                                                               | 
| EMPLID             | VARCHAR2     | 11          |           | PeopleSoft Employee ID -  populated with UFID values                                                                                 | 
| DATE_OF_BIRTH      | DATE         | 7           |           | Date of birth for the person                                                                                                         | 
| INSTITUTION        | VARCHAR2     | 5           |           | Institution Value - Currently all values contain UFLOR for University of Florida                                                     | 
| ACAD_CAREER        | VARCHAR2     | 4           |           | Academic Career - designates all course work undertaken by a student at an academic institution                                      | 
| AGE_YEARS          | NUMBER       | 10          | 0         | Age in Years of the person for the term                                                                                              | 
| AGE_MONTHS         | NUMBER       | 10          | 0         | Age in Months of the person for the term                                                                                             | 
| AGE_DAYS           | NUMBER       | 10          | 0         | Age in Days  of the person for the term                                                                                              | 
| TOT_CUMULATIVE     | NUMBER       | 8           | 3         | Student's total cumulative units for the term                                                                                        | 
| JUNIOR_SENIOR_FLAG | VARCHAR2     | 1           |           | Flag (Y/N) indicating if Student is a Junior or Senior                                                                               | 
| TOT_TAKEN_PRGRSS   | NUMBER       | 22          | 8         | Total Taken for Progress                                                                                                             | 
| TOT_TRNSFR         | NUMBER       | 22          | 8         | Total Transferred                                                                                                                    | 
| TOT_TEST_CREDIT    | NUMBER       | 22          | 8         | Total From Test Credit                                                                                                               | 
| TOT_OTHER          | NUMBER       | 22          | 8         | Total from Other Credit                                                                                                              | 
| TOT_PASSD_PRGRSS   | NUMBER       | 22          | 8         | Total Passed for Progress                                                                                                            | 
| UNT_TAKEN_PRGRSS   | NUMBER       | 22          | 8         | Units Taken for Progress                                                                                                             | 
| CUR_GPA            | NUMBER       | 22          | 8         | Current GPA for the term activity                                                                                                    | 
| CUM_GPA            | NUMBER       | 22          | 8         | Cumulative GPA  for all activity up to the term                                                                                      | 
| ENRL_CNT           | NUMBER       | 22          |           | Enrolled sections (classes) for the term                                                                                             | 
| ENRL_FLG           | VARCHAR2     | 1           |           | Enrollment/Registered Flag for the term                                                                                              | 
| SSR_TRMAC_LAST_DT  | DATE         | 7           |           | Max Academic Program Effective Date for the Term                                                                                     | 
| ACAD_LEVEL_BOT     | VARCHAR2     | 3           |           | Beginning of Term Academic Level Code                                                                                                | 
| ACAD_LEVEL_EOT     | VARCHAR2     | 3           |           | End of Term Academic Level Code                                                                                                      | 
| UF_CLASS           | VARCHAR2     | 1           |           | UF student classification level (0-9)                                                                                                | 
| RESIDENCY          | VARCHAR2     | 5           |           | Residency Code                                                                                                                       | 
| LASTUPD_EW_DTTM    | TIMESTAMP(6) | 11          | 6         | Last updated timestamp - Warehousing column and indicates when the row was last updated from a transaction commit time on the source | 
	
					