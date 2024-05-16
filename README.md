# Dissertation Project Source Code
This project is meant for Linux VMs.

## Requirements
This project uses additional Python libraries.
The required Python libraries can be found in the **requirements.txt** file.

The libraries can be installed using the following command:
```
pip install -r requirements.txt
```

### Opening Ports
Port **5555** must be open for ingress and egress UDP/TCP traffic on all machines. 

## Running the Project
### Server
The server can be run using the `python3` command below. A separate `server.py` file can be found in each of the ML models' folder. Please run the appropriate one for the cluster that is being run.
```
python3 server.py
```

### Clients
Each client must be run using the Bash script found in each of their respecive FL folders. 
```
./client.sh
 ```
