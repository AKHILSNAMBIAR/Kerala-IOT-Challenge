# <ins><u>Kerala IoT Challenge</u></ins>


## Introduction to IoT Challenge

***Foxlab Makerspace** in association with **GTech - Group of Technology Companies** in Kerala is launching our prestigious program  **“Kerala IoT Challenge 2021”**,  with a vision to mould 100 IoT experts in Kerala, hosting on the **MuLearn** platform. Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation.*


## Author

*Hi All, Myself **Akhil S Nambiar**. I am currently pursuing my final year of B.Tech at **College of Engineering Trikaripur**. The branch which I chose as my graduation stream is Electrical and Electronics Engineering. Looking forward to enthusiastically participate in this challenge and will try to imbibe the knowledges available in this platform at my full capacity.* 


## A brief intro to _What is IoT?_

*The Internet of Things (IoT) is a system of interrelated computing devices, mechanical and digital machines, objects, animals or people that are provided with unique identifiers and the ability to transfer data over a network without requiring human-to-human or human-to-computer interaction. IoT is at the epicenter of the Digital Transformation Revolution that is changing the shape of business, enterprise and people’s lives. This transformation influences everything from how we manage and operate our homes to automating processes across nearly all industries.*

*The following image will give us a better picture of IoT :-* 

<img src="https://user-images.githubusercontent.com/91836479/136671233-fc09dfe1-8324-4423-98a1-829520fd84d1.jpg">

## Iot Challenge Experiments

*Following are the list of experiments which are to be completed in this Level 1 Iot Challenge:-*

| *Experiment No* | *Name of Experiments* |
| :---: | :---: |
| *1* | *LED Blinking*  |
| *2* | *Traffic Light*  |
| *3*  | *Chasing Effect* |
| *4* | *Button Controlled LED* |
| *5*  | *Buzzer*  |
| *6*  |  *RGB LED* |



### Experiment No. 1
#### Hello World LED Blinking
##### *Aim:-*
*To familiarize with blinking of LED using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Resistor (220ohms)*     | *1*      |
| *5* | *LED*  | *1* |
| *6*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*

