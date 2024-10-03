- Based on [this](/dataset_note/papers/TON_Network_dataset.pdf) paper
- Testbed was designed  based on interacting network and Iot/IIoT systems with **three layers** of **edge, fog and cloud** 
- Edge and Fog computing are similar in offering on-premise services like SaaS, PaaS, Iaas
![architecture](<img/proposed dynamic architecture.png>)
- *Edge layer*: includes physical devices and their OSs (sensors, smartphone, …). The Hypevisor tech of NSX-VMware as deployed on a host server at the edge layer to manage the VMs created at the fog layer
- *Fog layer*: programs and controls the VMs
- *Cloud layer*: The public HIVE MQTT dashboard enabled us to publish and subscribe to the telemetry data of IoT/IIoT services via configuration. The public PHP vulnerable website was used to simulate injection hacking events. The other cloud services were configured either in Microsoft Azure or AWS to transmit sensory data to the cloud and visualize their patterns
