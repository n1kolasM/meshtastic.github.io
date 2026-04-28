## 🚀 Enhancements

- Reduce key duplication by enabling hardware RNG by @Komzpa in https://github.com/meshtastic/firmware/pull/8803
- Feat(stm32): Add STM32 ADC support to AnalogBatteryLevel by @ndoo in https://github.com/meshtastic/firmware/pull/9369
- Hash table index for O(1) packet history lookups by @rcd in https://github.com/meshtastic/firmware/pull/9499
- BaseUI: Implementation of Status Message for Favorite and NodeList views by @Xaositek in https://github.com/meshtastic/firmware/pull/9504
- Add RADIOLIB_EXCLUDE_LR2021 in places that excluded LR11x0 by @fifieldt in https://github.com/meshtastic/firmware/pull/10112
- Feat(Power): support EXT_PWR_DETECT_MODE & EXT_PWR_DETECT_VAL, simplify EXT_PWR_DETECT by @ndoo in https://github.com/meshtastic/firmware/pull/10140
- Compass improvements/refactoring by @HarukiToreda in https://github.com/meshtastic/firmware/pull/10166
- Test PR to remove LED_BUILTIN by @jp-bennett in https://github.com/meshtastic/firmware/pull/10179
- No longer need undefines, thanks to #10179 by @jp-bennett in https://github.com/meshtastic/firmware/pull/10180
- Add MCP server for interacting with meshtastic devices and testing framework / TUI by @thebentern in https://github.com/meshtastic/firmware/pull/10194
- BaseUI: Nodelist screen/favorite screen cleanup by @HarukiToreda in https://github.com/meshtastic/firmware/pull/10197
- Add authoring guide for native unit tests in README.md by @NomDeTom in https://github.com/meshtastic/firmware/pull/10201
- Add USB camera and uhubctl support for new test suite. Also included some bug fixes by @thebentern in https://github.com/meshtastic/firmware/pull/10204
- Add encryption overview to agent instructions in AGENTS.md by @thebentern in https://github.com/meshtastic/firmware/pull/10207
- BaseUI: Color Support for TFT Nodes by @HarukiToreda in https://github.com/meshtastic/firmware/pull/10233
- Improve options to align to names of UI options by @Xaositek in https://github.com/meshtastic/firmware/pull/10240
- Finish evil merge cleanup by @jp-bennett in https://github.com/meshtastic/firmware/pull/10253
- Router: demote cross-channel decrypt failures from ERROR to DEBUG by @nightjoker7 in https://github.com/meshtastic/firmware/pull/10259
- NimbleBluetooth misc cleanups by @cpatulea in https://github.com/meshtastic/firmware/pull/10264
- We have HardwareRNG, let's use it! by @jp-bennett in https://github.com/meshtastic/firmware/pull/10274
- Standardize PMU IRQ handling and enable power button cancel on tbeam-s3 by @jp-bennett in https://github.com/meshtastic/firmware/pull/10285
- InkHUD: Add full touch support to T5s3 by @HarukiToreda in https://github.com/meshtastic/firmware/pull/10286
- Fix(inkhud): scale map applet markers with font size by @giannoug in https://github.com/meshtastic/firmware/pull/10288
- Add search duration check for exceeding 15 minutes by @jp-bennett in https://github.com/meshtastic/firmware/pull/10293
- Native MacOS hello world by @thebentern in https://github.com/meshtastic/firmware/pull/10309

## 🐛 Bug fixes and maintenance

