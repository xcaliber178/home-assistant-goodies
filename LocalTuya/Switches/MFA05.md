`MFA05`
# Motion Switch Setup in Tuya Local
## Adding Device

Tuya Local > Configure > Add a new device > **Submit**

Discovered Devices > Pick from dropdown > **Submit**

Name: `[room/location]` (this is the entire device name)

*Submit*

## Creating Entities
### **??? Setting**
Platform: `switch`  
*Submit*

ID: `104`  
Friendly name: `[device_name] ???`
- [x] Restore the last set value in HomeAssistant after a lost connection

*Submit*

---

### **??? Setting**
Platform: `switch`
- [ ] Do not add any more entities

*Submit*

ID: `106`  
Friendly name: `[device_name] ???`
- [x] Restore the last set value in HomeAssistant after a lost connection

*Submit*

----

### **Light Switch Toggle**
Platform: `light`
- [ ] Do not add any more entities

*Submit*

ID: `1`  
Friendly name: `[device_name] Lights`  
*Submit*

---

### **Finishing**
- [*] Do not add any more entities

*Submit*  
__*Finish*__
