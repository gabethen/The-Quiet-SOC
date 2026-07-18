# Week 2 Reflection - Investigating User Activity and System Logs

## What did I learn this week?

This week I learned how security analysts use system logs and user behavior analysis to investigate suspicious activity.

I learned that malicious activity leaves a footprint in the Windows Event Viewer. Rather than blindly searching logs, a SOC Analyst targets specific Event IDs to reconstruct activity:
- Event ID 4624 (Successful Logon):** Used to verify legitimate access or identify compromised credential usage.
- Event ID 4625 (Failed Logon):** Crucial for identifying pattern-based attacks like brute-forcing or password spraying.
- Event ID 4688 (Process Creation):** Allows analysts to see exactly what applications or scripts were executed after a user logged in, which is vital for spotting malware execution.

## What surprised me?

What surprised me most was how much information is hidden inside everyday computer activity. Login attempts, failed passwords, successful logins, and user actions can all become important evidence during an investigation.

## Why are logs important?

Logs provide a timeline of events. They allow analysts to understand what happened, when it happened, and what systems or users were involved.

Without logs, investigators would have to rely on assumptions instead of evidence.

## What SOC skill did I practice?

This week I practiced:

- Reading Windows Event Logs
- Identifying suspicious login behavior
- Understanding authentication events
- Thinking like an investigator instead of making assumptions

## Biggest takeaway

A good SOC analyst does not immediately assume something is malicious. They collect evidence, look for patterns, and make decisions based on facts.
