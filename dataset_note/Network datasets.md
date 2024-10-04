### Overview
- Raw_datasets/Raw_Network_dataset = network_dataset_pcap + network_dataset_Bro
	- network_dataset_pcap = raw packets of normal and attack events (**pcap**) using the #netsniff-ng tool
	- network_dataset_Bro = the **log** and **csv** extracted from **pcap** using #Zeek . The **csv** files include the **data features** from the **log** file 
- Processed_datasets/Processed_Network_dataset = 23 **csv** files. Each has 44 attributes and 2 attributes of the class label and types either *normal* or *attack* category
- SecurityEvents_GroundTruth_datasets/Security Events_Network_datasets = ground truth tables used for labeling
	- The IP addresses of the offensive systems and their timestamps were logged to accurately label records
- Train_Test_datasets/Train_Test_Network_dataset = a **csv** includes a subset of the entire attack types and normal records. *suggested to be used for evaluating new AI-based cy bersecurity solutions*
- Description_stats_datasets/Description_stats_Network_dataset = data feature descriptions + number of recorded included