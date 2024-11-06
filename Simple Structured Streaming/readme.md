#Simple Structured Streaming
1. Povision ADLS Gen2 and create a container
2. Create your mount point in databricks
This project does not cover how to setup ADLS Gen2 or create mount point you need to figure out
Lets focus on creating a simple structured straming data pipeline
Steps:
1. Create directory structure in Azure ADLS Gen2
![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/over_directory_structure.png
 "ADLS Gen2 Directory Structure")

#input data here

![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/raw_container.png
 "ADLS Gen2 Directory Structure")
 
2. refer notebook for location of input, output, checkpoint along with mounts points and how readsteam and writestream is written

[Notebook here](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/very%20simple%20first%20level%20streamig%20use%20case.ipynb)  

4. here is the output generate
![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/processed_data_here.png
 "ADLS Gen2 Directory Structure")
5. Here is the checkpoint directory structure after running straming procesess
![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/checkpoint_container.png
 "ADLS Gen2 Directory Structure")

#Inside Checkpoint directory

![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/checkpoint_commits.png
 "ADLS Gen2 Checkpoint Directory")

 ![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/checkpoint_version.png
 "ADLS Gen2 Checkpoint Directory")

 
 ![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/checkpoint_offsetsstate_store.png
 "ADLS Gen2 Checkpoint Directory")
 
![text if the image fails to load](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/metadata.png
 "ADLS Gen2 Directory Structure")
 
[Here is how metadata id keeps track of raw-data schema](https://github.com/saleemshad/Streaning_Data_Engineering/blob/main/Simple%20Structured%20Streaming/checkpoint_metadata_id.pdf)  
 
