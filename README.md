# RB2B Flow 2

## Overview

An RB2B (website visitor identification) to CRM pipeline. When RB2B identifies a new website visitor, the workflow cleans the data, checks if the person already exists in the CRM, creates or updates the person record, creates an associated deal, and updates the deal stage based on the visitor's engagement. It routes through different paths depending on whether the person is new or existing.

## How It Works

```
RB2B New Message -> Cleanup Data -> Person Exists? -> If yes: Update Deal Stage -> If no: Create Person -> Create Deal -> Create Associated Deal
```

## Integrations

- **RB2B** - Website visitor identification trigger

## Setup

1. Import `RB2B_FLOW_2.json` into your n8n instance.
2. Configure RB2B and CRM credentials.
3. Activate the workflow.
