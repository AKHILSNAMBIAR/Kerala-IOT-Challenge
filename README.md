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
| *    2* |   |
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |


### Experiment No. 1
#### Hello World LED Blinking
##### *Aim:-*
*To familiarize with blinking of LED using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *2*   |
| *4*   | *Resistor (220ohms)*     | *1*      |
| *5* | *LED  | *1* |
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
delay(1000); <!---// wait for a second--->






