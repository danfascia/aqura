# Database Schemas

## Patients

## Sessions
Resource based schedules

## Episodes
Attendances with a facility (N-1: Patient)

## Studies
Individual tests within an episode (N-1: Episode)

## Services
Attached to Studies to map billing and operational instructions (protocol etc) (1:1)

## Invoices
Attached to episodes for billing cycle management (1:1)

## Results
Result for an Episode or Study (1:1) with additional permissions and distribution information to manage result lifecycle and access rights
