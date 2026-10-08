# Home Credit LAP Voice Agent — Test Cases

## Test 1 — Fully Eligible Customer

### Scenario

Customer provides all required information and satisfies every eligibility condition.

### Expected Behavior

The agent should collect all seven eligibility points and complete the preliminary qualification.

### Result

PASS

---

## Test 2 — Agricultural Property

### Customer Scenario

Customer says the property is agricultural land.

### Expected Behavior

The agent should immediately identify that agricultural property is not eligible, explain politely, and end the qualification.

### Result

PASS

---

## Test 3 — Cash Income

### Customer Scenario

Customer is self-employed and receives income entirely in cash.

### Expected Behavior

The agent should identify that cash income does not satisfy the requirement, politely explain the reason, and end the qualification.

### Result

PASS

---

## Test 4 — Original Documents Missing

### Customer Scenario

Customer has an eligible property but does not have the original property documents.

### Expected Behavior

The agent should immediately disqualify the customer for this specific offer and end the qualification.

### Result

PASS

---

## Test 5 — Loan Amount Above ₹75 Lakhs

### Customer Scenario

Customer requests a loan amount of ₹90 Lakhs.

### Expected Behavior

The agent should explain that the maximum offer is ₹75 Lakhs and ask whether the customer wants to continue with the maximum eligible amount.

If the customer agrees, the agent should continue the eligibility assessment.

### Result

PASS

---

## Test 6 — Existing Loan / EMI Reduction

### Customer Scenario

Customer says they already have a loan on the property and want to reduce their current EMI.

### Expected Behavior

The agent should:

1. Stop the normal LAP qualification flow.
2. Recognize the existing-loan/EMI-reduction requirement.
3. Explain that a loan-transfer specialist is required.
4. Trigger the configured call-transfer function.
5. Transfer the customer when the tool succeeds.

### Result

PASS

---

## Test 7 — Busy Customer / Callback

### Customer Scenario

Customer says they are currently busy and cannot talk.

### Expected Behavior

The agent should not continue the eligibility questions. It should ask for a convenient callback time, confirm it, and end the call politely.

### Result

PASS

---

## Additional Behavioral Tests

### Out-of-Order Information

The customer may provide eligibility information before the agent asks for it.

### Expected Behavior

The agent should remember the information and must not ask for the same information again.

### Result

PASS

---

### Customer Interruption

The customer may interrupt the agent during a question.

### Expected Behavior

The agent should respond naturally and continue from the appropriate unanswered eligibility point.

### Result

PASS

---

## Overall Test Result

All seven primary assignment scenarios were tested.

**Overall Status: PASS**

The agent successfully handles normal qualification, disqualification scenarios, amount-limit handling, existing-loan transfer logic, callback handling, and out-of-order customer information.
