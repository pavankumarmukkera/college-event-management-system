# College Event Management - Proposed Dataverse Schema

## Table: CollegeEvents

| Column | Type |
|---|---|
| EventName | Text |
| EventDate | Date |
| Venue | Text |
| Capacity | Whole Number |
| Organiser | Text |

## Table: EventRegistrations

| Column | Type |
|---|---|
| StudentName | Text |
| StudentEmail | Email/Text |
| Event | Lookup to CollegeEvents |
| RegistrationDate | Date |
| AttendanceStatus | Choice |

## Implementation Status
Proposed schema only.
No Dataverse tables have been deployed.
