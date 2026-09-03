# AI Customer Update Assistant

A small AI-assisted workflow for turning operational information into clear customer updates and next steps.

## Why I built this

In customer-facing operations, a lot of time can go into collecting scattered information, figuring out what matters, and turning it into a clear update for a customer. I wanted to explore how AI could help with that process without removing human judgment.

## What it does

The workflow takes operational information such as:

- Current situation
- Route or location
- Estimated arrival information
- Driver or resource availability
- Customer constraints
- Known issues or delays

It then helps structure:

1. A short situation summary
2. A risk level and why it matters
3. Missing information that should be checked
4. Recommended next steps
5. A clear customer-facing update

## How it works

**Input → AI-assisted analysis → Human review → Customer update**

The AI is used to organize information and create a first draft. A person reviews the output, checks the underlying information, and makes the final decision before anything is shared with a customer.

## How I built it

I built this as a small prototype to explore a practical use case for AI in customer-facing operations.

1. **Identified the problem:** Customer updates often require pulling together information from different sources and turning it into a clear message.
2. **Defined the inputs:** I listed the operational details that can affect a shipment update, such as location, ETA, available driving time, customer constraints, and known issues.
3. **Designed the workflow:** I created a reusable prompt that asks AI to organize the information, identify risks and missing details, recommend next steps, and draft a customer-facing update.
4. **Tested the workflow:** I used a fictional shipment scenario to see whether the output was useful, clear, and actionable.
5. **Added human review:** The workflow is intentionally designed so that AI provides structure and a first draft, while a person verifies the information and makes the final decision.
6. **Documented the result:** I included the prompt, example input, and example output so the process can be reviewed and reused.

## Example

See the example files in [`examples/`](examples/):

- [`example_input.md`](examples/example_input.md)
- [`example_output.md`](examples/example_output.md)

The scenario is fictional and does not contain real customer or company information.

## Prompt

The reusable prompt and workflow instructions are available in [`workflow/prompt.md`](workflow/prompt.md).

## What I learned

Building this small workflow helped me think more intentionally about where AI is useful in customer-facing work: not necessarily replacing the person making the decision, but helping turn messy information into something structured, consistent, and easier to act on.

It also reinforced the importance of reviewing AI-generated information, especially when the output is used to communicate with customers.

## Limitations

This is a small prototype, not a production application. It does not connect to live transportation systems, customer databases, or private company data.
