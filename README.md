# MMDVM-with-Bluetooth
Using MMDVM hat with HC-05 and Android phone

### Click to watch Video Tutorial:
<div align="center">
      <a href="https://youtu.be/peXm5wWeBAw">
     <img 
      src="https://user-images.githubusercontent.com/14138724/208304269-5abb270d-7763-4236-92d7-3a2a7517a342.jpg" 
      alt="YouTube link" 
      style="width:50%;">
      </a>
    </div>

    

##
1. ## Configure HC-05 Bluetooth Module 
   * Connect Bluetooth Module to PC using any FTDI module asper the pin connections
      * <img src="https://user-images.githubusercontent.com/14138724/206110883-1841c9f6-802f-495d-8f2b-246089349ba5.jpg" width="200">
      
      * <img src="https://user-images.githubusercontent.com/14138724/206869373-7f3b383b-f3fc-43ca-82c0-d3f298d8349d.png" width="200">
      

   * Plug-in FTDI module and Check **COM port** from device manager
   * Open **TeraTerm**, Screen will be displayed as shown below:
    
      * <img src="https://user-images.githubusercontent.com/14138724/205962954-df55a14b-78ab-4b7b-ae17-257f11541c3d.jpg" width="400">
    
    * Select **Serial** with the right **COM port**
    
      * <img src="https://user-images.githubusercontent.com/14138724/208306673-3958e21e-54b0-4cf2-aa61-17d81f7a1a68.png" width="400">  ***Click OK***

    * GoTO **Setup**   
      
      * <img src="https://user-images.githubusercontent.com/14138724/205966306-26ee5a72-787a-4b6c-969c-aaf116e80820.png" width="400">

    * Under *SETUP –> Terminal & select CR*+*LF at TRANSMIT* and *Enable Local echo*.

      * <img src="https://user-images.githubusercontent.com/14138724/205966962-d0e2944d-2ea5-4ad7-93f7-7f9f3e4e1c94.png" width="400">  ***Click OK***

    * Under *SETUP –> SERIAL PORT* select:
      * <img src="https://user-images.githubusercontent.com/14138724/205967313-ab16f421-1d1f-4794-8071-f4a9ffa93761.png" width="400">
 
      * <img src="https://user-images.githubusercontent.com/14138724/205987882-08d0c762-4f72-411c-875d-cc3cd354b07f.png" width="400">  ***Click New setting*** 
      
    * AT commands
      ```
      AT
      ```
     * you should get an ***OK*** response. This confirms our connections are correct.

        * <img src="https://user-images.githubusercontent.com/14138724/206116977-657e3623-a2d8-4991-83fd-c53357d1e978.png" width="200">
     
     * Check existing name and UART baud rate of the module <a id="anchor1"> </a>
          ```
          AT+NAME?
          ```
          ```
          AT+UART?
          ```
      
        * <img src="https://user-images.githubusercontent.com/14138724/206117911-74f012bb-3869-42c2-a28d-e9ec06114647.png" width="200">
        
     * Lets change the *name* and *UART baud rate*
          ```
          AT+NAME=BlueStack
          ```   
          ```
          AT+UART=115200,0,0
          ```   
    *  Response should be as shown
    
        * <img src="https://user-images.githubusercontent.com/14138724/206119813-a8a0ebbc-ae96-425f-af18-8eb07412a5de.png" width="200">
        
    *  We can verify name and UART with these [AT commands](#anchor1)
    

        * <img src="https://user-images.githubusercontent.com/14138724/206120475-006b66d0-56e6-4761-bf54-a8ad4da1b3c9.png" width="200">
        <br>
        <br>
        <br>
        
       
 2. ## Configure BlueDV application
     * Android settings
        
        * <img width="225" alt="1" src="https://user-images.githubusercontent.com/14138724/208306214-b681e08f-8c80-4820-aea8-1902753e32c9.png">          <img width="225" alt="2" src="https://user-images.githubusercontent.com/14138724/208306215-422bcdfa-c0d0-4918-88d1-fd9bfd09662c.png">     <img width="225" alt="3" src="https://user-images.githubusercontent.com/14138724/208306216-30993f17-a6bf-4a36-a3f2-b02962d4bf80.png">     <img width="225" alt="4" src="https://user-images.githubusercontent.com/14138724/208306287-3b04d5de-3ad2-4f7c-9a9c-3bda4767e2ad.png">








