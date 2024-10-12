### Table 2: IoT Fridge Features and Description

| Feature              | Description                                                                                                       |
| -------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `ts`                 | Timestamp of sensor reading data                                                                                  |
| `date`               | Date of logging sensor's telemetry data                                                                           |
| `time`               | Time of logging sensor's telemetry data                                                                           |
| `fridge_temperature` | Temperature measurement of a fridge sensor                                                                        |
| `temp_condition`     | Temperature conditions of a fridge sensor, where temperature is high or low based on a predefined threshold value |
| `label`              | Identify normal and attack records, where '0' indicates normal and '1' indicates attacks                          |
| `type`               | A tag with normal or attack sub-classes, such as DoS, DDoS and backdoor attacks                                   |
### Table 3: IoT Garage Door Features and Description

| Tính năng      | Mô tả                                                                                    |
| -------------- | ---------------------------------------------------------------------------------------- |
| `ts`           | Timestamp of sensor reading data                                                         |
| `date`         | Date of logging sensor's telemetry data                                                  |
| `time`         | Time of logging sensor's telemetry data                                                  |
| `door_state`   | State of a door sensor where the door is closed or open                                  |
| `phone_signal` | State of receiving the door signal on a phone where the signal is true or false          |
| `label`        | Identify normal and attack records, where '0' indicates normal and '1' indicates attacks |
| `type`         | A tag with normal or attack sub-classes, such as DoS, DDoS and backdoor attacks          |

### Table 4: IoT GPS Tracker Features and Description

| Tính năng   | Mô tả                                                                                    |
| ----------- | ---------------------------------------------------------------------------------------- |
| `ts`        | Timestamp of sensor reading data                                                         |
| `date`      | Date of logging sensor's telemetry data                                                  |
| `time`      | Time of logging sensor's telemetry data                                                  |
| `latitude`  | Latitude value of GPS tracker sensor                                                     |
| `longitude` | Longitude value of GPS tracker sensor                                                    |
| `label`     | Identify normal and attack records, where '0' indicates normal and '1' indicates attacks |
| `type`      | A tag with normal or attack sub-classes, such as DoS, DDoS and backdoor attacks          |
### Table 5: IoT Motion Light Features and Description

| Tính năng       | Mô tả                                                                                         |
| --------------- | --------------------------------------------------------------------------------------------- |
| `ts`            | Timestamp of sensor reading data                                                              |
| `date`          | Date of logging sensor's telemetry data                                                       |
| `time`          | Time of logging sensor's telemetry data                                                       |
| `motion_status` | Status of a motion sensor is either (on or off) where 1 indicates "on", and 0 indicates "off" |
| `light_status`  | Status of a light sensor is either on or off                                                  |
| `label`         | Identify normal and attack records, where '0' indicates normal and '1' indicates attacks      |
| `type`          | A tag with normal or attack sub-classes, such as DoS, DDoS and backdoor attacks               |
### Table 6: IoT Modbus Features and Description

| Tính năng                   | Mô tả                                                                                    |
| --------------------------- | ---------------------------------------------------------------------------------------- |
| `ts`                        | Timestamp of sensor reading data                                                         |
| `date`                      | Date of logging Modbus register's data                                                   |
| `time`                      | Time of logging Modbus register's data                                                   |
| `FC1_Read_Input_Register`   | Modbus function code that is responsible for reading an input register                   |
| `FC2_Read_Discrete_Value`   | Modbus function code that is in charge of reading a discrete value                       |
| `FC3_Read_Holding_Register` | Modbus function code that is responsible for reading a holding register                  |
| `FC4_Read_Coil`             | Modbus function code that is responsible for reading a coil                              |
| `label`                     | Identify normal and attack records, where '0' indicates normal and '1' indicates attacks |
| `type`                      | A tag with normal or attack sub-classes, such as DoS, DDoS and backdoor attacks          |
### Table 7: IoT Thermostat Features and Description

| Feature               | Description                                                                              |
| --------------------- | ---------------------------------------------------------------------------------------- |
| `ts`                  | Timestamp of sensor reading data                                                         |
| `date`                | Date of logging sensor's telemetry data                                                  |
| `time`                | Time of logging sensor's telemetry data                                                  |
| `current_temperature` | Current Temperature reading of a thermostat sensor                                       |
| `thermostat_status`   | Status of a thermostat sensor is either on or off                                        |
| `label`               | Identify normal and attack records, where '0' indicates normal and '1' indicates attacks |
| `type`                | A tag with normal or attack sub-classes, such as DoS, DDoS and backdoor attacks          |
### Table 8: IoT Weather Features and Description

| Feature       | Description                                                                              |
| ------------- | ---------------------------------------------------------------------------------------- |
| `ts`          | Timestamp of sensor reading data                                                         |
| `date`        | Date of logging sensor's telemetry data                                                  |
| `time`        | Time of logging sensor's telemetry data                                                  |
| `temperature` | Temperature measurements of a weather sensor                                             |
| `pressure`    | Pressure readings of a weather sensor                                                    |
| `humidity`    | Humidity readings of a weather sensor                                                    |
| `label`       | Identify normal and attack records, where '0' indicates normal and '1' indicates attacks |
| `type`        | A tag with normal or attack sub-classes, such as DoS, DDoS and backdoor attacks          |