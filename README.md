For

* klarstein Hot Spot Crystal Spotless Smart
* Termofol TF-750W
* Kogan glass panel heater

use

to fix issue with eco mode

```
external_components:
  - source: github://evlo/esphome-External-Components
    components: [tuyaClimateEcoEnum]
    refresh: 1s

climate:
  - platform: tuyaClimateEcoEnum
    supports_heat: true
    supports_cool: false
    name: "koupelnaTopeni"
    switch_datapoint: 1
    target_temperature_datapoint: 3  # min 5 - max 40
    current_temperature_datapoint: 4
    eco_datapoint: 7
    visual:
      min_temperature: 5
      max_temperature: 40
      temperature_step: 1
```
