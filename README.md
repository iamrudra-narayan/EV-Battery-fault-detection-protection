# EV-Battery-fault-detection-protection


EV Health Indicator App 

https://iamrudra-narayan.github.io/EV-Battery-Fault-Detector/

<b>FAULT DETECTION & PROTECTION OF EV BATTERY</b>
Rudra Narayan Muduli, Laxmi Priya Das, Ankita Biswal, 7th Sem, Department of Electrical & Electronics Engineering
Prasantini Samal, Asst. Professor, Department of Electrical Engineering
  Abstract: - With the increase in electric vehicles (EVs) the demand for lithium-ion Batteries is also on the rise the battery management system (BMS) plays a vital role in electric vehicles lithium-ion batteries (LIB) power systems have been commonly used for energy storage in an electric vehicle we know that there is different type of fault in battery like temperature fault, current fault, etc. However, it is quite challenging to implement a real-time fault and protection scheme to ensure battery safety and performance. The paper presents a framework for real-time fault diagnosis and protection in a lithium-ion battery as the demand increases complexity also increases which play a major role. To minimize this, we have to develop the diagnosis, health Monitoring & prognosis (DHMP) model that assures the safety system. This proposed work takes the telemetry data through the real-time sensor in EV which is battery operated. Then the sensor data is visualized through the Internet of Things (IoT). The devices and technology used through the Internet of Things (IoT) which is monitored and measured in real-time. This work also enhanced and assisted with the root cause analysis that is used in EV systems.
Keywords: - PyCharm, Thing speak
1.INTRODUCTION
Many countries have invested a lot of money and resources to develop renewable energy and made a very useful technique which is Electric Vehicles (EVs). The purpose of electric vehicles is to save the environment & fossil fuels the battery management system plays a vital role in an electric vehicle. As we know the use of lithium-ion battery significantly increased day by day. Because the benefit of lithium-ion battery is their long lifespan, high energy density, and high-power density & although the lithium-ion battery has reported accident due to public concern safety features has decreased. This serious consequence is thermal runaway and fire or explosion. So, lithium-ion batteries have gone through many modifications to improve Their safety features.
Many factors affect the lithium-ion batteries such as collision and shock, vibration, deformation of metallic lithium plating, etc. some external battery faults are sensor faults, including temperature, voltage, and current faults, etc. Some common internal battery faults are overcharged, over-discharged, internal & external short circuits, overheating & thermal runaway. These are the dangerous consequences. 
By reducing this kind of problem, we found a solution that is fault detection & protection in lithium-ion batteries. In this paper, we consider temperature faults in lithium-ion batteries and find out the real-time fault data by using a programming language. So first we detect the temperature fault using a temperature sensor in the lithium-ion battery. Then send the real-time data to the cloud by Arduino UNO programming language after that we retrieve the real-time data from the cloud and so in the display.
II.COMPONENTS OF SOLAR TRACKING SYSTEM
First, we sense the temperature data of an EV battery and send or write the temperature data to the Thinkspeak.com cloud using electronic instruments such as:

2.1.12v EV Li-ion Battery
A Lithium-ion (Li-ion) battery is a type of rechargeable battery used in electric vehicles and a number of portable electronics. They have a higher energy density than typical lead-acid or nickel-cadmium rechargeable batteries. This means that battery manufacturers can save space, reducing the overall size of the battery pack.
Lithium is also the lightest of all metals. However, lithium-ion (Li-ion) batteries contain no lithium metal, they contain ions. For those wondering what an ion is, an ion is an atom or molecule with an electric charge caused by the loss or gain of one or more electrons. 
2.2. Voltage Sensor
This sensor is used to monitor, calculate and determine the voltage supply. This sensor can determine the AC or DC voltage level. The input of this sensor can be the voltage whereas the output is the switches, analogue voltage signal, a current signal, an audible signal, etc. Some sensors provide sine waveforms or pulse waveforms like output & others can generate outputs like AM (Amplitude Modulation), PWM (Pulse Width Modulation) or FM (Frequency Modulation). The measurement of these sensors can depend on the voltage divider.
2.3. Current Sensor
The current sensor is a device that detects and converts current to get an output voltage, which is directly proportional to the current in the designed path. When current is passing through the circuit, a voltage drops across the path where the current is flowing. Also, a magnetic field is generated near the current-carrying conductor. These above phenomena are used in the current sensor design technique.
2.4. DC Motor
A DC motor is an electrical machine that converts electrical energy into mechanical energy. In a DC motor, the input electrical energy is the direct current which is transformed into the mechanical rotation   
2.5. Battery Management System
              The primary function of a BMS is to fulfil safety requirements. But there’s more to it. Objectives related to the more efficient usage of battery cells and prolongation of their lifetime are also being increasingly integrated into the design of BMS. While there is no unique definition of a BMS, it should be designed with a minimal set of requirements Such as- It must measure individual cell voltages The BMS must measure temperatures at different points as close as possible to the battery It must measure currents flowing through it The BMS should communicate information to control units and undertake action to ensure the battery will be operated within safety limits The BMS should balance battery cells passively or actively The Battery management system guarantees the protection of the Battery Pack and manages the battery.                                       
