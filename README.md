# Electrical_5ServoArduino_task1
This repository is for task 1 of the ELECTRICAL track of my summer training at Smart-Methods

----------------------------------------------------------

  //5 Servo motors for robot arm connected with arduino / breadboard

    #include<Servo.h>

  //create objects
  
    Servo servo1,servo2,servo3,servo4,servo5;
    
  //loops:
  
    void setup()
    {
    Serial.begin(9600);
    //set the signals for each servo motor
    servo1.attach(8);
    servo2.attach(9);
    servo3.attach(10);
    servo4.attach(11); 
    servo5.attach(12); 
    }
    void loop()
    {
    //set 90 degrees
    servo1.write(90);
    servo2.write(90);
    servo3.write(90);
    servo4.write(90);
    servo5.write(90);
    delay(1000);

    //set 0 degree
    servo1.write(0);
    servo2.write(0);
    servo3.write(0);
    servo4.write(0);
    servo5.write(0);
    delay(1000);
    }
