# Tines_automation

Tines Automation with Wazuh
We will automate Tines with Wazuh using a webhook and integrate it with our favorite ticketing system.

Step 1: Configure Webhook in Wazuh
First, drag and drop the webhook, copy the link, and add an integration block to the ossec.conf file in Wazuh. You can locate this configuration file in your Wazuh instance.

![image](https://github.com/user-attachments/assets/ce0833cb-3e49-4e6b-b411-5fbf654b47c2)

![image](https://github.com/user-attachments/assets/c47572ed-b640-411d-8318-a9107d39a538)

![image](https://github.com/user-attachments/assets/450e1202-1330-470f-b158-4ae6a0ec5d1c)


Step 2: Verify Alerts
Once configured, you should immediately start seeing alerts. In our case, we observed four alerts because we only have one agent installed. Currently, we are using the Wazuh OVA (I was too lazy to install a full instance 😅). You can download the Wazuh OVA from the following link:

link to wazuh's ova
https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html


![image](https://github.com/user-attachments/assets/8e3e5242-0480-41e2-bd11-0b31a8644d52)

Step 3: Customize Wazuh Alerts
You can customize Wazuh alerts to send emails directly to your inbox.

![image](https://github.com/user-attachments/assets/e563259a-fc77-4ef8-92f1-e1f682169a6f)
![image](https://github.com/user-attachments/assets/12f371dd-50b5-49b2-97a7-6abd10108297)


Step 4: Add Transform Arguments
Next, add a transform argument. This feature allows you to control the throttle, delay incoming events, and more. Explore the other available options to further customize your setup.
![image](https://github.com/user-attachments/assets/2153995f-3b62-4ac4-aaa9-2c274823b938)


Step 5: Configure HTTP Request
The HTTP request feature lets you route traffic to a specified location. This is where we integrate our ticketing system.
![image](https://github.com/user-attachments/assets/dffbbeca-e6e0-4262-b0b3-e514adbfad70)

Step 6: Add API Key
Before integrating, you must add an API key. Navigate to the main menu, select Settings, and then choose API.

![image](https://github.com/user-attachments/assets/78be534a-5c87-4214-a5bb-95cc0ea508f7)

After adding the API key, you can navigate to your ticketing system and add the URL to complete the integration.

let's jump over to https://github.com/RottenCybersecurity/Tines_TicketSystem to see what this looks like!
