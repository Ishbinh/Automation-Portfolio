**Employee Leave Request Approval**

## Objective
Built a simple leave approval workflow using expressions and an IF node.

## Workflow
Manual Trigger

→ Edit Fields

→ IF (No of days = 2)

True → Auto Approved

False → Needs Manager Approval

## Expression Used

Access a field
```javascript
{{ $json["Employee Name"] }}
```

Convert to number
```javascript
{{ Number($json["No of days"]) }}
```

Dynamic message
```javascript
Hi {{ $json["Employee Name"] }},
Your request for {{ $json["Leave Type"] }} for {{ $json["No of days"] }} days needs manager approval.
```

## Key Learnings
- Used `{{ }}` expressions to access data.
- Used `$json` to read values from previous nodes.
- Built conditional branching with an IF node.
- Learned that a node cannot reference fields it is creating.

<img width="1542" height="685" alt="image" src="https://github.com/user-attachments/assets/b66f987f-8099-43b3-9308-410882b57cb4" />
