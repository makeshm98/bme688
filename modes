# BME688 Sensor Measurement Modes

The BME688 sensor supports various measurement modes, including forced mode, parallel mode, and sequential mode. Each mode offers different capabilities and is suitable for specific application requirements.

## 1. Forced Mode

Forced mode, also known as on-demand mode, is a measurement mode where sensor measurements are triggered explicitly by the user. In forced mode, the sensor remains in a low-power state until a measurement command is issued. Once triggered, the sensor performs a single measurement cycle and then returns to the low-power state.

### Workflow:

1. **Initialization:** Configure the sensor for forced mode operation and set the desired measurement parameters (e.g., oversampling rates, filter settings).
2. **Trigger Measurement:** Send a command to the sensor to initiate a measurement cycle. The sensor will perform a single measurement of temperature, pressure, humidity, and gas resistance based on the configured settings.
3. **Read Sensor Data:** After the measurement cycle is complete, read the sensor data registers to retrieve the measured values.
4. **Data Processing:** Process the acquired sensor data as needed (e.g., apply compensation algorithms, convert raw data to physical quantities).
5. **Optional:** Repeat the measurement process if additional measurements are required.

Forced mode is suitable for applications where periodic measurements are sufficient, and power consumption needs to be minimized during idle periods.

## 2. Parallel Mode

Parallel mode, also known as parallel sampling, is a measurement mode where multiple sensors operate simultaneously and independently. In parallel mode, each sensor performs its measurements concurrently without waiting for other sensors to complete their measurements.

### Workflow:

1. **Initialization:** Configure each sensor for parallel mode operation and set the desired measurement parameters independently for each sensor.
2. **Trigger Measurements:** Send measurement commands to all sensors simultaneously to initiate measurement cycles.
3. **Read Sensor Data:** After the measurement cycles are complete, read the sensor data registers for each sensor to retrieve the measured values.
4. **Data Processing:** Process the acquired sensor data from each sensor as needed.
5. **Optional:** Repeat the measurement process if additional measurements are required.

Parallel mode is suitable for applications that require synchronous measurements from multiple sensors or when sensor measurements need to be independent of each other.

## 3. Sequential Mode

Sequential mode, also known as sequential sampling, is a measurement mode where multiple sensors operate sequentially in a predefined sequence. In sequential mode, each sensor performs its measurements one after the other in a predefined order.

### Workflow:

1. **Initialization:** Configure each sensor for sequential mode operation and set the desired measurement parameters independently for each sensor.
2. **Trigger Sequential Measurements:** Send measurement commands to the first sensor in the sequence to initiate its measurement cycle.
3. **Wait for Completion:** Wait for the first sensor to complete its measurement cycle before triggering the next sensor in the sequence.
4. **Read Sensor Data:** After each sensor completes its measurement cycle, read the sensor data registers to retrieve the measured values.
5. **Data Processing:** Process the acquired sensor data from each sensor as needed.
6. **Repeat:** Repeat the sequential measurement process for subsequent cycles if necessary.

Sequential mode is suitable for applications that require measurements from multiple sensors in a specific order or when sensor measurements need to be coordinated.

Each mode offers distinct advantages and is chosen based on the specific requirements of the application, such as power consumption, synchronization, and measurement frequency. Consult the sensor datasheet and application notes for detailed information on implementing each mode and optimizing sensor performance.
