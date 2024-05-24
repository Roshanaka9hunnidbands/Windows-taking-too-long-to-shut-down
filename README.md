## Xbox 360 Controller Disconnect Issue on Windows 11 (AMD Ryzen 5 7600) - Solution

### Problem Description

If you're experiencing issues with your Xbox 360 controller disconnecting on Windows 11, particularly with AMD Ryzen 5 7600 (non-X variant) systems after the February 23H2 update, you're not alone. The root cause of this issue is the receiver going into standby mode, which causes the controller to disappear from the Device Manager when turned off. This problem is not with the controller itself but with the receiver.

### Symptoms
- Xbox 360 controller disconnects and disappears from the Device Manager when turned off.
- The receiver intermittently turns off and on, signaling the controller to turn off if no input is detected for 3 minutes.
- This issue predominantly occurs after the Windows 11 February 23H2 update.

### Workaround Solution
To mitigate this issue, follow these steps:

1. **Replace the Receiver**:
   - Use a receiver that does not go into standby mode. The larger receivers with blinking LEDs tend to have this issue, while smaller, stubby 2.4 GHz receivers without lights work better.

2. **Avoid Connecting/Disconnecting Controllers Frequently**:
   - If your current receiver has a standby mode, avoid frequently connecting or disconnecting your controller.

3. **Use an Always-Connected Controller**:
   - Opt for a controller that shows as always connected in the Device Manager, regardless of activity status.

### Temporary Fixes
While waiting for Microsoft to address this issue in a future update, you can try these temporary fixes:

1. **Uninstall the 23H2 Update**:
   - Roll back to a previous Windows version before the February 23H2 update.

2. **Put Your PC to Sleep Instead of Shutting Down**:
   - Use sleep mode instead of shutting down your PC to maintain the connection.

### Conclusion
The issue primarily stems from the receiver entering standby mode, causing disconnections. By using a more reliable receiver and adjusting your usage habits, you can mitigate the problem until a permanent fix is released in a future Windows update.

Feel free to open an issue if you have further questions or need additional assistance. Your feedback helps improve the solution for everyone facing similar problems. 

---

If you have any suggestions or additional solutions, please contribute to this repository by creating a pull request or opening an issue. Thank you!
