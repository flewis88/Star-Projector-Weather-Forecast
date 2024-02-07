# Star-Projector-Weather-Forecast
Integration with Home Assistant to pull weather forecast and project galaxy colour depending on forecast temperature for today (in Celsisus), and increase brightness of stars dependent on forecast rain from 0-100mm.

Prerequisites:
- Home Assistant
- Tuya compatible Star Projector
- LocalTuya integration

Steps:
1. Configure Star Projector & DP IDs via GUI or \config\.storage\core.config_entries as per LocalTuyaDeviceConfig.md (Note Colour uses the 'select' entity with hardcoded colours expressed in 12bit HEX "hhhhssssvvvv". This may be able to be modified to accept input of the HSV colour as unique 12 bit HEX, allowing for seamless temp changes)
2. Create sensor for "Forecast High Temp" & "Rainfall Projection" in templates.yaml
3. Create script for "Turn Stars on Temp & Rain"in scripts.yaml
4. Create an Automation to execute the script at a given time in Automations.yaml

![il_680x540 3766546169_593x](https://github.com/flewis88/Star-Projector-Weather-Forecast/assets/52615288/e544f308-7ad9-4029-81f1-adffc4c975cf)
