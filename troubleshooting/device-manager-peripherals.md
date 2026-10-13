# Troubleshooting Guide: Device Manager and Peripherals

## Scenario
A monitor, keyboard, mouse, printer, webcam, headset, dock, or other device is not detected or does not work properly.

## 1. Identify the device and impact
- What device is affected and what should it do?
- Is it USB, Bluetooth, network-connected, or dock-connected?
- Is the issue new or intermittent?
- Does it affect another port, cable, or computer?
- Did a driver, Windows update, or hardware change occur recently?

## 2. Check simple causes first
1. Check power, battery, mute switch, cable seating, and physical damage.
2. Confirm the correct input/output device or monitor source is selected.
3. For Bluetooth, check power, pairing, and whether the device is connected to another host.
4. For printers, check power, paper, error indicators, and whether the correct printer/queue is selected.
5. Test a known-good cable/port or device if available and authorized.

## 3. Review Device Manager
1. Right-click Start and open **Device Manager**.
2. Look for warning icons and identify the affected device category.
3. Open the device's Properties and review **Device status** on the General tab.
4. If useful, review the Driver tab and record the provider/version.
5. Check Windows Update or the device manufacturer's official support page for the appropriate driver.
6. Do not download drivers from unknown sites.

## 4. Apply a cautious fix
- Restart the application or reconnect the peripheral.
- Try another port or approved cable.
- Install an approved driver/update when evidence supports it.
- Use **Roll Back Driver** only if a recent driver change is a plausible cause and the option is available.
- Do not uninstall a device, delete driver packages, or change system-wide settings without understanding the impact and having a recovery plan.
- For a managed workstation, follow the organization's hardware and driver process.

## 5. Device-specific checks
### Display or dock
- Confirm monitor power and input source.
- Confirm cable/adapter compatibility.
- Press `Win + P` and check the intended display mode.
- Test direct connection versus dock if available.

### Audio or headset
- Check selected output/input device and volume.
- Check mute controls and app-specific audio settings.
- Test with an approved known-good headset if possible.

### Printer
- Confirm printer status and queue.
- Check connectivity and correct printer selection.
- Print a test page if authorized.
- Escalate shared print-server/queue issues to the responsible team.

## 6. Verify and document
- Confirm the device appears normally and works in the intended application.
- Re-test after restart if appropriate.
- Record device type, status/error, steps, driver details if relevant, and outcome.
