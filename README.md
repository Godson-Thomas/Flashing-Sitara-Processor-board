



## _Flashing: Sitara Processor Board_

<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/Sitara.PNG" width="150">  <br>















### _Requirements_
1. Hyperterminal<br>
2. Putty<br>
3. RS232 to USB converter<br>
4. Ethernet LAN Cable (Serial)
5. Following files:

<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/Files.PNG" width="650">  <br><br>

-----------------------------------

# _HyperTerminal_

----------------------------


* **Connect the RS232 to USB converter** and find the port from the **Device Manager**.

<br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(1).png" width="700"><br><br>


* Open Hyperterminal.

<br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(2).png" width="700"><br><br>

  * Select the port.
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(3).png" width="700"><br><br>

  * Set **Bits per second** to  _115200_ .
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(4).png" width="700"><br><br>

 * Since flash is empty, _CCCCC_ will be printed on the console.


<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(5).png" width="700"><br><br>




* **_Transfer_** >> **_Send File_**.

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(6).png" width="700"><br><br>
        
   - set _Protocol_ to _1K Xmodem_.

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(7).png" width="700"><br><br>

* Click on _Browse_ and select the _u-boot-spl.bin_ for transfer.
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(8).png" width="700"><br><br>

* **_Transfer_** >> **_Send File_**
   - set _Protocol_ to _Y modem_.

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(9).png" width="700"><br><br>

* Click on _Browse_ and select the _u-boot_ for transfer.
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(10).png" width="700"><br><br>

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(11).png" width="700"><br><br>

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(12).png" width="700"><br><br>



- Close the HyperTerminal window.
---------------------------
<br>


# _Putty_
--------------------------

* Open Putty
   - Select the port and set the configuration as follows.

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(13).png" width="700"><br><br>





* U-boot is accessible now.

  - set the serverip & ipaddr using the following commands.

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(14).png" width="500"><br><br>

* **Connect the LAN Cable**


* Windows Control Pannel
    
     - _Network and Internet_
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(15).png" width="700"><br><br>
     - _Network and Sharing Center_
    <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(16).png" width="700"><br><br>
     - _Change adapter settings_

     <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(17).png" width="700"><br><br>

     - Right click on _Ethernet_ & select _Properties_.

     <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(18).png" width="700"><br><br>


     - Select _Internet Protocol Version 4 (TCP/IPv4)_ and click on _Properties_.

     <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(19).png" width="700"><br><br>


     - set the IP address as follows.

     <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(20).png" width="700"><br><br>

* Check whether the server(PC) is responding.
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(21).png" width="500"><br><br>



-----------------------------------------------------

# _TFTP_
----------------------------------------
* Run the _tftpd32_ with admin privilages.

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(22).png" width="550"><br><br>

* Type the following command from the U-boot:
```
run setup
```
* The Ubi image will be written into the flash.


<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(23).png" width="500"><br><br>
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(24).png" width="500"><br><br>





----------------------------------

# _Easy Connect_

* Setting password for the Linux using Easy Connect.

<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(25).png" width="700"><br><br>

*  Open the easy connect
*  **Devices** >> **SYNC261** >> **SYNC261-M1** >> **Add Device to Configuration**.
<br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(26).png" width="700"><br><br>

* Click on _IP Configuration_.
    <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(27).png" width="700"><br><br>

* Set the Target (SYNC261) IP.
    <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(28).png" width="700"><br><br>

* Enter the password and click on _Set Password_
   <br><br>
<img src="https://github.com/Godson-Thomas/Flashing-Sitara-Processor-board/blob/master/S(29).png" width="700"><br><br>