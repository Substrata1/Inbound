**Inbound** broadcasts notifications when patrol helicopters, supply drops, hackable crates, cargo ships, Excavator, Bradley, or Chinook are active / inbound.

## Configuration

```json
{
  "Notifications": {
    "Chat Notifications": true,
    "Popup Notifications": false
  },
  "Discord Messages": {
    "Enabled": false,
    "Webhook URL": "",
    "Embedded Messages": true,
    "Embed Color": 3447003,
    "Embed Title": ":arrow_lower_right:  Inbound"
  },
  "UI Notify": {
    "Enabled": false,
    "Notification Type": 0
  },
  "Alerts": {
    "Patrol Helicopter Alerts": true,
    "Cargo Ship Alerts": true,
    "Cargo Ship Harbor Alerts": true,
    "Cargo Plane Alerts": true,
    "CH47 Chinook Alerts": true,
    "Bradley APC Alerts": true,
    "Excavator Activated Alerts": true,
    "Excavator Supply Request Alerts": true,
    "Hackable Crate Alerts": true,
    "Player Hacking Crate Alerts": true,
    "Supply Signal Alerts": true,
    "Supply Drop Alerts": true,
    "Supply Drop Landed Alerts": true
  },
  "Location": {
    "Show Grid": true,
    "Show 'Oil Rig' Labels": true,
    "Show 'Cargo Ship' Label": true,
    "Show 'Excavator' Label": true,
    "Hide Unmarked Grids": true,
    "Grid Offset": false,
    "Show Coordinates": false,
    "Hide Y Coordinate": false,
    "Hide Coordinate Decimals": false
  },
  "Misc": {
    "Chat Icon (SteamID64)": 0,
    "Hide Cargo Ship Crate Messages": false,
    "Hide Oil Rig Crate & Chinook Messages": false,
    "Show Supply Drop Player": false,
    "Hide Player-Called Supply Drop Messages": false,
    "Hide Random Supply Drop Messages": false
  },
  "Logging": {
    "Log To Console": false,
    "Log To File": false,
    "Log All Events": false
  },
  "Version (Do not modify)": {
    "Major": 0,
    "Minor": 6,
    "Patch": 6
  }
}
```

- **Show Supply Drop Player** will add the name of the player who called in a Cargo Plane / Supply Drop when those alerts are shown. This can be further tweaked in the language file.
- **Hide Player-Called Supply Drop Messages** will hide alerts for Cargo Planes and Supply Drops that have been called in by a player, with a supply signal or at the Excavator signal computer. **Hide Random Supply Drop Messages** will hide alerts for those that have not.
- **Grid Offset** will offset the grid number by 1, if needed. See Known Issues for more info.
- For info on creating a Webhook for Discord Messages, check out [Intro to Webhooks](https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks).

## Localization

```json
{
  "PatrolHeli": "Patrol Helicopter inbound{0}{1}",
  "CargoShip_": "Cargo Ship inbound{0}{1}",
  "CargoShipApproachHarbor": "Cargo Ship is approaching the harbor{0}",
  "CargoShipAtHarbor": "Cargo Ship has docked at the harbor{0}",
  "CargoShipLeaveHarbor": "Cargo Ship is leaving the harbor{0}",
  "CargoPlane_": "{0}Cargo Plane inbound{1}{2}",
  "CH47": "Chinook inbound{0}{1}",
  "BradleyAPC": "Bradley APC inbound{0}",
  "Excavator_": "{0} has activated The Excavator{1}",
  "ExcavatorSupplyRequest": "{0} has requested a supply drop{1}",
  "HackableCrateSpawned": "Hackable Crate has spawned{0}",
  "HackingCrate": "{0} is hacking a locked crate{1}",
  "SupplySignal": "{0} has deployed a supply signal{1}",
  "SupplyDropDropped": "{0}Supply Drop has dropped{1}",
  "SupplyDropLanded_": "{0}Supply Drop has landed{1}",
  "SupplyDropPlayer": "{0}'s ",
  "Location": " at {0}",
  "Destination": " and headed to {0}",
  "DiscordMessage_": "{0}"
}
```

- The **{0}** in **"CargoPlane_"**, **"SupplyDropDropped"**, and **"SupplyDropLanded_"** will show the player name, if enabled in the config.<br />Example: "Substrata's Supply Drop has dropped at D3"

## Known Issues

- The **Show Supply Drop Player**, **Hide Player-Called Supply Drop Messages**, and **Hide Random Supply Drop Messages** options do not currently work with any plugins that kill & respawn the Cargo Plane or Supply Drop. These include Fancy Drop, Airdrop Precision, and possibly others. Compatibility for these can hopefully be added at some point.
- On some map sizes (3500, for example), the grid number may be off by 1. If this is the case for you, you can use the **Grid Offset** option to correct it. This is on Facepunch to fix.
- Unmarked grids to the left of the map will not show, as there is currently no good way of labeling these.

## Credits

- **PaiN** and **Splak**, for originally fulfilling the heli notification request, but in the wrong place. ;)
- **Tori1157**, for helping maintain the plugin
- **Wulf**, the original author of this plugin

## Donate

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F1F8826WW)
