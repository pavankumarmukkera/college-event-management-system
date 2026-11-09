# College Event Management - Power Apps

## Overview
Proposed Canvas App for managing college events,
registrations and attendance.

## Planned Screens
- Events Dashboard
- Event Registration
- My Registrations
- Attendance Management

## Example Power Fx

### Display Upcoming Events

```powerfx
Filter(
    CollegeEvents,
    EventDate >= Today()
)
```

### Submit Registration

```powerfx
Patch(
    EventRegistrations,
    Defaults(EventRegistrations),
    {
        Title: txtStudentName.Text,
        StudentEmail: txtStudentEmail.Text,
        EventID: varSelectedEvent.ID
    }
)
```

## Implementation Status
Sample formulas only.

The data sources, screen controls and variables
must be configured before these formulas can work.
