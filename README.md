# counterfit-lightsensor-led
Light sensor with LED signal (sent through MQTT) using CounterFit - Fake IoT Hardware | Python 3.9.13

Refer to [Microsoft IoT For Beginners](https://github.com/microsoft/IoT-For-Beginners/tree/main/1-getting-started/lessons/4-connect-internet)

# TL;DR
There are 2 folders:
- [Client](https://github.com/keira-n/counterfit-lightsensor-led/tree/main/nightlight_thing_whatever/nightlight) is for sending telemetry from the IoT device (CounterFit) to the MQTT broker and receiving commands.
- [Server](https://github.com/keira-n/counterfit-lightsensor-led/tree/main/nightlight_thing_whatever/nightlight_server) is for receiving telemetry from the MQTT broker and sending commands back.

## Running order: CounterFit > Client = Server
### CounterFit
1. Create a terminal

2. Activate the virtual environment 
`> .venv\Scripts\activate`

3. Launch CounterFit
`> counterfit`

4. Navigate to http://localhost:5000/

5. Create a light sensor
![image](https://github.com/user-attachments/assets/f71e658f-9ef9-407a-ad08-45a3159f73ed)

6. Set value to random (optional)

7. Create an LED actuator (pin 5)
> Change the colour if you want to :>

![image](https://github.com/user-attachments/assets/e1ebc4ba-821c-46c6-b34d-7a9814958747)

### Client (nightlight)
1. Create a new terminal

2. Activate the virtual environment
`> .venv\Scripts\activate`

3. Run the python app
`> py app.py`

### Open a new a new VSCode window for the Server (Easier to navigate)
1. Create a new terminal

2. Activate the virtual environment
`> .venv\Scripts\activate`

3. Run the python app
`> py app.py`

## What it should look like now
Client Terminal View
![ab](https://github.com/user-attachments/assets/70919e96-bf26-481e-8e9a-b225ef3270ae)

Server Terminal View
![ab2](https://github.com/user-attachments/assets/d53174aa-777c-449a-a90d-201747c6885c)

That's it :> ♥
