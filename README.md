# Real Estate – Instant Enquiry Alert

## Overview

An n8n automation prototype designed to help real estate agents respond promptly to property viewing enquiries.

The workflow captures prospective buyers' details and sends email notifications to both the agent and the prospective buyer.

## How It Works

1. A prospective buyer submits a property viewing enquiry form.
2. The workflow captures their contact details and property of interest.
3. The submitted information passes through workflow conditions.
4. The agent receives an enquiry notification by email.
5. The prospective buyer receives an acknowledgement email.

## Technology Stack

- n8n
- n8n Form Trigger
- Gmail
- Conditional logic

## Testing

I tested the workflow by submitting enquiries through the form.

Both the agent notification and prospective buyer acknowledgement emails were successfully received during testing.

## Setup Requirements

To run this workflow, you will need:
- An n8n instance.
- A Gmail account connected through n8n credentials.
- Your own agent notification email address.

The exported workflow has had credential references and the original notification recipient removed. Configure your own Gmail credentials and notification recipient before running it.

## Limitations and Future Improvements

This is a working prototype, not a production-ready enquiry management system.

Known limitations:
- The phone validation node's false output is not connected to a rejection or feedback path.
- Duplicate enquiry prevention has not been implemented.
- Error notifications and recovery handling have not been implemented.
- Additional safeguards are needed before handling prospective buyers' personal information in production.

Potential improvements include:
- Completing phone validation and rejection handling.
- Implementing persistent duplicate enquiry prevention.
- Adding error notifications and recovery handling.
- Strengthening personal information handling.

## Repository Contents

- `enquiry-alert-workflow.json` — exported n8n workflow.

## Project Status

Completed portfolio prototype.