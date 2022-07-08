# Servo-motor
# using Tinkercad to design and code the Servo motor circuit

#include <Servo.h>
Servo servo1;
int pos =0;
void setup()
{
  servo1.attach(13);// because signal pin is connected with 13
}

void loop()
{
  // rotate from 0 to 180 degree
  for(pos=0;pos<=180;pos++){
    servo1.write(pos);
    delay(15);}
  for(pos=10;pos>=0;pos--){
    servo1.write(pos);
    delay(15);}
    
}
