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


### Experiment No. 7
#### Button Controlled LED 
##### *Aim:-*

*To familiarize with LDR light Sensor using Arduino Uno.*

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
| *8* | *LDR sensor*  | *1* |

##### *Circuit Diagram:-*

##### *Code:-*

int potpin=0; <!---// initialize analog pin 0, connected with photovaristor--->

int ledpin=11;<!---// initialize digital pin 11 --->

int val=0;<!---// initialize variable val--->

void setup()

{

pinMode(ledpin,OUTPUT);<!---// set digital pin 11 as “output”--->

Serial.begin(9600);<!---// set baud rate at “9600”--->

}

void loop()

{

val=analogRead(potpin);<!---// read the value of the sensor and assign it to val--->

Serial.println(val);<!---// display the value of val--->
Serial.println(val);<!---// display the value of val--->

analogWrite(ledpin,val/4);<!---// set up brightness（maximum value 255）--->

delay(10);<!---// wait for 0.01 --->

}


### Experiment No. 8
#### Flame Sensor
##### *Aim:-*

*To familiarize with flame sensor using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Resistor (10Kohms)*     | *1*      |
| *5* | *Buzzer*  | *6* |
| *6*        | *USB Cable*     |   *1* |
| *7*        | *Flame Sensor*     |   *1* |

##### *Circuit Diagram:-*

##### *Code:-*

int flame=0;<!---// select analog pin 0 for the sensor --->

int Beep=9;<!---// select digital pin 9 for the buzzer --->

int val=0;<!---// initialize variable --->

void setup()

{

pinMode(Beep,OUTPUT);<!---// set LED pin as “output” --->

pinMode(flame,INPUT);<!---// set buzzer pin as “input” --->

Serial.begin(9600);<!---// set baud rate at “9600” --->

} 

void loop() 

{ 

val=analogRead(flame);<!---// read the analog value of the sensor ---> 

Serial.println(val);<!---// output and display the analog value --->

if(val>=600)<!---// when the analog value is larger than 600, the buzzer will buzz --->

{  

digitalWrite(Beep,HIGH); 
   
}
   
else 
   
{  

digitalWrite(Beep,LOW); 
     
}

delay(500); 

}

### Experiment No. 9
#### LM35 Sensor
##### *Aim:-*
*To familiarize with LM35 sensor using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *LM35 Sensor*     | *1*      |
| *5*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*

##### *Code:-*

int potPin = 0; <!---// initialize analog pin 0 for LM35 temperature sensor --->

void setup()

{

Serial.begin(9600);<!---// set baud rate at”9600” --->

}

void loop()

{

int val;<!---// define variable --->

int dat;<!---// define variable --->

val=analogRead(0);<!---// read the analog value of the sensor and assign it to val --->

dat=(125*val)>>8;<!---// temperature calculation formula ---> 

Serial.print("Tep");<!---// output and display characters beginning with Tep --->

Serial.print(dat);<!---// output and display value of dat --->

Serial.println("C");<!---// display “C” characters --->

delay(500);<!---// wait for 0.5 second --->

}

### Experiment No. 10
#### IR Remote Control Using TSOP 
##### *Aim:-*

*To familiarize with IR Remote Control using Arduino Uno and TSOP.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Resistor (220ohms)*     | *6*      |
| *5* | *LED*  | *6* |
| *6*        | *USB Cable*     |   *1* |
| *7*        | *Infrared Remote Control*     |   *1* |
| *8*        | *Infrared Receiver*     |   *1* |

##### *Circuit Diagram:-*

##### *Code:-*

#include <IRremote.h>

int RECV_PIN = 11;

int LED1 = 2;

int LED2 = 3;

int LED3 = 4;

int LED4 = 5;

int LED5 = 6;

int LED6 = 7;

long on1  = 0x00FF6897;

long off1 = 0x00FF9867;

long on2 = 0x00FFB04F;

long off2 = 0x00FF30CF;

long on3 = 0x00FF18E7;

long off3 = 0x00FF7A85;

long on4 = 0x00FF10EF;

long off4 = 0x00FF38C7;

long on5 = 0x00FF5AA5;

long off5 = 0x00FF42BD;

long on6 = 0x00FF4AB5;

long off6 = 0x00FF52AD;

IRrecv irrecv(RECV_PIN);

decode_results results;

// Dumps out the decode_results structure.

// Call this after IRrecv::decode()

// void * to work around compiler issue

<!---//void dump(void *v) --->

