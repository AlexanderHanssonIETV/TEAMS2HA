---
icon: hand-wave
---

# README

![CodeQL](https://github.com/jimmyeao/TEAMS2HA/actions/workflows/codeql.yml/badge.svg)

![GitHub tag](https://img.shields.io/github/tag/jimmyeao/TEAMS2HA?include_prereleases=\&sort=semver\&color=blue)

![License](https://img.shields.io/badge/License-MIT-blue)

![issues - Teams2HA](https://img.shields.io/github/issues/jimmyeao/TEAMS2HA)

## Teams2HA

DONT FORGET TO ENABLE THE API IN TEAMS! test!

Settings, Privacy, scroll to bottom and under 3rd party api click Manage Api then enable it

This is an agent that runs on windows and uses the Local teams API (https://support.microsoft.com/en-gb/office/connect-to-third-party-devices-in-microsoft-teams-aabca9f2-47bb-407f-9f9b-81a104a883d6?wt.mc\_id=SEC-MVP-5004985) to retrieve the status of the user (In a meeting, Video On, Mute, blur etc) and push these into homeassistant sensors using MQTT.

Download the latest version from https://github.com/jimmyeao/TEAMS2HA/releases (app will auto update once installed)

![image](https://github.com/jimmyeao/TEAMS2HA/assets/5197831/c79d09a4-0770-470f-a941-d21f85e1cf37)

### Pairing

to pair, have the app running, launch a teams meeting (using meetnow?) and click Pair wtih teams. This will initiate a pairing request in teams, accept this, and then the app will store the key, in an encrypted format.

The application will minimize to the system tray.

### MQTT

Provide your MQTT instance details (IP, username and password) The password is encrypted before being saved to the settings file and is not stored in clear text.\
We support plain MQTT, MQTT over TLS, MQTT over Websockets and MQTT over Websockets with TLS and the ability to ignore certificate errors if you are using self-signed certs (I would strongly advise you to use Lets Encrypt as a minimum)

### Entities

Click the Entities button to see a list of entities this program will create:

![image](https://github.com/jimmyeao/TEAMS2HA/assets/5197831/5c87da53-e66a-4bc8-af4b-34af0ddc6d47)

You can either right click and copy or double click to copy the entity name to the clipboard.

### System Tray

You can right click the system tray icon for a selection of functions:

![image](https://github.com/jimmyeao/TEAMS2HA/assets/5197831/a8878f2e-38f6-4fce-a823-32f2008a0763)

This is how it should look in MQTT in Homeassistant

![image](https://github.com/jimmyeao/TEAMS2HA/assets/5197831/ce524451-a96a-4eac-bb94-67e36f449527)
