# Battery-Detect

Battery events & Properties:
Note: Use battery API to detect battery status:
Ex- Js
code: navigator.getBattery() — access battery info as in the object;
If success: navigator.getBattery().then((e_name) =>{})

Properties: 
@: charging: This property is used to detect current battery charging, TRUE or FALSE.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.charging? “Charging” : “Not Charging”}`);
});

@: level: This property is used to detect current battery level, 0.0 to 1.0.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.level * 100}`);
});

@: chargingTime: The remaining time in seconds until the battery is fully charged. Returns 0 if the battery is already full or Infinity if the device is discharging.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.chargingTime}seconds`);
});

@: dischargingTime: The remaining time in seconds until the battery is completely discharged. Returns Infinity if the device is charging.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.dischargingTime}seconds`);
});

Events:

@ chargingchange : Triggered when the charging status change or update.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`${battery.charging? “Charging” : “Not Charging”}`);
});

@ levelchange : Triggered when the battery's charge level (level property) changes.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`Battery level changed: ${battery.level * 100}%`);
});

@ chargingtimechange : Triggered when the remaining charging time (chargingTime property) changes.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`Charging time changed: ${battery.chargingTime} seconds`);
});

@ dischargingtimechange : Triggered when the remaining discharging time (dischargingTime property) changes.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`Discharging time changed: ${battery.dischargingTime} seconds`);
});









