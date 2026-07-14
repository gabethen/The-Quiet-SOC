# Mission 04 – Windows Event Logs

### 1. Why are Windows Event Logs valuable during an investigation?

Windows Event Logs are valuable during an investigation because they record important activity that occurs on a computer. They provide evidence of events such as user logins, system changes, software activity, and security-related actions, allowing investigators to understand what happened and when it happened.

### 2. Which log would you check first if you suspected someone was trying to guess a user's password?

I would check the **Security** log first because it records successful and failed login attempts, account lockouts, password changes, and other authentication-related events. These logs can help determine whether someone is attempting to gain unauthorized access.

### 3. Why isn't one failed login enough to prove an attack?

One failed login is not enough to prove an attack because people often mistype their passwords or forget them. A SOC analyst should look for patterns, such as multiple failed login attempts, unusual login times, unfamiliar locations, or a successful login immediately after several failures before concluding that malicious activity occurred.

### 4. What does Event ID 4624 represent?

Event ID **4624** represents a successful user login.

### 5. What does Event ID 4625 represent?

Event ID **4625** represents a failed user login attempt.
