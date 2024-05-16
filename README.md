# Dissertation Project Source Code
This project is meant for Linux VMs. It was made for a server and three client machines.

## Requirements
### Python Libraries
This project uses additional Python libraries.
The required Python libraries can be found in the **requirements.txt** file.

The libraries can be installed using the following command:
```
pip install -r requirements.txt
```

### Opening Ports
Port **5555** must be open for ingress and egress UDP/TCP traffic on all machines for the SVM cluster. Port **5556** must be opened for the RF cluster.

### Changing Server IPs
The server IP must be changed for each client in their respective client-_**no**_.py files for each cluster.

### Datasets
The CSE-CIC-IDS2018 was deleted as it was very large. Please download it as per the instructions here, https://www.unb.ca/cic/datasets/ids-2018.html. Add the files to the "dataset" folder of Client 2.
If the original datasets were too large, they were kept in their zip archive form. Unzip them if you wish to run any "making datasets" Jupyter Notebooks.


## Running the Project
### Archives
The `code.zip` archive contains the archives of each machine required. Unzip the `code.zip` archive and transfer the other zip files to their assigned machines. Unzip those archives on the target machines.

### Jupyter Notebooks
The Jupyer Notebooks can be run without any preparation.

### Federated Learning Files
The federated learning files can be find in the "**FL**" folder for each machine.

#### Server
The server can be run using the `python3` command below. A separate `server.py` file can be found in each of the federated ML models' folder. Please run the appropriate one for the cluster that is being run.
```
python3 server.py
```

#### Clients
Each client must be run using the Bash script found in each of their respecive FL folders. 
```
./client.sh
 ```
