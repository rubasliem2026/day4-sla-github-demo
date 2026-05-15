# Manual Test Notes

## Test case 1
Input:
- CASE-101
- slaBreached: true
- escalated: false

Expected result:
- escalationEventCreated: true
- escalated becomes true

## Test case 2
Input:
- CASE-102
- slaBreached: true
- escalated: true

Expected result:
- escalationEventCreated: false
- no duplicate escalation

## Test case 3
Input:
- CASE-103
- slaBreached: false
- escalated: false

Expected result:
- escalationEventCreated: false
- no escalation needed
