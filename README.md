# Battery-Detect

# Battery events & Properties:
Note: Use battery API to detect battery status:
Ex- Js
code: navigator.getBattery() — access battery info as in the object;
If success: navigator.getBattery().then((e_name) =>{})

Properties: 
# @: charging: This property is used to detect current battery charging, TRUE or FALSE.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.charging? “Charging” : “Not Charging”}`);
});

# @: level: This property is used to detect current battery level, 0.0 to 1.0.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.level * 100}`);
});

# @: chargingTime: The remaining time in seconds until the battery is fully charged. Returns 0 if the battery is already full or Infinity if the device is discharging.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.chargingTime}seconds`);
});

# @: dischargingTime: The remaining time in seconds until the battery is completely discharged. Returns Infinity if the device is charging.
Ex-
navigator.getBattery().then((battery) =>{
console.log(`${battery.dischargingTime}seconds`);
});

# Events:

# @ chargingchange : Triggered when the charging status change or update.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`${battery.charging? “Charging” : “Not Charging”}`);
});

# @ levelchange : Triggered when the battery's charge level (level property) changes.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`Battery level changed: ${battery.level * 100}%`);
});

# @ chargingtimechange : Triggered when the remaining charging time (chargingTime property) changes.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`Charging time changed: ${battery.chargingTime} seconds`);
});

# @ dischargingtimechange : Triggered when the remaining discharging time (dischargingTime property) changes.
Ex-
navigator.getBattery().then((battery) =>{
battery addEventListener(“chargingchange”,() =>{
console.log(`Discharging time changed: ${battery.dischargingTime} seconds`);
});


# Screenshot 
https://lh3.googleusercontent.com/fife/ALs6j_GmDgsSG9d3BD4kVDePhIl8rT5b-_-n1wkx1SWJsK7KCKWfRURuYmrvPIQBJdb-DtsltxQX_9jchVncHcLhTXB-alTfB48DW7ueWtATkOjWYoO9SdxUJyVegMt9-KVWX3rOrMS1L8g7DQH49E4IsUiI0O1xfZvdkbBm_fXE51Cnd53HMoR_krHdz3IJHcsdNeBhEnT7rDhFgIXGWXda83SoUQEVcxtBfyu7p98_Ao_EtrZ8HWC99w8pwqN1OBifbRkCp9rud2jdYj-WB8jwIzYNHbORj87rV_9uvZXdKMVfBa5OSHatMchnRbMBBOkSW9Pddd8OaS7-OOHct9ENb2OFUA0XK4wYwU2-XXEctH4hq8JbWPBpQ7BuhYk79-O4ABCU50WwPFUk809LcCn-YCEBlRKfMvlxp4SQ8megPE8aTJRVruOyquwTg1Q08JYhHfUtRPicDxehIiLSnKc6aKQVfRxJbHyoz9R7g6FE04JwkgYGusGKJs7_7E-k1Rw1aQO6GheLzmadcjaKJSGfnwTF7ypmIEL9Hs11sG_YK7Ik5Quco08LxeUJYQ-q-tdinVPMtCIiUzTwMv1G8liUcODNIGFJiy9ER1ozummSL-M0Ostir6hru-O7-5iMVMrg7juCct41cH3Bx6ELTwrlrf1Zq5tJnS6ypJGu8tB2KmZLHsO2EjC-TWXq_1Wsk5nku9lkF-ZZbtppV1BUEogGA0SDG3UrylTBU6Dr94-ruzHBNYFBumE1Oq-bF62syg1aIngFjUqNO4CEir1KZ5ApU6uYk5YHgxizLTKq-rMc7bWbnYM2KO4lTUrLNZf6yLZyhBiGJCPYFqdAUkcpagTQlWtxOyr_XJXJStuBVBBLVqjGTuvGvWc3l10sROc80x-I0EvsNBIY8JjdwYscvMMkC7TERogXl7piszWyKj2r15Izew7f03O_oi-TtxZTZaEv9OivE4uw9SdrjJMJRaIqbWblIPOpRgwSNz0CCft5ic0x1ucvaza9Xy7REfHnUAIimBWxDAaUvEyFbx_HxciwP9JzYprpOGSN9JhKysTynE_RH4KNW0nsZNcZRnHXHvVL45erfzHIqeXycg33Obm4UDpJJBW4X24s9skj7KLFbqOOQ7pT6AsRdGYpq0PlRKhjXuLCXQbYybpsAcEdZrTMQjyGfrO8PZ_oabQlfRpDgLRi0LlbbnCZDYWvyA67Qxzxluh4Py6carXfBmE0FarQxfgaK0UBslVp1X6tq_w5jH2QJT75Z_LlTkrdw2lPjA4F1ApgRVK69CTc=s446-w446-h444-n-k?authuser=0&hl=en-GB

# live

https://codpro-sui.github.io/Battery-Detect/





