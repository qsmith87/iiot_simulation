Project Overview

The project simulates an IIoT environment with:





Sensor Data Simulation: Generates random temperature (20–25°C) and humidity (30–50%) data.



Protocols:





MQTT: Publishes data to a Mosquitto broker using a pub/sub model.



CoAP: Sends data to a custom CoAP server using REST-like requests.



OPC UA: Hosts a server with readable temperature and humidity variables.



Visualization: Displays real-time plots of sensor data for each protocol.



Comparison Report: Analyzes MQTT, CoAP, and OPC UA based on latency, scalability, security, and use cases.

Prerequisites





Python: 3.8 or higher



Mosquitto MQTT Broker: Download from https://mosquitto.org/



LaTeX Distribution: TeX Live or similar for compiling the report



Git: For cloning the repository



Code Editor: Visual Studio Code recommended



Screen Recording Tool: OBS Studio or similar for visualization_demo.mp4

Setup Instructions





Clone the Repository:

git clone https://github.com/yourusername/iiot_simulation.git
cd iiot_simulation

Replace https://github.com/yourusername/iiot_simulation.git with your repository URL.



Set Up Virtual Environment:

python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows



Install Dependencies:

pip install -r requirements.txt



Install Mosquitto:





Follow instructions at https://mosquitto.org/ for your operating system.



Verify Mosquitto runs on localhost:1883.



Create Visualizations Directory:

mkdir visualizations

Running the Simulation

Run each command in a separate terminal after activating the virtual environment.





Start Mosquitto Broker:

mosquitto



Start CoAP Server:

python coap_server.py



Run Sensor Simulations:

python mqtt_sensor_simulation.py
python coap_sensor_simulation.py
python opcua_sensor_simulation.py



Run Visualization Scripts:

python mqtt_data_visualization.py
python coap_data_visualization.py
python opcua_data_visualization.py
