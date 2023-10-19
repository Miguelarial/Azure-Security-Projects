Azure Security Project

This repository documents the steps taken to set up Azure Sentinel SIEM, a log analytics workspace, and integrate geolocation data to observe and map failed RDP attempts on a virtual machine.

Features:
- Azure Virtual Machine Setup: Detailed documentation on creating and configuring a VM for log observation.
- Comprehensive Log Analytics: Utilization of Azure's Log Analytics Workspace for detailed log scrutiny.
- Microsoft Sentinel Integration: Guidance on integrating and setting up Microsoft Sentinel for enhanced security monitoring.
- Real-time Log Collection: Steps on connecting the VM to the Log Analytics Workspace for continuous log collection.
- Geolocation Integration: Process to extract geolocation data from RDP attempt logs for mapping purposes.
- Custom Log Creation: Instructions on how to create and manage custom logs within Azure's Log Analytics Workspace.
- Sentinel Geographical Mapping: Utilize Azure Sentinel's mapping feature to visually represent RDP attempt origins based on geolocation data.

Project Steps:

1. Virtual Machine Creation
   - Set up a virtual machine to observe and gather logs related to RDP attempts.

2. Firewall Configuration
   - Allow all incoming and outgoing connections in the firewall for the initial setup.

3. Log Analytics Workspace
   - Establish a dedicated workspace for gathering and analyzing logs.

4. Integration with Security Center
   - Enable the gathering of VM logs within Azure's Security Center.

5. VM and Log Analytics Connection
   - Integrate the virtual machine with the log analytics workspace to enable real-time log collection.

6. Microsoft Sentinel Setup
   - Set up Microsoft Sentinel and log into the virtual machine using remote desktop.

7. Event Viewer Observations
   - Observe the event viewer logs on the virtual machine to monitor RDP attempts and other events.

8. Windows Firewall Configuration
   - Disable the Windows Firewall on the VM to ensure uninterrupted log gathering.

9. PowerShell Script Download
   - Download the necessary PowerShell script that aids in extracting and processing log data.

10. Geolocation API
   - Acquire an API key from geolocation.io to enable the extraction of geolocation data for IP addresses.

11. Geolocation Script Execution
   - Execute the provided script to gather geolocation data about potential attackers based on the logs.

12. Custom Log Creation
   - Set up a custom log within the Log Analytics Workspace to bring in the processed and raw log data.

13. Custom Field Extractions
   - Extract custom fields from the raw log data to enhance readability and analysis.

14. Testing
   - Test the data extraction and logging mechanisms to ensure accuracy and completeness.

15. Sentinel Mapping
   - Utilize Azure Sentinel's mapping features to plot the latitude and longitude data of RDP attempt origins.

Important Notes:
- Ensure that you secure your VM and only disable firewalls temporarily for testing purposes. Always prioritize security in live environments.
- Make necessary adjustments based on the specific configurations and versions of tools you are using.

Contributions:
This project was created and documented by Mike Chibuzo Arihalam. For any queries or suggestions, please raise an issue or reach out directly.


