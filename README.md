# Windows taking too long to shut down when connected to a third party or a first party Xbox controller with a USB 2.4 GHz Receiver

# Fix for Shutdown Issues with Non-Bluetooth Xbox Controllers on Windows 11

## Overview

This repository documents a critical fix for a prominent issue affecting many Windows 11 users, particularly those using Xbox 360 controllers or other third-party controllers (excluding Xbox Series S Bluetooth controllers). The issue manifests as difficulties in shutting down the computer when these controllers are connected, especially if Steam or other specific background programs are running. Despite its prevalence, this problem has not received adequate attention or documentation.

## Problem Description

### The Issue

Many Windows 11 users have reported consistent issues with shutting down their computers when an Xbox 360 controller or other third-party controllers are connected. This problem is notably persistent if Steam or certain other background applications are running. Symptoms include:

- The computer hanging or taking an unusually long time to shut down.
- The shutdown process failing altogether, requiring a hard reset.
- Random errors or freezes during the shutdown process.

### Lack of Documentation

Despite being a widespread issue, there has been little to no credible documentation or official acknowledgement from Microsoft or other major sources. This lack of visibility has left many users without a clear solution, leading to frustration and repeated troubleshooting attempts.

## Solution

### Fix Using a 2.4 GHz Receiver and Adjusting GameInput Service Settings

A reliable fix involves using a 2.4 GHz receiver to spoof the computer into believing an Xbox 360 controller is always connected and adjusting the recovery settings of the GameInput Service in Windows. Additionally, it is crucial to ensure the receiver is always shown in Device Manager and disable it to prevent interference with existing controllers' connections.

### Steps to Implement the Fix

#### 1. Using a 2.4 GHz Receiver

1. **Plug in a 2.4 GHz Receiver**:
   - Connect a 2.4 GHz receiver to your computer. This will make the system think that an Xbox 360 controller is always plugged in and connected.
2. **Ensure the Receiver is Shown in Device Manager**:
   - Press `Win + X` and select **Device Manager**.
   - Locate the 2.4 GHz receiver under **Universal Serial Bus controllers** or **Human Interface Devices**.
   - Make sure the receiver is listed and recognized by the system.
3. **Disable the Receiver**:
   - Right-click on the 2.4 GHz receiver in Device Manager and select **Disable device**. This prevents interference with the existing controller's 2.4 GHz connection.

#### 2. Adjusting GameInput Service Settings

1. **Open Services**:
   - Press `Win + R`, type `services.msc`, and press `Enter`.
2. **Locate GameInput Service**:
   - Scroll down and find the **GameInput Service**.
3. **Modify Recovery Settings**:
   - Right-click on **GameInput Service** and select **Properties**.
   - Go to the **Recovery** tab.
   - For **First failure**, **Second failure**, and **Subsequent failures**, select **Take No Action** from the dropdown menus.
4. **Apply and Restart**:
   - Click **Apply** and then **OK**. Restart your computer to apply these changes.

### Verification

1. **Restart Your Computer**:
   - After implementing the fix, restart your computer.
2. **Test Shutdown**:
   - Test the shutdown process with the Xbox 360 controller or other third-party controllers connected.
3. **Run Background Programs**:
   - Ensure Steam or the previously problematic background program is running during the shutdown test.

### Expected Outcome

Following these steps should resolve the shutdown issues, resulting in a smooth shutdown process even with controllers connected and background applications running.

## Additional Notes

- This fix has been consistently effective but might not address all potential underlying causes related to specific hardware or software configurations.
- User feedback and further community testing are welcome to refine this workaround.


