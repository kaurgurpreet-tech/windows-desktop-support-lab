# Troubleshooting Guide: Windows Sign-In Problems

## Scenario
A user reports they cannot sign in to Windows or repeatedly receives a sign-in error.

## 1. Clarify the symptoms
Ask:
- What exact error appears? Record it without passwords or personal data.
- Did sign-in work previously?
- Did anything change recently (password, update, network, device)?
- Is this a local account or an organization-managed account?
- Is one user affected or are multiple users affected?

## 2. Safe initial checks
1. Confirm the device is powered and has completed startup.
2. Check keyboard layout, Caps Lock, Num Lock, and input method.
3. Confirm the correct account/sign-in option is selected.
4. If using an organization account, check whether the device needs the organization's network or approved VPN for the particular operation.
5. Check whether there is a service outage or account lockout through approved support channels.
6. Avoid repeated guesses that could trigger lockout.

## 3. Gather evidence
- Record the error text, time, and recent changes.
- Determine whether the failure occurs before or after entering credentials.
- If authorized and accessible, review relevant Windows logs through Event Viewer.
- Do not record credentials, password hashes, recovery keys, or MFA codes.

## 4. Troubleshooting branches
### Keyboard or input issue suspected
- Test keyboard input in a safe field that does not expose sensitive information.
- Check keyboard layout and accessibility settings.
- Try a known-good keyboard if available.

### Account or password issue suspected
- Follow the official account recovery or help-desk identity-verification process.
- Check account status with an authorized administrator if this is a managed account.
- Never ask a user to send a password or MFA code.

### Organization sign-in or connectivity issue suspected
- Check whether other users are affected.
- Confirm approved network connectivity.
- Escalate identity-provider, domain, or device-enrollment errors to the authorized team.

### Profile or Windows issue suspected
- Record error details and check approved event logs.
- Avoid deleting or recreating profiles until data is protected and the procedure is authorized.
- Escalate if profile corruption or data loss is possible.

## 5. Verify
- Have the user sign in using the approved method.
- Confirm the desktop loads and required applications can open.
- Confirm the issue does not immediately recur.
- Record any remaining restrictions.

## Ticket notes
- Symptoms/error: `[actual text, sanitized]`
- Scope: `[one user/device or broader]`
- Checks and results: `[what you actually tried]`
- Cause: `[confirmed / suspected / unknown]`
- Resolution and verification: `[actual outcome]`
- Escalation: `[team/reason, if applicable]`
