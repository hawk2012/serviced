# serviced
Script for service creation. Written by me in Python.

The script is designed to create Systemd service files based on the parameters entered by the user. It requests the following data from the user:

The name of the service (for example, my_service)
The command to start the service (for example, /path/to/my_script.sh )
Description of the service (brief explanation of the purpose of the service)
The process group (the user group under which the process will run)
The user (the user under which the command will run)
The working directory (the directory where the command will be run)
Based on this data, the script creates a .service file in the /etc/systemd/system/ directory, which can then be used to manage the service through Systemd. The script also displays messages about the progress and successful creation of the service.

Thus, this tool simplifies the creation of new service files for Systemd, allowing you to quickly configure the automatic launch of applications or scripts when the system boots.

This script can be saved anywhere and run through the Python interpreter (`sudo python3 serviced`). If you want to use it as a system utility, you will need to set the execution rights and place it in the appropriate directory, for example, `/usr/local/bin` (`sudo mv serviced /usr/local/bin` or `sudo mv serviced /usr/bin`).
