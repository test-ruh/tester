# Step 5 of 5 — Access

## User Access

### Authorized Teams

| Team               | Access Level | Members (approx) |
|--------------------|-------------|-------------------|
| owner | full | just me |

### Restricted From

| Team / Role          | Reason                          |
|----------------------|---------------------------------|
| external users | This is only a dummy internal test agent. |

## HiTL Approvers

| Skill                | Action                         | Approver             | Fallback Approver    |
|----------------------|--------------------------------|----------------------|----------------------|
| store-test-request | approve data write | owner | skip write and return validation failure |

## Model Configuration

| Field                | Value                          |
|----------------------|--------------------------------|
| **Primary Model**    | gpt-4.1-mini   |
| **Fallback Model**   | gpt-4.1-mini  |

## Token Budget

| Field                  | Value                  |
|------------------------|------------------------|
| **Monthly Budget**     | 10000 tokens |
| **Alert Threshold**    | 8000 tokens |
| **Auto-Pause on Limit**| Yes |

## Security & Permissions

| Permission                         | Allowed    |
|------------------------------------|------------|
| database:write | ✅ |
| network:external | ❌ |
