###PROGRAMMING

    The programming in Arduino IDE is much similar to 'c' programming.

###Setup() and Loop (

   There are two special functions that are a part of every Arduino sketch: setup () and loop (). At the start of power or a reset, the setup () function is called once. It is used only for one time operations required at power on. 

   The loop () function takes care of the application code. It keeps on executing until the power supply is switched off. It is mandatory to include both the functions, whether needed or not.



    ARDUINO CODE (HARDWARE):

#include <SoftwareSerial.h>

SoftwareSerialmySerial(2, 3);

int rl = A0;

int 12-A1;

int r3 = A2;

int r4=A3;

//Bluetooth Data Clear

int incomingByte =0;

// put your setup code here, to run once:

pinMode(r1, OUTPUT);

pinMode(r2, OUTPUT);

pinMode(r3, OUTPUT);

pinMode(r4, OUTPUT);

Serial.begin(9600); // Arduino 0-TX, 1-RX, Bluetooth TX, RX



mySerial.begin(9600); // Arduino 2-TX, 3-RX

// put your main code here, to run repeatedly:

serialdata();

void serialdata()

if(mySerial.available() > 0)

incomingByte mySerial.read():

switch(incomingByte)

digitalWrite(r), HIGH);

int 14-A3;

int incomingByte = 0;

void setup() {

pinMode(r3, OUTPUT);

void loop() {

case 'I':
digitalWrite(r1,HIGH):

Serial.println("Device 1 ON ");

incomingByte="*";

break;

mySerial.println("Device 1 ON "); mySerial.println("Device 1 OFF");

case '2':

digitalWrite(rl, LOW);

Serial.println("Device 1 OFF");

incomingByte="*";

break;

case '3':

digitalWrite(r2, HIGH);

Serial.println("Device 2 ON ");

mySerial.println("Device 2 ON ");

incomingByte-'*';

break;

case '4':

digitalWrite(r2, LOW);

Serial.println("Device 2 OFF");

mySerial.println("Device 2 OFF");

incomingByte="*";

break;

}
}

