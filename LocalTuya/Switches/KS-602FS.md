`KS-602FS`
# Standard Switch Setup in Tuya Local
## Adding Device

Tuya Local > Configure > Add a new device > **Submit**

Discovered Devices > Pick from dropdown > **Submit**

Name: `[room/location]` (this is the entire device name)

*Submit*

## Creating Entities
### **Default State Behavior** - *This may not be functional*

Platform: `select`  
*Submit*

ID: `14`  
Friendly name: `[device_name] Default Behavior`  
Valid entries: `power_off; power_on; last`  
User Friendly options: `Off; On; Last State`
- [x] Restore the last set value in HomeAssistant after a lost connection

*Submit*

---

### **Physical Lockout Setting**
Platform: `switch`
- [ ] Do not add any more entities

*Submit*

ID: `101`  
Friendly name: `[device_name] Lockout`
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
