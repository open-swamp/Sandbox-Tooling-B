# Sandbox Tooling Hardening Audit

## Premise
The task objective stated: "Harden sandbox tooling at the command boundary. Based on the current implementation, add a centralized policy for executable allowlisting, argument handling without shell interpolation, workspace path containment including symlink/junction escapes, environment-variable allowlisting/redaction, output limits, timeouts, and explicit denial reasons."

## Observation
Upon inspection, the repository is essentially empty. There is no existing implementation of sandbox tooling to harden.

## Action Taken
As per the operating contract ("If the repository is empty, the premise is contradicted by current code, or a prerequisite is absent, do not fabricate a large greenfield implementation. Instead add a concise evidence report under docs/audits/ for this task and implement only the smallest safe groundwork supported by existing architecture."), I am creating this evidence report and adding a stub implementation (`src/sandbox.py`) with stubs for adversarial tests (`tests/test_sandbox.py`) to provide the smallest safe groundwork.
