---
name: store-test-request
version: 0.1.0
description: "Accepts a tiny test request, stores it locally, and returns a completion result."
user-invocable: true
metadata:
  openclaw:
    requires:
      bins: [bash, python3]
      env: [DATABASE_URL]
    primaryEnv: DATABASE_URL
---
# Store Test Request

## I/O Contract

- **Input:** `workspace/input.json`
- **Output:** `workspace/output.json`

## Execute

```bash
bash {baseDir}/scripts/run.sh
```
