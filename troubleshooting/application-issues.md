# Troubleshooting Guide: Windows Application Problems

## Scenario
An application will not launch, crashes, displays an error, or cannot access a required feature.

## 1. Establish scope and impact
- What application and version are affected?
- What is the exact error and when does it occur?
- Is the problem repeatable?
- Does it affect one user, one device, or multiple users?
- Did an update, configuration change, or password change occur recently?
- Is there an urgent business impact or workaround?

## 2. Start with low-risk checks
1. Confirm Windows is responsive and other applications work.
2. Close and reopen the application, saving work first if possible.
3. Check whether the application has a known service issue using an approved source.
4. Confirm the user can access the required network or resource.
5. Check date/time and available disk space where relevant.
6. Restart only if appropriate and after saving work.
7. Do not uninstall the application or delete its data before checking impact and backup needs.

## 3. Collect evidence
- Capture the exact error, time, application version, and steps to reproduce.
- Check Task Manager for an unresponsive process, if appropriate.
- Review application logs or Windows Event Viewer when accessible and relevant.
- Compare with a known-good account/device only when authorized.
- Remove personal information, tokens, and confidential content from screenshots/logs.

## 4. Diagnose likely causes
- **Application-specific:** one app fails but others work.
- **Account/permission:** app opens but a feature or resource is denied.
- **Network/service:** app cannot reach a server or online service.
- **Compatibility/update:** issue started after an update or OS change.
- **Resource/profile:** crash may relate to memory, disk, or user profile.
- **Wider outage:** multiple users report the same failure.

Treat these as hypotheses until evidence confirms them.

## 5. Apply an approved fix
- Follow vendor guidance or organizational procedures.
- Apply an approved update or repair option if suitable.
- Check permissions with an authorized administrator; do not grant excessive access.
- Escalate suspected server-side, licensing, security, or production issues.
- Change one thing at a time and record the result.

## 6. Verify and document
- Reopen the application.
- Repeat the original action that failed.
- Confirm the user can access the required function.
- Confirm no new error appears.
- Record the resolution, validation, and any follow-up.

## Case record
Application/version: `[value]`
Error and reproduction steps: `[value]`
Checks performed/results: `[value]`
Confirmed cause or current hypothesis: `[value]`
Change made and approval (if applicable): `[value]`
Verification: `[value]`
Status: `[Resolved / Escalated / Monitoring]`
