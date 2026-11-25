# Hestia — Off-Grid Smart Home Hub & Local IoT Controller

Hestia is a local-first, 100% offline smart home dashboard and IoT automation controller for Android. Built with Kotlin, Jetpack Compose, and Material 3, Hestia connects directly to your local smart home network (Home Assistant Local REST/WS API, MQTT / Zigbee2MQTT, Tasmota, Philips Hue, Matter) over mDNS/Zeroconf — with zero cloud subscriptions, zero external telemetry, and zero mandatory accounts.

---

## 🏡 Key Features & Subsystem Breakdown

### 📡 Local IoT Protocols & Discovery (`iot-core`)
- **Current**: mDNS / Zeroconf local network device discovery, MQTT client connection, Home Assistant WebSocket API, and Philips Hue local hub discovery.
- **Planned / Roadmap**: Native Matter / Thread commissioning, CoAP / Kasa local protocol driver, and Tuya local key controller.

### 🎛️ Room Dashboards & Widgets (`dashboard`)
- **Current**: Customizable room grid dashboards, light brightness/color temperature sliders, climate thermostat controls, and media player tiles.
- **Planned / Roadmap**: Drag-and-drop floorplan map view, camera RTSP live view tiles, and customizable dashboard themes.

### ⚡ Local Automations & Scenes (`automations`)
- **Current**: Local scene triggers, schedule timers, and device state conditional rules.
- **Planned / Roadmap**: Sensor event graph builder, sunrise/sunset astronomical triggers, and presence detection rule engine.

---

## 🏗️ Architecture & Technology Stack

- **Platform**: Android 13+ (minSdk 33, targetSdk 37).
- **UI & Layout**: Kotlin, Jetpack Compose, Material 3.
- **Network Stack**: mDNS / Zeroconf (JmDNS), HiveMQ MQTT Client, WebSocket.
- **Privacy Contract**: Operates 100% on local Wi-Fi / LAN; zero external server pings.
- **Licensing**: AGPL-3.0.

---

## 🛠️ Building & Running

```bash
./gradlew assembleDebug
./gradlew installDebug
```

---

## 📜 License

Hestia is released under the **GNU Affero General Public License v3.0** (AGPL-3.0). See [`LICENSE`](LICENSE) for details.
