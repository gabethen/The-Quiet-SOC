Mission 05 – Investigating Windows Event Logs
1. What events occurred in order?

A user attempted to log in and experienced three failed login attempts at 9:00 AM, 9:01 AM, and 9:02 AM. At 9:03 AM, a successful login (Event ID 4624) occurred. Two minutes later, at 9:05 AM, the user logged off (Event ID 4634).

2. What activity looks unusual?

The most unusual activity is the three consecutive failed login attempts followed immediately by a successful login. While this could simply be a user entering the wrong password multiple times, it could also indicate someone attempting to guess a password. The quick logoff shortly after the successful login is also worth noting and should be investigated further.

3. Is there enough evidence to confirm an attack? Why or why not?

No, there is not enough evidence to confirm an attack. The failed login attempts could have been caused by a legitimate user forgetting or mistyping their password. Additional evidence is needed before determining whether the activity is malicious.

4. What additional information would you want before escalating this incident?

Before escalating the incident, I would gather the following information:

Username
Source IP address
Device name
Previous login history
Whether the user reported login issues
Any unusual activity recorded in the Windows Event Logs after the successful login

This additional information would help determine whether the login was legitimate or suspicious.

5. What would you recommend as the next step?

Based on the available evidence, I would:

Continue monitoring the account for additional suspicious activity.
Review the Windows Security Event Logs for related events.
Contact the user to verify whether they experienced login problems.
Recommend a password reset if the activity cannot be explained.
Escalate the incident to a senior analyst only if additional evidence suggests malicious activity.
