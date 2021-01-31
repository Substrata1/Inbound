**Inbound** broadcasts notifications when patrol helicopters, supply drops, hackable crates, cargo ships, Excavator, Bradley, or Chinook are active / inbound.

## Configuration

* The destination settings currently apply to patrol heli, cargo plane, and Chinook, and show where they are headed.
* When **Show Oil Rig / Cargo Ship Labels** is set to true, the grid will be replaced with Oil Rig, Large Oil Rig, or Cargo Ship, where applicable. If you enable the 'Hide on Cargo Ship / Oil Rig' options, these messages will be hidden regardless.
* In order to use a custom chat icon, you must enter a valid Steam ID. The associated profile picture will then be shown in chat messages. Default = 0.
* For info on creating a Webhook for Discord Messages, check out [Intro to Webhooks](https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks).

```json
{
  "Notifications (true/false)": {
    "Chat Notifications": true,
    "Popup Notifications": false
  },
  "Discord Messages": {
    "Enabled (true/false)": false,
    "Webhook URL": ""
  },
  "Chat Icon": {
    "Steam ID": 0
  },
  "Alerts (true/false)": {
    "Bradley APC Alerts": true,
    "Cargo Plane Alerts": true,
    "Cargo Ship Alerts": true,
    "CH47 Chinook Alerts": true,
    "Excavator Alerts": true,
    "Hackable Crate Alerts": true,
    "Patrol Helicopter Alerts": true,
    "Player Hacking Crate Alerts": true,
    "Player Supply Signal Alerts": true,
    "Supply Drop Alerts": true,
    "Supply Drop Landed Alerts": true
  },
  "Grid (true/false)": {
    "Show Grid": true,
    "Show Grid - Destination": true,
    "Show Oil Rig / Cargo Ship Labels": true
  },
  "Coordinates (true/false)": {
    "Show Coordinates": false,
    "Show Coordinates - Destination": false
  },
  "Misc (true/false)": {
    "Hide Cargo Ship Crate Messages": false,
    "Hide Oil Rig Crate Messages": false,
    "Log To Console": false,
    "Log To File": false
  }
}
```

## Localization

```json
{
  "BradleyAPC": "Bradley APC inbound{0}",
  "CargoPlane": "Cargo Plane inbound{0}{1}",
  "CargoShip": "Cargo Ship inbound{0}",
  "CH47": "Chinook inbound{0}{1}",
  "Excavator": "The Excavator has been activated{0}",
  "HackableCrate": "Hackable Crate has spawned{0}",
  "PatrolHeli": "Patrol Helicopter inbound{0}{1}",
  "HackingCrate": "{0} is hacking a locked crate{1}",
  "SupplySignal": "{0} has deployed a supply signal{1}",
  "SupplyDrop": "Supply Drop has dropped{0}",
  "SupplyDropLanded": "Supply Drop has landed{0}",
  "Location": " at {0}",
  "LocationDestination": " and headed to {0}",
  "DiscordMessage": ":arrow_lower_right:  **{0}**"
}
```

## Known Issues

* Unmarked grids to the left of the map will not show, as there is currently no good way of labeling these.
* Cargo Ship destination is (as far as I know) not currently accessible, and can't be shown.

## Credits

* **PaiN** and **Splak**, for originally fulfilling the heli notification request, but in the wrong place. ;)
* **Tori1157**, for helping maintain the plugin
* **Wulf**, the original author of this plugin