2.6. Jumper Wires  
Jumper wires are simply wires that have connector pins at each end, allowing them to be used to connect two points to each other without soldering. Jumper wires are typically used with breadboards and other prototyping tools in order to make it easy to change a circuit as needed. Fairly simple. In fact, it doesn’t get much more basic than jumper wires. Though jumper wires come in a variety of colours, the colours don’t actually mean anything. This means that a red jumper wire is technically the same as a black one. But the colours can be used to your advantage in order to differentiate between types of connections, such as ground or power.                                                                                                                                                                   
2.7. Arduino UNO Controller 
A microcontroller based on the Arduino UNO platform has been utilized to control the process as a whole. There are fourteen input and output pins on this device. PWM, which stands for "pulse width modulation," is assigned responsibility for six of these pins. It has been determined that Arduino UNO is the most suitable controller to employ for the prototype due to its user-friendliness. The controller's job is to keep track of the movements of the Sun and then transmit the appropriate signal to the actuators so that they can spin in response. In addition to following the path of the sun, the controller is also responsible for performing the task of self-cleaning by directing the movement of an external actuator.
2.8.  ESP8266 wifi module 
ESP8266 is the name of an infamous WiFi module that is a system on a chip (SoC) developed by Systems, a company based in Shanghai. Originally used with Arduino boards to WiFi-enable hardware projects, it soon became a cheap standalone Arduino-compatible development board. It can function in complete autonomy, without an additional microcontroller like Arduino board for example.
2.9. DHT11 Sensor

To measure both simultaneously, you need a temperature and humidity sensor (DHT11). The digital relative humidity and temperature sensor is a highly accurate component in measuring temperature and humidity


Circuit Diagram:
 
3.Results and Discussion
Thingspeak.com (It’s a cloud website where we can send any data and show or visualize in it)
Then, we upload this source code into the Arduino UNO microcontroller using Arduino IDE.
After Uploading the code, Using the Think speak website all the data shown below,
 
After that, we built our own simple web application where we show or visualize our real-time battery temperature data and indicate whether our battery condition is good or not or whether our battery is running safely or not as well as protecting our battery from fire.
If certainly, the EV battery temperature will increase more than its peak value, then there would be a chance of the battery getting fired. 
So first we retrieve its per second real-time temperature data from the think speak read API link i.e. https://api.thingspeak.com/channels/1842205/fields/1.json?results= and set its particular peak value and give command if the temperature data is exceeded its peak value, then it gives to the user a warning to disconnect the BMS (Battery Management System) which breaks the connection between vehicle’s motor with its battery and save the battery from a dangerous fire.
The EV Battery Fault Indicator and Protector Web Application’s source code is found below the GitHub Link: 
SOURCE CODE:
https://github.com/iamrudra-narayan/EV-Battery-Fault-Detector.git
Open any IDE like VS Code, PyCharm, or any.
Our Web Application is shown below:
When a battery is under peak condition or in a safe condition
 
When the battery is above peak condition then it warns the user first to break the connection of the BMS
 
When the battery is above peak condition then it disconnects BMS
 
Users can visit the link to know their Battery condition and warnings on their mobile phone or on their Desktop.
Link: - https://ev-battery-fault-detector.vercel.app

Available for Android and IOS:
Users can visit the link to know their Battery condition and warnings on their mobile phone or on their Desktop.
Link: - https://ev-battery-fault-detector.vercel.app

4. CONCLUSION
This paper presents a model-based diagnostic scheme for lithium–in–battery cells to determine the presence of the temperature and current fault to get rid of damage in electric vehicles battery. As we know how electric vehicles are essential for us. So, we have the concern to check about vehicle components and we found a way to detect a fault. It’s estimated that near future there will be a massive number of electric vehicles going to be used. So that we can stop air pollution, and even global warming. In near future, this topic has the scope to improve electric vehicle features and solve damages that occur in the EV due to the battery.    
REFERENCES
[1] Wagner F T, Lakshmanan B, and Mathias M F. Electrochemistry and the future of the automobile [J]. Journal of Physics
Chemical Letters, 2010, V1: 2204-2219.
[2] Frank P M. Fault diagnosis in dynamic systems using analytical and knowledge-based redundancy: a survey and some new results [J]. Automatica, 1990, 26 (3): 459-474.
[3] Bohlen O, Buller S, De Doncker R W, et al. Impedance-based battery diagnosis for automotive applications[C]. Power Electronics Specialists Conference, 2004 PESC 04, 2004 IEEE 35th Annual. IEEE, 2004, 4: 2792-2797.
[4] Zheng Y, Han X, Lu L, et al. Lithium-ion battery pack power fade fault identification based on Shannon entropy in electric vehicles[J]. Journal of Power Sources, 2013, VI (223): 136-146.
[5] Grobelink M. Big-data computing: Creating revolutionary breakthroughs in commerce, science, and society [N/OL] (2012-10-02)
