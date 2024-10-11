- Based on [A new distributed architecture for evaluating AI-based security systems at the edge: Network TON_IoT datasets](https://www.researchgate.net/publication/352055999_A_new_distributed_architecture_for_evaluating_AI-based_security_systems_at_the_edge_Network_TON_IoT_datasets) paper


![architecture](<img/proposed dynamic architecture.png>)
### Edge layer: 
- Includes physical devices and their OSs (sensors, smartphone, …). 
- The #hypevisor tech of #NSX-VMware as deployed on a host server at the edge layer to manage the VMs created at the fog layer
### Fog layer
- Programs and controls the VMs using #NSX-VMware
### Cloud layer 
- The fog and edge services connected with:
	- The public HIVE MQTT dashboard
	- Public PHP vulnerable website
	- Cloud virtualization services
	- Cloud data analytics services
### SDN (Software-Defined Network)
- Using #NSX-VMware to provide an SDN solution
- #NSX-VMware  was deployed with #VMware-vSphere allowing the creation and management of various VMs to offer #Iot-IIot and network services
- *Controller*: #VMware-vSphere
	- ESXi vCenter Server: combines app on less hardware, offers a centralized platform for managing vSphere systems
	- Service controller platform: comprises single sign-on, licensing, and a certificate authority that secures accessing the controller.
- *Network*: #NSX-VMware + #NSX-vCloud 
	- Enables granular overlay networking and security at the hypervisor level
- *Storage*: #VM-vSAN
	- Provides simple hypervisor converged storage embedded in the hypervisor that can be co-located with the VNF workloads
### NFV (Network Function Virtualization)
- Allows the replacement of expensive hardware devices with software-based devices
- #NSX-vCloud enables creating and controlling several VMs for hacking and normal operations, allowing comm between the edge, fog and the cloud layers
- Fog NFV data cluster
	- ESXi hosts are the basic compute building blocks of vCloud NFV and NSX 
	- ESXi host resources are grouped together to create fog-nodes , called a cluster
### SO (Service Orchestration)
- SO = SDN + NVF???



![Configured Testbed of TON_IoT datasets](<img/Configured Testbed of TON_IoT datasets.png>)
### Fog nodes
- Orchestrated server: stimlate real production networks (DNS, FTP, HTTP,…) to generate various legitimate packets
- Middleware server: implementing #Iot-IIot  services linked them with the cloud layer to subcribe and publish telemetry data through #Node-RED
- Client Systems:
	- Two windows OSs used as remote web interface of the node-red and their traffic audit traces were logged
	- DVWA (damn vulnerable web app) used to make securtiy vulnerabilities using offensive systems
	- OWASP security Sphered VM has many sec-vuln against mobile and web app exploited using offensive sys
	- Same as Metasploitable 3
- Offensive sys:
	- Kali linux VMs (10 VMs) 
	- Scripts of hacking scenarios (scanning, backdoor, ransomware, DoS, DDoS, MITM, data injection, XSS, password violations) [Nine attack scenarios](/dataset_note/Nine%20attack%20scenarios.md)
- Data management: logger tools for raw and filtered data from OSs, #Iot-IIot , network
	- Window: Microsoft Data Collector Sets to store processes, CPUs, mems, hard disk
	- Linux: atop (same as Window)
	- Telemetry logger: installed in middleware VM
	- Network: 
		- the #netsniff-ng tool was used to capture the entire network packets in **pcap formats** 
		- The #Zeek Net work Security Monitor tool used to generate data features from the **pcap files**