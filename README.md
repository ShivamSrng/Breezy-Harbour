# Breezy-Harbour

## Introduction
Harbour is a place where all the import or export business of any country for a specific state or the whole country takes place. 

Due to this management of Harbour resources like monetary funds becomes necessary as much of country’s wealth is based on its export or import business. 

Using our project Harbour management becomes lot more easily as it provides flexibility as well as portability to users as well as the main Harbour authorities to monitor dock availability. Not only it provides monitoring of dock to authorities, but also incoming ships’ pilots or sailors can get to know whether a place for docking is available at port or not. 

Along with dock monitoring it also gives information about temperature and humidity of that place. Due to this weather can be forecasted, tides can be predicted which in turn proves to be beneficial to Harbour authorities as well as maritime sailors. 

Also, it provides information whether ship is correctly docked or not which prevents the collision of ship with the land of Harbour. Due to this a lot of money loss which could have been incurred in prevented. 

For smoother operation this all thing can be monitored just by using an app specially designed for this purpose. In this app, Harbour authorities are given special privilege of turning sensors on/off which normal users cannot enjoy. Hence it also maintains secrecy of some resources of database from users which are not intended to know.


## Circuit Diagram
![image](https://user-images.githubusercontent.com/67229090/209555828-82eb4c1d-0ebf-4885-aefc-f98d7b739f22.png)


## Working of Model
1. The sensor would capture values at interval of every 2 millisecond that a ship is available at Harbour or not. And, on next 2 millisecond temperature, humidity, pressure, wind speed and wind inclination  values are recorded. 

2. This distance passed to Firebase Database which then is transferred to Kodular app with help of Firebase Database extension. 

3. Now based on distance received into Kodular software, if distance is less than 15 cm and greater than 8 cm, it shows “Perfect Distance” message to Administrator only. But if distance between Ship and port is less than 8 cm it shows “Ship too close to port” as message. Such messages are shown only to Harbour Authorities as such messages are of no use to normal users. 

4. Along with Distance, Temperature, Humidity, Pressure, Wind Speed and Wind Inclination is also passed to Firebase Database which are then, by similar process is transferred to Kodular software which can be seen by both Administrators as well as Users. 

5. Also, to add visual aid an LED is provided which lights up when the ship is docked appropriately i.e., at a distance less than 30cm and greater than 10cm. This provides better vision at night-time to sailors, maritime sailors as well as to authorities. 

6. Authentication of user is based on their Email. A user is classified as Normal User or Harbour Authority based on his/her Email. This is done by Kodular software. All the Harbour Authority Emails can be pre-stored in Kodular software to provide them administrative controls like turning a particular sensor on/off, etc.


## Actual Implementation




