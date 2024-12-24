# Advent of Cyber 2024

## Communication Protocols - MQTT & Wireshark

- Reviwed how IoT devices (e.g. HVAC units, smart lights, etc.) communicate
- MQTT - Message Queuing Telemetry Transport, a language very commonly used in IoT devices for communication purposes. It works on a publish/subscribe model, where any client device can publish messages, and other client devices can subscribe to the messages if they are related to a topic of interest

### Room Example

- Went over how to use wireshark to review MQTT traffic from the test HVAC and smart light devices
- Found the topic that is used to turn on lights and then used `mosquitto_pub` to mimic the controller to activate the lights to find the flag
    - E.g. Used wireshark to find the appropraite topic ID and then used the message of `on` to mimick the request
    ```bash
    mosquitto_pub -h localhost -t "d2FyZXZpbGxl/Y2hyaXN0bWFzbGlnaHRz" -m "on"
    ```
