# API Documentation

## Endpoints
### Student Intake
- **Description**: Collect, validate and normalize attendance from SIS; attach a runId and timestamp for traceability.
- **Type**: Processing

### Draft
- **Description**: Execute draft phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Self-Critique
- **Description**: Execute self-critique phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Proctoring
- **Description**: Proctoring across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Personalized Plan
- **Description**: Personalized Plan across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Practice Recommendation
- **Description**: Practice Recommendation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Readiness Check
- **Description**: Readiness Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Instructor Review
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to Tutoring System; return response JSON for the client.
- **Type**: Processing
