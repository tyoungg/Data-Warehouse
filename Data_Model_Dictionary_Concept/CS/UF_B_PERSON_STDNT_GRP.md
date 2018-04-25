# UF_B_PERSON_STDNT_GRP

UF_B_PERSON_STDNT_GRP maintains the effective starting date and effective end date of a person's student group and includes the history of the student groups. This is a bridge table to be joined between the fact table by PERSON_SID and the UF_D_STDNT_GROUP dimension. Student groups back to the person for tagging.					
					
					
| Column Name     | Data Type | Data Length | Precision | Description                                 | 
|-----------------|-----------|-------------|-----------|---------------------------------------------| 
| PERSON_SID      | NUMBER    | 10          | 0         | Person surrogate identification             | 
| STDNT_GROUP_SID | NUMBER    | 10          | 0         | Student Group surrogate identification      | 
| INSTITUTION_SID | NUMBER    | 10          | 0         | Institution surrogate identification        | 
| EFFDT_SID       | NUMBER    | 10          | 0         | Effect start date surrogate identification  | 
| END_EFFDT_SID   | NUMBER    | 10          | 0         | Effective end date surrogate identification | 
| EFF_STATUS      | VARCHAR2  | 1           |           | Effective Status (A- Active, I- Inactive)   | 