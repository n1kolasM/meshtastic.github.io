> [!WARNING]
> Due to resource constraints, the HTTP server is deprecated on original-generation ESP32 devices and should not be relied on going forward.  
> Support continues on ESP32-S3 and other newer ESP32 generations.

## 🚀 Enhancements

- Add T5-4.7-S3 Epaper Pro support. #6625
- Apply Thailand NBTC 920-925 MHz limits (27 dBm, 10% duty cycle). #9827
- Switch nRF52840 builds to C++17. #9874
- Clean up SEN5X warnings. #9884
- Refactor BaseUI emotes. #9896
- Add spoof detection in `UdpMulticastHandler`. #9905
- Enable LNA by default on Heltec v4.3. #9906
- Rotate MUI for the Heltec V4 + TFT expansion kit. #9938
- Make `hexDump()` take a `const` buffer. #9944
- Add `meshtasticd` config metadata. #10001
- Add `MESHTASTIC_EXCLUDE_ACCELEROMETER`. #10004
- Adapt MUI WiFi map tile downloads for Heltec V4. #10011
- Fix Mesh-tab WiFi map and exclude-screen behavior. #10038
- Include Thinknode M5 minor fixes. #10049

## 🐛 Bug fixes and maintenance

- Remove GPS baudrate locking on the Seeed Xiao S3 kit. #9374
- Fix RAK4631 Ethernet gateway API connection loss after W5100S brownouts. #9754
- Fix W5100S socket exhaustion blocking MQTT and additional TCP clients. #9770
- Fix traceroute over MQTT when the uplink node is encrypted. #9798
- Extend Debian sourcedeb cache expiration. #9858
- Fix T-LoRA Pager SPI bus sharing between SX1262 and the SD card. #9870
- Update `ESP8266Audio` to the Meshtastic fork for compatibility. #9872
- Fix `rak_wismeshtag` low-voltage reboot hangs after app configuration. #9897
- Preserve `pki_encrypted` and `public_key` when relaying UDP multicast packets to radio. #9916
- Add the new RAK 13302 power curve. #9929
- Fix MQTT settings not persisting when the broker is unreachable. #9934
- Fix BMP detection by not returning early during BME address scans. #9935
- Enforce infrastructure-role minimums even when scaling is disabled. #9937
- Fix traceroute hop rendering for `ffff` / unknown-dB hops. #9945
- Fix NodeInfo suppression so it only applies to external requests. #9947
- Enable touch-to-backlight on T-Echo, not just T-Echo Plus. #9953
- Prevent licensed users from rebroadcasting packets to or from unlicensed users. #9958
- Add the `heltec_mesh_node_t096` board. #9960
- Add Cardputer-Adv I2S audio support. #9963
- Fix the Cyrillic OLED double-space issue. #9971
- Add `LED_BUILTIN` for `tlora_v1`. #9973
- Add a timeout for PPA uploads. #9989
- Exclude the web server, Paxcounter, and a few other components on original ESP32 boards to avoid IRAM overflow. #10005
- Rework External Notifications logic. #10006
- Improve STM32WL support. #10015
- Configure NFC pins as GPIO for older bootloaders. #10016
- Fix `TransmitHistory` epoch handling. #10017
- Inherit `build_unflags` for `wio-sdk-wm1110`. #10034
- Remove PSRAM from `tbeam` boards to reclaim IRAM. #10036
- Move `t5s3_epaper_inkhud` to `extra`. #10037

## ⚙️ Dependencies

- Update `meshtastic-esp32_https_server` to digest `b78f12c`. #9851
- Update `meshtastic/device-ui` through digests `622b034`, `f36d2a9`, `7b1485b`, and `1897dd1`. #9864 #9940 #10023 #10044 #10050
- Update `GxEPD2` to `v1.6.8`. #9918
- Update `pnpm/action-setup` to `v5`. #9926
- Update `dorny/test-reporter` to `v3`. #9981
- Clean up LewisHe library references and dependency matching, and tighten Renovate scheduling. #10007 #10008 #10039
- Update `Adafruit_BME680` to `v2.0.6`. #10009

**Full Changelog**: https://github.com/meshtastic/firmware/compare/v2.7.20.6658ec2...v2.7.21.1370b23