- T-Watch S3 Power button managment by @Emanuele-Mb in https://github.com/meshtastic/firmware/pull/9855
- Fix(native): implement BinarySemaphorePosix with proper pthread synchronization by @iannucci in https://github.com/meshtastic/firmware/pull/9895
- Fix/feat(stm32/russell): Serial2 build fix and BME680 support by @ndoo in https://github.com/meshtastic/firmware/pull/10097
- Fix last cppcheck issue by @caveman99 in https://github.com/meshtastic/firmware/pull/10154
- Fix heap blowout on TBeams by @thebentern in https://github.com/meshtastic/firmware/pull/10155
- Add PortduinoSetOptions to overwrite the realhardware bool by @jp-bennett in https://github.com/meshtastic/firmware/pull/10157
- Support for Spreading Factors 5 and 6 on compatible radios by @derpyspike in https://github.com/meshtastic/firmware/pull/10160
- Add meshtasticd config for Luckfox Pico Max Waveshare Pico LoRa HAT by @Ruledo in https://github.com/meshtastic/firmware/pull/10175
- Fix(Power): refactor EXT_CHRG_DETECT to compile-time macros with pull-mode inference by @ndoo in https://github.com/meshtastic/firmware/pull/10191
- Prompt markdownlint md040 fix for new prompts. by @h3lix1 in https://github.com/meshtastic/firmware/pull/10199
- Feat(t5s3-epaper): add InkHUD port for LilyGo T5 E-Paper S3 Pro by @giannoug in https://github.com/meshtastic/firmware/pull/10211
- Filter out SKIPPED tests in PlatformIO output to improve log cla… by @NomDeTom in https://github.com/meshtastic/firmware/pull/10214
- SX126x: re-apply 0x8B5 register in resetAGC() to preserve RX sensitivity by @nightjoker7 in https://github.com/meshtastic/firmware/pull/10219
- Detach power interrupts for sleep by @jp-bennett in https://github.com/meshtastic/firmware/pull/10230
- T watch pinfix by @jp-bennett in https://github.com/meshtastic/firmware/pull/10231
- T5s3-epaper: Move variant.cpp -> extra_variants/variant.cpp by @vidplace7 in https://github.com/meshtastic/firmware/pull/10241
- Cardputer-adv: Move variant.cpp -> extra_variants/variant.cpp by @vidplace7 in https://github.com/meshtastic/firmware/pull/10242
- Fix INA226 detection for non-TI compatible chip (Silergy) by @theKorzh in https://github.com/meshtastic/firmware/pull/10247
- StoreForwardModule::historyAdd: memcpy source size, not buffer capacity by @nightjoker7 in https://github.com/meshtastic/firmware/pull/10250
- PositionModule::sendLostAndFoundText: use stack buffer, eliminate heap alloc by @nightjoker7 in https://github.com/meshtastic/firmware/pull/10251
- RadioLibInterface: clear static `instance` on destruction to prevent UAF by @nightjoker7 in https://github.com/meshtastic/firmware/pull/10254
- PhoneAPI: add missing tak_tag case + skip reserved gap in module-config iteration by @nightjoker7 in https://github.com/meshtastic/firmware/pull/10256
- Only enable wakeup via EXT_CHRG_DETECT if we shut down due to low power by @jp-bennett in https://github.com/meshtastic/firmware/pull/10263
- Add heltec-v4-r8 board by @Quency-D in https://github.com/meshtastic/firmware/pull/10268
- Fix example comment in airtime.h by @VBart in https://github.com/meshtastic/firmware/pull/10275
- Remove incorrect LED_STATE_ON definition for t-beam-s3 by @jp-bennett in https://github.com/meshtastic/firmware/pull/10280
- T5s3-epaper: Move variant.cpp -> extra_variants/variant.cpp ...again by @vidplace7 in https://github.com/meshtastic/firmware/pull/10297
- Fix(Router): localize p_encrypted to prevent recursive-overwrite leak by @nightjoker7 in https://github.com/meshtastic/firmware/pull/10311
- Actions: Build MacOS binary by @vidplace7 in https://github.com/meshtastic/firmware/pull/10319

## ⚙️ Dependencies

- Update platform-native digest to 71ed55b by @app/renovate in https://github.com/meshtastic/firmware/pull/10165
- Update meshtastic-st7789 digest to 92bae2e by @app/renovate in https://github.com/meshtastic/firmware/pull/10182
- Update meshtastic/device-ui digest to 5305670 by @app/renovate in https://github.com/meshtastic/firmware/pull/10183
- Update meshtastic/device-ui digest to 56e1da4 by @app/renovate in https://github.com/meshtastic/firmware/pull/10195
- Update GxEPD2 to v1.6.9 by @app/renovate in https://github.com/meshtastic/firmware/pull/10212
- Update LovyanGFX to v1.2.20 by @app/renovate in https://github.com/meshtastic/firmware/pull/10232
- Update meshtastic-esp8266-oled-ssd1306 digest to 6bfd1f1 by @app/renovate in https://github.com/meshtastic/firmware/pull/10277
- Update platform-native digest to 135b91e by @app/renovate in https://github.com/meshtastic/firmware/pull/10300
- Update meshtastic/device-ui digest to 7289329 by @app/renovate in https://github.com/meshtastic/firmware/pull/10313
- Update platform-native digest to 4ea5e09 by @app/renovate in https://github.com/meshtastic/firmware/pull/10314

**Full Changelog**: https://github.com/meshtastic/firmware/compare/v2.7.22.96dd647...v2.7.22.9f1b85c
