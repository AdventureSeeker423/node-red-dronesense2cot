<h1 align='center'>node-red-dronesense2cot</h1>

<p align='center'>A node red flow using Axon Air / Dronesense's API key in order to generate COT messages to be sent to a TAK server</p>

<p align='center'>Pulls drone location, details, and link to video stream.</p>

<p align='center'>Portions of this code are derived from https://github.com/dfpc-coe/etl-drone-sense licensed under the MIT License.</p>

<p align="center"><img src="https://github.com/AdventureSeeker423/node-red-dronesense2cot/blob/main/dronesense_flow_example.png?raw=true" alt="Dronesense Flow Example"></p>


## Pre-Requisites / Setup
1. Create an API Key through the [DroneSense / Axon Air website](https://accounts.dronesense.com/).
2. Once you login, navigate to the Admin page, then Settings at the top, and then Add New API Key.
3. Select Token Enabled, Video Enabled, and Allow All Missions or Select from the list the missions you want it to access.
4. Set an expiration date in the future and copy the API Key it gives you once pressing "Save."

## Deployment
1. Install [node-red-contrib-tak](https://flows.nodered.org/node/node-red-contrib-tak) if not already installed.
2. Import the node red flow.
3. Open the "Fetch Dronesense Devices" function and fill in your API TOKEN inside the quotations.
4. Edit your server connections by editing the "Dronesense" server connection node.  You will need to replace your host, port, and import your certificate/key files for the TLS connection.
