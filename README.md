# Tines_automation

We're going to be automating tines w/ Wazuh using a Webhook and adding our favorite ticketing system 

First we have to drag and drop our webhook, grab the link and add an integration block in the ossec.conf file that we can locate in wazuh

![image](https://github.com/user-attachments/assets/ce0833cb-3e49-4e6b-b411-5fbf654b47c2)

![image](https://github.com/user-attachments/assets/c47572ed-b640-411d-8318-a9107d39a538)

![image](https://github.com/user-attachments/assets/450e1202-1330-470f-b158-4ae6a0ec5d1c)


One that's done we should imidiatelly start seeing alerts
so far 4 since we only have one agent installed and we're currently using Wazuh OVA -i was too lazy to install a full instance- lol
link to wazuh's ova
https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html


![image](https://github.com/user-attachments/assets/8e3e5242-0480-41e2-bd11-0b31a8644d52)

We can now customize our wazuh alerts to have email sent to us directly

![image](https://github.com/user-attachments/assets/e563259a-fc77-4ef8-92f1-e1f682169a6f)
![image](https://github.com/user-attachments/assets/12f371dd-50b5-49b2-97a7-6abd10108297)


Now lets keep going. We've added a transform argument. Here we can control throttle, delay our incoming events. There's other features here as well to play with so try it out.

![image](https://github.com/user-attachments/assets/2153995f-3b62-4ac4-aaa9-2c274823b938)


Http request will allow us to drive our traffic to a specified location. This is where our ticketing system comes in

![image](https://github.com/user-attachments/assets/dffbbeca-e6e0-4262-b0b3-e514adbfad70)

before we integrate we'll have to add a key
so navigate to the main menu and select settings and api

![image](https://github.com/user-attachments/assets/78be534a-5c87-4214-a5bb-95cc0ea508f7)

once you added your API key. 
We can navigate and add the URL
