# Internet of Things, Politecnico di Milano (2025–2026)

Reports for the four challenges of the Internet of Things course, from energy budgets on an ESP32 node to
protocol analysis, Node-RED flows and MAC-layer sizing. Each folder has the LaTeX source and the compiled
`report.pdf`.

| Challenge | Topic | Highlights |
|---|---|---|
| [1 · Energy analysis](challenge-1/energy-analysis) | ESP32 occupancy/light node simulated in Wokwi | Per-phase timing and energy from measured cycles, battery-life model (~2.5 days), and a delta-reporting redesign with RTC memory that roughly halves energy per skipped cycle |
| [1 · Ex. 4](challenge-1/ex-4-radio-energy) | Direct vs multi-hop radio energy | First-order radio model over 40 m: multi-hop chosen to spare the battery-powered sensor |
| [2 · Protocol analysis](challenge-2/coap-mqtt-pcap-analysis) | CoAP and MQTT on real captures | Eight questions answered from pcap files with tshark, grep and awk |
| [2 · Energy](challenge-2/coap-vs-mqtt-energy) | CoAP CON vs MQTT QoS 1 | Energy for an hour of readings through a gateway; MQTT with a persistent session picked |
| [3 · Node-RED](challenge-3/node-red-zigbee) | ZigBee packet pipeline over MQTT | Node-RED flow with ID generation, a 200-message gate, ZCL and Link Status routing, CSV logs and ThingSpeak charts |
| [3 · LoRaWAN](challenge-3/lorawan-sizing) | Class A network sizing | Largest airtime for 40 nodes at 75% success, leading to SF7 |
| [4 · Part 1](challenge-4/part-1-ieee802154-cfp) | IEEE 802.15.4 beacon-enabled CFP | Slot sizing for three vibration nodes and room for four more |
| [4 · Part 2](challenge-4/part-2-ble-beacon) | BLE beacon firmware redesign | Event-driven firmware (wake-on-motion, in-mouth check) with 86–89% less radio charge |
| [4 · Part 3](challenge-4/part-3-rfid-aloha) | RFID dynamic frame ALOHA | Identification efficiency for 4 tags across initial frame sizes |

Challenge 1 is individual work by Raul Agolli. Challenges 2 to 4 were done with **Gabriele Lorenzo Singe**.

To rebuild a report: `tectonic main.tex` (or `pdflatex main.tex`) in its folder.