![image](https://user-images.githubusercontent.com/91836479/136679381-599e84b1-a273-495f-b942-5ce70445da4b.png)

##### *Code:-*

int ledPin = 10; <!---// define digital pin 10.--->

void setup()

{

pinMode(ledPin, OUTPUT);<!---// define pin with LED connected as output.--->

}

void loop()
{

digitalWrite(ledPin, HIGH);<!---// set the LED on.--->

delay(1000); <!---// wait for a second.--->

digitalWrite(ledPin, LOW); <!---// set the LED off.--->

delay(1000);<!---// wait for a second--->

}

##### *Video Tutorial:-*

<video src="https://user-images.githubusercontent.com/91836479/137487506-2c81113e-5992-41c7-b0f0-62637ed940ec.mp4" controls="" width="50%" height"50%"></video>


### Experiment No. 2
#### Traffic Light
##### *Aim:-*
*To model an electronic circuit of traffic lights using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Resistor (220ohms)*     | *3*      |
| *5* | *Red LED*  | *1* |
| *6* | *Yellow LED*  | *1* |
| *7* | *Green LED*  | *1* |
| *8*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*
 
![image](https://user-images.githubusercontent.com/91836479/136680440-22ce53be-7612-42de-8afb-730e9418cc9d.png)

##### *Code:-*

int redled =10; <!---// initialize digital pin 10.--->

int yellowled =7; <!---// initialize digital pin 7.--->

int greenled =4; <!---// initialize digital pin 4.--->

void setup()

{

pinMode(redled, OUTPUT); <!---// set the pin with red LED as “output”--->

pinMode(yellowled, OUTPUT); <!---// set the pin with yellow LED as “output”--->

pinMode(greenled, OUTPUT); <!---// set the pin with green LED as “output”--->

}

void loop()

{
digitalWrite(greenled, HIGH); <!---//// turn on green LED--->

delay(5000); <!---// wait 5 seconds--->

digitalWrite(greenled, LOW); <!---// turn off green LED--->

for(int i=0;i<3;i++) <!--- // blinks for 3 times--->

{

delay(500); <!---// wait 0.5 second--->

digitalWrite(yellowled, HIGH); <!---// turn on yellow LED--->

delay(500); <!---// wait 0.5 second--->

digitalWrite(yellowled, LOW); <!---// turn off yellow LED--->

} 

delay(500); <!---// wait 0.5 second--->

digitalWrite(redled, HIGH); <!---// turn on red LED--->

delay(5000); <!---// wait 5 seconds--->

digitalWrite(redled, LOW); <!---// turn off red LED--->

}

##### *Video Tutorial:-*

<video src="https://user-images.githubusercontent.com/91836479/137471820-0b5a0676-b2de-4313-b3ba-6a2d8f3b9ed7.mp4" controls="" width="30%"></video>


### Experiment No. 3
#### Chasing Effect 
##### *Aim:-*

*To compile a program to simulate LED chasing effect and practically model it using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Resistor (220ohms)*     | *6*      |
| *5* | *LED*  | *6* |
| *6*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*

![image](https://user-images.githubusercontent.com/91836479/136680646-d6c07623-632b-4c05-96bf-9bdfd1004198.png)

##### *Code:-*

int BASE = 2 ; <!---// the I/O pin for the first LED--->

int NUM = 6; <!---// number of LEDs--->

void setup()

{

   for (int i=BASE;i<)BASE+NUM);i++) 
   
   {
  
pinMode(i, OUTPUT); <!---// set the pin with yellow LED as “output”--->
     
   }
   
}

void loop()

{

   for (int i=BASE; i<(BASE+NUM);i++) 
   
   {
   
digitalWrite(i, LOW); <!---// set I/O pins as "output"--->
     
delay(200); <!---// delay--->
     
   }
   
   for (int i = BASE; i < BASE + NUM; i ++) 
   
   {
   
digitalWrite(i, HIGH); <!--- //setI/Opinsas“high”,turnonLEDsonebyone --->
     
delay(200); <!--- //delay --->
     
   }  
   
}

##### *Video Tutorial:-*

<video src="https://user-images.githubusercontent.com/91836479/137472022-0953fcd3-0f56-422b-b555-2743172bad6a.mp4" controls="" width="30%"></video>


### Experiment No. 4
#### Button Controlled LED 
##### *Aim:-*

*To program an Arduino UNO for controlling an LED using a button and experimentally verify it.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Resistor (220ohms)*     | *1*      |
| *5*   | *Resistor (1Kohms)*     | *1*      |
| *6* | *LED*  | *1* |
| *7*        | *USB Cable*     |   *1* |
| *8* | *Button Switch*  | *1* |

##### *Circuit Diagram:-*


##### *Code:-*

int ledpin=11;<!---// initialize pin 11--->

int inpin=7;<!---// initialize pin 7--->

int val;<!---// define val--->

void setup()

{

pinMode(ledpin,OUTPUT);<!---// set LED pin as “output”--->

pinMode(inpin,INPUT);<!---// set button pin as “input”--->

}

void loop()

{

val=digitalRead(inpin);<!---// read the level value of pin 7 and assign if to val--->

if(val==LOW)<!---// check if the button is pressed, if yes, turn on the LED--->

{

digitalWrite(ledpin,LOW);

}

else

{

digitalWrite(ledpin,HIGH);

}

}

##### *Video Tutorial:-*

<video src="https://user-images.githubusercontent.com/91836479/137473752-d73eb118-0721-48f8-b76a-b3762b072b3c.mp4" controls="" width="30%"></video>


### Experiment No. 5
#### Buzzer
##### *Aim:-*
*To familiarize with buzzer using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Buzzer*     | *1*      |
| *5*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*

##### *Code:-*

int buzzer=8;<!---// initialize digital IO pin that controls the buzzer--->

void setup() 

{ 

pinMode(buzzer,OUTPUT);<!---// set pin mode as “output”--->

} 

void loop() 

{

digitalWrite(buzzer, HIGH); <!---// produce sound--->

}

##### *Video Tutorial:-*

<video src="https://user-images.githubusercontent.com/91836479/137473988-f69a222b-9868-4c9f-a922-9d56a7b1dd61.mp4" controls="" width="30%"></video>


### Experiment No. 6
#### RGB LED
##### *Aim:-*
*To familiarize with RGB LED using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *RGB LED*  | *1*      |
| *5*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*

##### *Code:-*
int redpin = 11; <!---//select the pin for the red LED--->

int bluepin =10; <!---// select the pin for the blue LED--->

int greenpin =9;<!---// select the pin for the green LED--->

int val;

void setup() 

{

pinMode(redpin, OUTPUT);

pinMode(bluepin, OUTPUT);

pinMode(greenpin, OUTPUT);

Serial.begin(9600);

}

void loop() 

{

for(val=255; val>0; val--)

{
   
analogWrite(11, val);
   
analogWrite(10, 255-val);

analogWrite(9, 128-val);

delay(1); 

}

for(val=0; val<255; val++)

{

analogWrite(11, val);

analogWrite(10, 255-val);

analogWrite(9, 128-val);

delay(1);
 
}
 
Serial.println(val, DEC);

}