{

<!---//  decode_results *results = (decode_results *)v--->
void dump(decode_results *results*) 

{

int count = results->rawlen;

if (results->decode_type == UNKNOWN) 

{

Serial.println("Could not decode message");

} 

else 

{

if (results->decode_type == NEC) 

{

Serial.print("Decoded NEC: ");

} 

else if (results->decode_type == SONY) 

{
       
Serial.print("Decoded SONY: ");
      
} 
    
else if (results->decode_type == RC5) 

{

Serial.print("Decoded RC5: ");
     
} 
    
else if (results->decode_type == RC6) 
      
{
       
Serial.print("Decoded RC6: ");
      
}
     
Serial.print(results->value, HEX);

Serial.print(" (");

Serial.print(results->bits, DEC);

Serial.println(" bits)");

}

Serial.print("Raw (");

Serial.print(count, DEC);

Serial.print("): ");

for (int i = 0; i < count; i++) 

{
     
if ((i % 2) == 1) {
      
Serial.print(results->rawbuf[i]** USECPERTICK, DEC);
     
} 
    
else  
     
{
      
Serial.print(-(int)results->rawbuf[i]*USECPERTICK, DEC);
     
}
    
Serial.print(" ");
     
}
      
Serial.println("");
   
}

void setup()

{

pinMode(RECV_PIN, INPUT); 

pinMode(LED1, OUTPUT);
  
pinMode(LED2, OUTPUT);

pinMode(LED3, OUTPUT);

pinMode(LED4, OUTPUT);

pinMode(LED5, OUTPUT);

pinMode(LED6, OUTPUT);  

pinMode(13, OUTPUT);

Serial.begin(9600);

irrecv.enableIRIn(); <!---// Start the receiver --->

}

int on = 0;

unsigned long last = millis();

void loop() 

{

if (irrecv.decode(&results)) 

{

<!---// If it's been at least 1/4 second since the last --->

<!---// IR received, toggle the relay --->

if (millis() - last > 250) 

{

on = !on;

digitalWrite(8, on ? HIGH : LOW);

digitalWrite(13, on ? HIGH : LOW);
       
dump(&results);


}

if (results.value == on1 )

digitalWrite(LED1, HIGH);

if (results.value == off1 )

digitalWrite(LED1, LOW); 

if (results.value == on2 )

digitalWrite(LED2, HIGH);

if (results.value == off2 )

digitalWrite(LED2, LOW); 

if (results.value == on3 )

digitalWrite(LED3, HIGH);

if (results.value == off3 )

digitalWrite(LED3, LOW);

if (results.value == on4 )

digitalWrite(LED4, HIGH);

if (results.value == off4 )

digitalWrite(LED4, LOW); 

if (results.value == on5 )

digitalWrite(LED5, HIGH);

if (results.value == off5 )

digitalWrite(LED5, LOW); 

if (results.value == on6 )

digitalWrite(LED6, HIGH);

if (results.value == off6 )

digitalWrite(LED6, LOW);        

last = millis();      

irrecv.resume(); <!---// Receive the next value --->

}

}

### Experiment No. 11
#### Potentiometer Analog Value Reading
##### *Aim:-*
*To familiarize with Potentiometer analog value reading using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *10Kohms Potentiometer*  | *1*      |
| *5*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*

##### *Code:-*
int potpin=0;<!---// initialize analog pin 0 --->

int ledpin=13;<!---// initialize digital pin 13 --->

int val=0;<!---// define val, assign initial value 0 --->

void setup()

{

pinMode(ledpin,OUTPUT);<!---// set digital pin as “output” --->

Serial.begin(9600);<!---// set baud rate at 9600 --->

}

void loop()

{

digitalWrite(ledpin,HIGH);<!---// turn on the LED on pin 13 --->

delay(50);<!---// wait for 0.05 second --->

digitalWrite(ledpin,LOW);<!---// turn off the LED on pin 13 --->

delay(50);<!---// wait for 0.05 second --->

val=analogRead(potpin);<!---// read the analog value of analog pin 0, and assign it to val  --->

Serial.println(val);<!---// display val’s value --->

}

### Experiment No. 12
#### 7 Segment Display
##### *Aim:-*

*To compile a program to operate a 7Segment Display and simulate the model using Arduino Uno.*

##### *Components Required:-*

| *No.* | *Component Name* | *Requirement* |
| :---:         |     :---:      |          :---: |
| *1*   | *Arduino Uno*    | *1*    |
| *2*     | *Breadboard*       | *1*    |
| *3*   | *Jumper wire (Male to Male)*     | *as per need*   |
| *4*   | *Resistor (220ohms)*     | *8*      |
| *5* | *1-digit LED Segment Display*  | *1* |
| *6*        | *USB Cable*     |   *1* |

##### *Circuit Diagram:-*

##### *Code:-*

int a=7;<!---// set digital pin 7 for segment a--->

int b=6;<!---// set digital pin 6 for segment b--->

int c=5;<!---// set digital pin 5 for segment c--->

int d=10;<!---// set digital pin 10 for segment d--->

int e=11;<!---// set digital pin 11 for segment e--->

int f=8;<!---// set digital pin 8 for segment f--->

int g=9;<!---// set digital pin 9 for segment g--->--->

int dp=4;<!---// set digital pin 4 for segment dp--->

void digital_0(void) <!---// display number 5--->

{

unsigned char j;

digitalWrite(a,HIGH);

digitalWrite(b,HIGH);

digitalWrite(c,HIGH);

digitalWrite(d,HIGH);

digitalWrite(e,HIGH);

digitalWrite(f,HIGH);

digitalWrite(g,LOW);

digitalWrite(dp,LOW);

}

void digital_1(void) <!---// display number 1--->

{

unsigned char j;

digitalWrite(c,HIGH);<!---// set level as “high” for pin 5, turn on segment c--->

digitalWrite(b,HIGH);<!---// turn on segment b--->

for(j=7;j<=11;j++)<!---// turn off other segments--->

digitalWrite(j,LOW);

digitalWrite(dp,LOW);<!---// turn off segment dp--->

}

void digital_2(void)<!--- // display number 2--->

{

unsigned char j;

digitalWrite(b,HIGH);

digitalWrite(a,HIGH);

for(j=9;j<=11;j++)

digitalWrite(j,HIGH);

digitalWrite(dp,LOW);

digitalWrite(c,LOW);

digitalWrite(f,LOW);

}

void digital_3(void)<!--- // display number 3--->

{digitalWrite(g,HIGH);

digitalWrite(a,HIGH);

digitalWrite(b,HIGH);

digitalWrite(c,HIGH);

digitalWrite(d,HIGH);

digitalWrite(dp,LOW);

digitalWrite(f,LOW);

digitalWrite(e,LOW);

}

void digital_4(void) <!---// display number 4--->

{digitalWrite(c,HIGH);

digitalWrite(b,HIGH);

digitalWrite(f,HIGH);

digitalWrite(g,HIGH);

digitalWrite(dp,LOW);

digitalWrite(a,LOW);

digitalWrite(e,LOW);

digitalWrite(d,LOW);

}

void digital_5(void)<!--- // display number 5--->

{

unsigned char j;

digitalWrite(a,HIGH);

digitalWrite(b, LOW);

digitalWrite(c,HIGH);

digitalWrite(d,HIGH);

digitalWrite(e, LOW);

digitalWrite(f,HIGH);

digitalWrite(g,HIGH);

digitalWrite(dp,LOW);

}

void digital_6(void)<!--- // display number 6--->

{

unsigned char j;

for(j=7;j<=11;j++)

digitalWrite(j,HIGH);

digitalWrite(c,HIGH);

digitalWrite(dp,LOW);

digitalWrite(b,LOW);

}

void digital_7(void) <!---// display number 7--->

{

unsigned char j;

for(j=5;j<=7;j++)

digitalWrite(j,HIGH);

digitalWrite(dp,LOW);

for(j=8;j<=11;j++)

digitalWrite(j,LOW);

}

void digital_8(void)<!--- // display number 8--->

{

unsigned char j;

for(j=5;j<=11;j++)

digitalWrite(j,HIGH);

digitalWrite(dp,LOW);

}

void digital_9(void) <!---// display number 5--->

{

unsigned char j;

digitalWrite(a,HIGH);

digitalWrite(b,HIGH);

digitalWrite(c,HIGH);

digitalWrite(d,HIGH);

digitalWrite(e, LOW);

digitalWrite(f,HIGH);

digitalWrite(g,HIGH);

digitalWrite(dp,LOW);

}

void setup()

{

int i;<!---// set variable--->

for(i=4;i<=11;i++)

pinMode(i,OUTPUT);<!---// set pin 4-11as “output”--->

}

void loop()

{

while(1)

{

digital_0();<!---// display number 0--->

delay(1000);<!---// wait for 1s--->

digital_1();<!---// display number 1--->

delay(1000);<!---// wait for 1s--->

digital_2();<!---// display number 2--->

delay(1000);<!--- // wait for 1s--->

digital_3();<!---// display number 3--->

delay(1000);<!--- // wait for 1s--->

digital_4();<!---// display number 4--->

delay(1000);<!--- // wait for 1s--->

digital_5();<!---// display number 5--->

delay(1000); <!---// wait for 1s--->

digital_6();<!---// display number 6--->

delay(1000);<!--- // wait for 1s--->

digital_7();<!---// display number 7--->

delay(1000);<!--- // wait for 1s--->

digital_8();<!---// display number 8--->

delay(1000); <!---// wait for 1s--->

digital_9();<!---// display number 9--->

delay(1000);<!--- // wait for 1s--->

}

}








