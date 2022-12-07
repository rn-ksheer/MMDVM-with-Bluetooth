# MMDVM-with-Bluetooth
Using MMDVM hat with HC-05 and Android phone


##
1. ## Configure HC-05 Bluetooth Module 
   * Connect Bluetooth Module to PC using any FTDI module asper the pin connections
      * <img src="https://user-images.githubusercontent.com/14138724/206110883-1841c9f6-802f-495d-8f2b-246089349ba5.jpg" width="200">
      
      * <img src="https://user-images.githubusercontent.com/14138724/206111728-42e907f2-2965-4109-b268-73f197bab4e5.png" width="200">

   * Check **COM port** from device manager
   * Plug-in FTDI module and Open **TeraTerm**, Screen will be displayed as shown below:
    
      * <img src="https://user-images.githubusercontent.com/14138724/205962954-df55a14b-78ab-4b7b-ae17-257f11541c3d.jpg" width="400">
    
    * Select **Serial** with the right **COM port**
    
      * <img src="https://user-images.githubusercontent.com/14138724/205965192-b1087012-d5f8-426c-bf72-6d89ed3d370e.png" width="400">  ***Click OK***
    
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
        
        
        







