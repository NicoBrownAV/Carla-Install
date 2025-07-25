# Carla-Install
## CARLA 0.9.15 Ubuntu 22.04 Installation 

### The following requirements should be fulfilled before installing CARLA:

- System requirements: CARLA is built for Windows and Linux systems.
- An adequate GPU: CARLA aims for realistic simulations, so the server needs at least a 6 GB GPU although we would recommend 8 GB. A dedicated GPU is highly recommended for machine learning.
    - I recommend Using a GPU with at least 12GB of VRAM and have at least 32GM of RAM for your CPU. 
- Disk space: CARLA will use about 20 GB of space.
- Python: Python is the main scripting language in CARLA. CARLA supports Python 2.7 and Python 3 on Linux.
- Pip: Some installation methods of the CARLA client library require pip or pip3 (depending on your Python version) version 20.3 or higher. To check your pip version:

#### Step 1: update before every installation
    'sudo apt update'
  
#### Step 2: upgrade if needed
    'sudo apt upgrade'
  
#### Step 3: pip installtion (Check the version you have of pip if you have it already installed)
    'pip -V' or 'pip3 -V'    

##### If pip is not installed:
    'sudo apt install python3-pip'

##### Upgrade if needed:
    "pip3 install --upgrade pip' # for python 3

#### Step 4: Install pygame numpy
    "pip3 install --user pygame numpy"

#### Step 5: Download the file for installation from Github
Download CARLA 0.9.15 (*.tar.gz file)
- https://github.com/carla-simulator/carla/blob/master/Docs/download.md

#### Step 6: Create a directory for Carla Simulator and extract the file there for installtion
- Make the folder using the UI (command line: mk dir name_of_folder)
- Move the downloaded *.tar file to the new directory (command line: mv CARLA_0.9.15.tar.gz /path_to_new_dir) *in the downloads directory
- Extract the *.tar file in new dir (command line: tar -xvzf CARLA_0.9.15.tar.gz)

#### Step 7: Build Carla : This builds the client for compability with python 3.10. * make sure you only have python 3.10. * this does not need an egg file
    'pip install carla'

#### Step 8: Additional Maps:
You can download the additional maps. Make sure to merge with the content folder in CarlaUE4 folder the after building Carla  

#### Step 9: Start Carla: From the Carla dir with the *.sh file:
    './CarlaUE4.sh'

#### Step10: Navigate to PythonAPI directory for installing python requirment for using the built-in python examples. 
    'python3 -m pip install -r requirement.txt'

#### Examples Folder in Python API directory
    'python3 generate_traffic.py'
    'python3 manual_control.py'


 
