# Architecture Documentation

## Overview
This Reflection implements Curriculum Planner for Enrollment for Education use cases.

## Components
1. **Student Intake**: Collect, validate and normalize attendance from SIS; attach a runId and timestamp for traceability.
2. **Draft**: Execute draft phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Self-Critique**: Execute self-critique phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Proctoring**: Proctoring across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Personalized Plan**: Personalized Plan across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Practice Recommendation**: Practice Recommendation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Readiness Check**: Readiness Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Instructor Review**: Assemble final payload with status, artifacts, KPIs and audit trail; store to Tutoring System; return response JSON for the client.

## Data Flow
- Input: Student Intake
- Processing: 8 sequential steps
- Output: Instructor Review
