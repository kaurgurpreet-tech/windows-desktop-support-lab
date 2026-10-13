# Workstation Setup Checklist

## Purpose
Prepare a Windows workstation for use and record the checks completed. This is a general lab checklist, not a substitute for an organization's build standard.

## 1. Confirm requirements
- [ ] Confirm the intended user role and required applications.
- [ ] Confirm device ownership, asset tag (if applicable), and approved build instructions.
- [ ] Confirm Windows edition/version and hardware compatibility.
- [ ] Confirm whether the device is personal, lab-owned, or organization-managed.
- [ ] Confirm the approved network and account setup method.
- [ ] Record any special requirements and obtain approval before making changes.

## 2. Inspect hardware
- [ ] Check laptop/desktop, power adapter, monitor, dock, keyboard, mouse, webcam, headset, and cables.
- [ ] Look for visible damage or unusual heat/noise.
- [ ] Confirm the display, ports, and power connection work.
- [ ] Connect peripherals one at a time if diagnosing a problem.
- [ ] Record faults and do not deploy damaged equipment.

## 3. Record system information
Open **Settings > System > About** and record the device model, processor, installed RAM, Windows edition, and version. Do not include serial numbers or other identifiers in a public repository.

Optional command:
```powershell
Get-ComputerInfo | Select-Object WindowsProductName, WindowsVersion, OsBuildNumber, CsManufacturer, CsModel
```
Review output before saving; redact device identifiers and sensitive information.

## 4. Windows configuration
- [ ] Confirm Windows activation/status through Settings.
- [ ] Check date, time, time zone, and language.
- [ ] Check Windows Update and install approved updates.
- [ ] Restart if required, then recheck update status.
- [ ] Confirm storage has reasonable free space.
- [ ] Review Device Manager for unexpected warning symbols.
- [ ] Confirm Windows Security status without weakening protections.
- [ ] Confirm power, sleep, display, and accessibility settings as required.
- [ ] Confirm the correct account type and least-privilege access.
- [ ] For a managed device, follow the organization's approved enrollment and security process; do not improvise enrollment.

## 5. Accounts and access
- [ ] Use only an authorized test account in this lab.
- [ ] Verify sign-in and sign-out.
- [ ] Check that the user has only the permissions required.
- [ ] Confirm access to approved resources.
- [ ] Do not store passwords, recovery codes, or MFA secrets in the repository.

## 6. Network
- [ ] Connect to the intended authorized network.
- [ ] Check IP configuration using `ipconfig /all`.
- [ ] Test the local gateway with `ping <gateway-IP>` if ICMP is allowed.
- [ ] Test name resolution with `nslookup <approved-hostname>`.
- [ ] Test access to an approved website or business resource.
- [ ] Record whether the issue is Wi-Fi, IP configuration, DNS, VPN, or application-specific.

## 7. Applications and peripherals
- [ ] Install only approved software from a trusted source.
- [ ] Confirm application launches successfully.
- [ ] Confirm required sign-in and permitted access.
- [ ] Test printing or other peripherals if included in the setup.
- [ ] Test audio, microphone, camera, and external display if required.
- [ ] Record version numbers where useful.

## 8. Final review
- [ ] Complete `pre-deployment-validation.md`.
- [ ] Complete `user-handover.md`.
- [ ] Record unresolved issues and their owners.
- [ ] Confirm no test data, personal data, or secrets remain on the device.
- [ ] Record date, tester, and outcome in your private lab notes.

## Results
- Date tested: `[YYYY-MM-DD]`
- Environment: `[device/VM and Windows version]`
- Outcome: `[Pass / Pass with issues / Fail]`
- Findings: `[actual observations only]`
