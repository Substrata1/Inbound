**Inbound** broadcasts notifications when patrol helicopters, supply drops, hackable crates, cargo ships, Bradley, or Chinook are inbound.

## Configuration

```json
{
  "Alerts (true/false)": {
    "Bradley APC Alerts": true,
    "Cargo Plane Alerts": true,
    "Cargo Ship Alerts": true,
    "CH47 Chinook Alerts": true,
    "Hackable Crate Alerts": true,
    "Patrol Helicopter Alerts": true,
    "Player Hacking Crate Alerts": true,
    "Player Supply Signal Alerts": true,
    "Supply Drop Alerts": true
  },
  "Coordinates (true/false)": {
    "Show Coordinates": false,
    "Show Coordinates - Destination": false
  },
  "Grid (true/false)": {
    "Show Grid": true,
    "Show Grid - Destination": true,
    "Show Oil Rig / Cargo Ship Labels": true
  },
  "Misc (true/false)": {
    "Log To Console": false,
    "Log To File": false
  }
}
```

* The destination settings currently apply to patrol heli, cargo plane, and Chinook, and show where they are headed.
* When **Show Oil Rig / Cargo Ship Labels** is set to true, the grid will be replaced with Oil Rig, Large Oil Rig, or Cargo Ship, where applicable.

## Localization

```json
{
  "BradleyAPC": "Bradley APC inbound{0}",
  "CargoPlane": "Cargo Plane inbound{0}{1}",
  "CargoShip": "Cargo Ship inbound{0}",
  "CH47": "Chinook inbound{0}{1}",
  "HackableCrate": "Hackable Crate has spawned{0}",
  "PatrolHeli": "Patrol Helicopter inbound{0}{1}",
  "HackingCrate": "{0} is hacking a locked crate{1}",
  "SupplySignal": "{0} has deployed a supply signal{1}",
  "SupplyDrop": "Supply Drop has dropped{0}",
  "Location": " at {0}",
  "LocationDestination": " and headed to {0}"
}
```

## Known Issues

* Unmarked grids to the left of the map will not show, as there is currently no good way of labeling these.
* Cargo Ship destination is (as far as I know) not currently accessible, and can't be shown.

## Credits

* **PaiN** and **Splak**, for originally fulfilling the heli notification request, but in the wrong place. ;)
* **Tori1157**, for helping maintain the plugin
* **Wulf**, the original author of this plugin
