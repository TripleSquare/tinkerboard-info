##Testing Temperatures

| Load | Temperature | Description |
| --- | ---:| --- |
| - | 22°C | Ambient Room Temperature |


###Tinkerboard with Case 

| Load | Temperature | Description |
| --- | ---:| --- |
| idle | 46°C | none |
| 100% | 77~80°C | throttling 1~1.5GHz | 


###Tinkerboard without Case

| Load | Temperature | Description |
| --- | ---:| --- |
| idle | 40~42°C | none |
| 100% | 77~80°C | throttling 1~1.5GHz |


###Definition

**Idle**
>fresh OS flash with wired Ethernet, wifi and Bluetooth not connected, no peripherals connected

**Load**
>Synthetic load, generated using:  
```for i in 1 2 3 4; do while : ; do : ; done & done```
