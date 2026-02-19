# Compliance Engine

The compliance engine defines the checks used to approve, flag, or reject marketplace content and seller behavior.

## Control Layers

1. **Pre-Publish Controls**: static checks for required fields, claim patterns, and restricted terms.
2. **Risk Scoring**: prioritization by seller tier, category risk, and historical behavior.
3. **Human Review**: adjudication for ambiguous, high-risk, or escalated cases.
4. **Post-Publish Monitoring**: continuous detection of harmful trends and repeat violations.

## Decision Outcomes

- **Approve**: listing passes controls and is publishable.
- **Conditional Approve**: publish with mandatory edits or warnings.
- **Reject**: listing blocked pending substantive correction.
- **Escalate**: route to moderation governance for final decision.

## Auditability

Every decision must preserve:

- Decision timestamp,
- Triggered checks,
- Responsible reviewer or system control,
- Enforcement action and rationale.
