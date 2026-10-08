# Home Credit LAP Qualification Voice Agent

## Project Overview

This project is a voice-based AI agent designed for the **Home Credit Loan Against Property (LAP) Qualification** use case.

The agent contacts existing customers, explains a pre-approved LAP offer, performs preliminary eligibility screening, and handles qualified customers according to the defined business rules.

## Use Case

The agent can:

* Greet and identify the customer.
* Handle customers who are busy and arrange a callback.
* Explain the LAP offer of up to **₹75 Lakhs**.
* Collect the required eligibility information.
* Remember information provided out of order and avoid asking the same question again.
* Immediately disqualify customers who do not meet mandatory criteria.
* Handle loan requests above ₹75 Lakhs.
* Detect existing loans and EMI-reduction/loan-transfer requests.
* Transfer appropriate customers to the configured specialist.
* Hand off qualified customers to the senior loan expert process.

## Eligibility Criteria

The agent checks the following seven data points:

1. **Property Type**

   * Residential: Eligible
   * Commercial: Eligible
   * Industrial: Eligible
   * Agricultural: Not eligible

2. **Property Ownership**

   * Sole ownership: Eligible
   * Joint ownership: Eligible

3. **Original Property Documents**

   * Must be available.

4. **Loan Amount**

   * Maximum eligible amount: ₹75 Lakhs.

5. **Occupation & Income Mode**

   * Salaried or Self-employed.
   * Income must be received through a bank.
   * Cash income: Not eligible.

6. **Market Value**

   * Collected from the customer for preliminary assessment.

7. **Loan Tenure**

   * Minimum: 3 years
   * Maximum: 15 years

## Technology

* Retell AI
* Voice AI Agent
* System Prompt / Conversational Logic
* Call Transfer
* Call Recording and Transcript

## Testing

The agent was tested using multiple edge cases:

| Test | Scenario                      | Result |
| ---- | ----------------------------- | ------ |
| 1    | Fully Eligible Customer       | PASS   |
| 2    | Agricultural Property         | PASS   |
| 3    | Cash Income                   | PASS   |
| 4    | Original Documents Missing    | PASS   |
| 5    | Loan Amount Above ₹75 Lakhs   | PASS   |
| 6    | Existing Loan / EMI Reduction | PASS   |
| 7    | Busy Customer / Callback      | PASS   |

## Expected Outcome

The agent should conduct a natural conversation, follow the defined eligibility rules, avoid unnecessary repeated questions, and route customers appropriately based on their responses.

## Assignment

**Use Case:** Home Credit Loan Against Property (LAP) Qualification

**Platform:** Retell AI
