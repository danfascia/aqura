![](https://github.com/danfascia/aqura/blob/main/assets/aqura-full-logo.svg)

# Aqura Diagnostics

## Aquris
### Functionality
- Receives referrals
- Protocolling
- Scheduling
- Patient Account Management
- Episode Management
- Billing
- Reporting
- Result Delivery
- API for front end solutions

#### In depth

| Functionality | Description | Frontend | Backend |
| --- | --- | --- | --- |
| Electronic Referrals | Electronic referral forms for authenticated referrers | Web based forms POST to | Aquris Rest API |
| Protocolling | Referral status episodes have studies assigned |  | Aquiris web GUI |
| Scheduling | Automated email to patient asking to select appointment time based on some rules and slots | Cal.com integration? | How would it integrate to Aquiris? Needs exploration |
| Patient Account Management | Patient > episodes (invoices, appointments) > studies | SPA with authenticated API calls for data | Aquiris web GUI |
| Episode Management | Protocol referrals, assign studies, calculate invoices, assign appointments, notify patient (status needed to trigger) | Aquiris web GUI + backend functions |
| Billing | Triggered on status change for episode (protocolled), pre-appointment depending on funding. | Email and web page render of invoice with pay links | Aquiris web GUI to administer |
| Reporting | Reports authored by radiologists into Aquris|  | Aquiris web GUI + system level VR & text macros  |
| Result Delivery | Options given to radiologist at authoring time on how/who to notify. | Email notification + protected web rendered report | Aquirus web GUI offers controls |
| REST API | Drives authentication and data for both front end 'apps' and 'views' as well as Aquiris web GUI | Aquiris web GUI | Postgres |
