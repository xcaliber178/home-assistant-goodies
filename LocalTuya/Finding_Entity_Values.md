# Finding Instructions and Values with IoT Platform

The Tuya IoT Platform provides, among many other things, a list of all linked devices. This information is very useful for adding new devices that we have not documented yet. 

The IoT Platform will show you all of the *Standard Instructions* as well as the *DP Instructions*. These instructions are methods of passing values to and from the device via Home Assistant entities. While the device (and IoT Platform) may reference `switch_1`, LocalTuya may reference it as `ID: 1` followed by it's current value such as `(value: False)`. In this example `switch_1` is a boolean and has a value of `True` or `False`.

Instructions can be a variety of data types including booleans, strings, integers, enums, and possibly more. The *Standard Instruction* mode is a standardized set of instructions provided by IoT Platform and appear to be consistant across all devices. Behind this layer is the *DP Instruction* mode. This mode feeds instructions into the *Standard Instruction* mode but also can contain device/developer specific instructions. These are also visible to LocalTuya during the *Configure entity* stage of adding a device.

Determining which device instruction goes to which `ID:` in LocalTuya is not as streamlined as one would hope. Upon initial documentation of a device, pull up the devices instruction table on IoT Platform and add the device in LocalTuya as a tester. Get to the *Configure entity* stage and compare the `ID:` values to the instruction values. You can issue commands back to the device from the IoT Platform and then back out of the *Configure entity* page and go back in and see what changed. It's also useful to monitor the physical device to match instructions/`ID:` values to the actual function it controls.

*Beware that not all instructions are useful, produce meaningful results, provide meaningful info, or function at all in it's application.*

## Getting *Standard Instruction* Table and Values

0. Have a Tuya IoT Platform account
0. Go to the [Tuya IoT Platform](https://iot.tuya.com/)
0. Go to the **Cloud** portal (left sidebar)
0. Select your project
    - **ICT-HA** in our case
0. Go to the **Devices** tab
0. Find the device
    - Try sorting by *Product*
0. Select **Debug Device**
0. Go to the **Device Debugging** tab
    - The left column shows a list of all your devices
    - The center column shows current values and allows you to control the device
        - **Update Device Status**
        - **Send Instructions**
    - The right column shows details about each instruction including the *data type* and the *possible values*

## Getting *DP Instruction* Table

1. Follow the instructions above to the **Device Tab**
0. On the horizontal bar *View Devices by Product.*, find the product of the device and cl

## _**IN PROGRESS**_