## Managing Windows Updates with Deep Freeze

Deep Freeze allows administrators to perform Windows Updates remotely across multiple devices. This feature is particularly useful for keeping systems up-to-date with the latest security patches and features without needing to physically access each machine.

### Remote Windows Updates
When you initiate a Windows Update remotely through the Deep Freeze Console, the device is automatically Thawed, allowing the update process to complete. Once the updates are installed, the system is automatically Refrozen, ensuring that the device remains protected against unwanted changes.

### Important Note on Outdated Devices
> **Note:** If a device has not been updated for an extended period, it may require multiple reboots and firmware updates during the Windows Update process. Deep Freeze may not fully handle these scenarios, as the system may require more reboots than a typical update. In such cases, it is recommended to manually Unfreeze the device, perform the Windows Updates directly through the Windows Update tool, and then Refreeze the device once all updates are complete.

### Steps to Perform Windows Updates Remotely

#### Method 1: Using the Context Menu
1. Open the Deep Freeze Console.
2. Right-click on the device you wish to update.
3. Select **Windows Update** from the context menu.
4. Confirm that the device is Thawed, and the update process will begin.
5. Once the update is completed, the device will automatically Refreeze.

![Windows Update](https://github.com/user-attachments/assets/3e2ae5e6-4182-40ac-9c76-6e3899b990d6)


#### Method 2: Using the Toolbar
1. Open the Deep Freeze Console.
2. Click on the device you wish to update to select it.
3. In the top Toolbar, click on the **Windows Update** icon.
4. Confirm that the device is Thawed, and the update process will begin.
5. The device will automatically Refreeze after the updates are installed.

![Windows Update2](https://github.com/user-attachments/assets/4b8aa770-0d6e-4a76-b696-01abc8b94cde)


This remote update feature helps maintain security and functionality across all managed devices, but manual intervention may be necessary for devices that have not been updated in a long time.
