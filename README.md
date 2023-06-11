# Bmw-F10-cluster-canbus
Here are some can bus ids and bytes for them

Fore some ids you have to make a counter!


oil temp: 0x3f9, 0x02, count, count, 0x00, 0x00, 148, count, count;

fuel: 0x349, 0x00, 0x01, 0xBE, 0x0A, 0x00, 0x00, 0x00, 0x00;

airbag: 0xD7, count, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00;

parking Brake: 0x36f, count, count, count;

seatbelt: 0x581, 0x40, 0x4d, 0, 0x28, 0xff, 0xff, 0xff, 0xff;
################################################################

Drive mode | byte 5 change mode

0x3A7, 0x00, count, 0x00, 0x00, 5, 0x00, 0x00, 0x00;

1= Traction, 2= Comfort, 4= Sport, 5= Sport+, 6= DSC off

##################################################################


ignition: 0x12F, 0xFB, count, 0x8a, 0x1C, 0xF1, 0x05, 0x30, 0x86;

left menu: 0x1EE, 0xC4, 0x0C, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00;

###################################################################

EfficientDynamics  byte 6 | byte 3 rpm


  0xF3, count, count, 0x00, 0x00, 1, count, count, count;
  
  
  ##################################################################
  
  ABS | both can ids have to be present for abs to turn off!
  
  
  0x36E, 0x00, count, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00;
  
  0xB6E, count, count, count, count, count, count, count, count;
  
  #######################################################################

  Speedometer     kinda work?                byte 5 change speed


  0x1A1,0x00, count, 0x00, count, 0xAA,count,count,count
  
  
  #########################################################################
  
  Steering thing and esp. first byte= steering lock light, second is ESP light
  
   CanSend(0x2a7, 0, STCount, 0, 0, 0, 0, 0, 0);
   
   
 
   
   STCount++;
     if (GayCount > 0x101)
     {
         GayCount = 0xA1;
         
      
     }
  
    
    ###########################################################################
  
  
  
  
  
  
  
  
  
  






