Smart Link 56K Modem Driver

Version: 3.40.06 

(C) 1998-2003 Smart Link Ltd.
=============================

This document contains release notes and other information about 
this product. Information in this document is the most current 
available. For your convenience, print a copy of this file and 
keep it with your user manual. 

------------------------
How to Use This Document
------------------------
To view README.TXT on screen in Windows Notepad, maximize the 
Notepad window.

To print README.TXT, open it in Windows Write, Microsoft Word, 
or another word processor.  Then select the entire document 
and format the text in 10-point Courier before printing.

This file (README.TXT) contains:

--------
Contents
--------
1) Quick Start
2) How to verify installation
3) Uninstall procedure
4) Update procedure
5) Country selection
6) Call Progress Sounds
7) Known issues
8) Troubleshooting
9) Disclaimers

--------------
1. Quick Start
--------------

1) This driver supports HAMR5600, HAMR5603, SL5604, SL-1500,
   SL-1800,SL-1801, SL-1900 chipsets.  

2) For HAMR5600, SmartRiser56,and SmartRiser561 this driver is compatible with 
   motherboards based on Intel 810, 820, 815E, 820E, 845, 850, ICH4, 
   440MX (Banister), VIA VT82C686, VIA KT266, VIA 8231,VIA 8233,VIA 8235,
   SiS 540/630/96x, NVidia MCP and ALI M1535/M1535D+ core logic chipsets. 

   All riser card form factors are supported (AMR/MDC, CNR and ACR).

   
3) This version of drivers is only compatible with Microsoft 
   Windows XP or Windows 2000. 

4) If any type of Smart Link modem is already installed in your
   system and you want to update its' device driver you may either:

   a) first uninstall existing drivers (See Uninstall Procedure), and only 
      then proceed to install the new drivers.

   b) install the new drivers using Setup.Exe (See installation Procedure).

5) Before installing a riser card modem, check your card for proper 
   jumper setting of Primary or Secondary Codec Mode. PCI modems 
   usually won't have jumpers.


To install your modem drivers for the first time:
-------------------------------------------------

Option 1-Automatic Hardware Detection:

a) Turn your PC off, and remove the power cord.

	NOTE: SOME PCI 2.2 MOTHERBOARDS KEEP THE SLOTS POWERED EVEN 
	WHEN THE PC IS TURNED OFF. TO PREVENT DAMAGE TO YOUR MODEM 
	AND YOUR PC, REMOVE THE POWER CORD.

b) Plug in your modem card into a free slot (AMR/MDC/CNR/ACR slot
   for riser cards or PCI slot).

c) Restart your PC.

d) Windows will instantly detect the modem and will start software
   installation.

e) When requested, point to the drivers installtion directory on the
   floppy disk or CD-ROM. 

f) Modem drivers will be installed.

Option 2-Setup.Exe (this file is provided with the drivers and should be run                       from the drivers installation directory):

a) Turn your PC off, and remove the power cord.

	NOTE: SOME PCI 2.2 MOTHERBOARDS KEEP THE SLOTS POWERED EVEN 
	WHEN THE PC IS TURNED OFF. TO PREVENT DAMAGE TO YOUR MODEM 
	AND YOUR PC, REMOVE THE POWER CORD.

b) Plug in your modem card into a free slot (AMR/MDC/CNR/ACR slot
   for riser cards or PCI slot).

c) Restart your PC.

d) When Windows detects the modem and starts software installation, press    "cancel" to cancel the installation wizard.

e) Double-click on Setup.Exe and follow the instructions.

f) Modem drivers will be installed.


-----------------------------
2. How to verify installation
-----------------------------

To verify that the modem is installed correctly, follow these steps:

 a) Click "Start > Settings > Control Panel > Modem": check for the
    presence of a "Smart Link 56K Modem".

 b) In "Control Panel > Modems > Properties > Diagnostics" click on 
    "Query Modem" button and check that the modem responds.

To Check that the modem is working properly:

 a) Open "Hyper Terminal".
 b) Select the "Smart Link 56K Modem" or "Direct to port" option.
 c) Type ATI1, ATI2 or ATI3 and make sure you receive the modem IDs. 
    Dial any accessible phone number, and see that that phone rings.
    Dial to another modem (ATDTxxx or via the dial button of the     
    TAPI interface) and see that a modem session is established.

    If you have successfully connected, then the modem has been     
    successfully installed.


----------------------
3. Uninstall Procedure
----------------------
a) Click "Start > Settings > Control Panel > Add/Remove Programs".

b) Select "Smart Link 56K Modem".

c) Click the "Add/Remove" button.

d) An Unistall Wizard appears.Follow the instructions.

   You must choose to restart the system in order to complete modem removal.

e) Modem drivers will be uninstalled.

f) You may turn your PC off, remove the power cord and remove the 
   modem card from its' socket.

     NOTE: SOME PCI 2.2 MOTHERBOARDS KEEP THE SLOTS POWERED EVEN
     WHEN THE PC IS TURNED OFF. TO PREVENT DAMAGE TO YOUR MODEM 
     AND PC, REMOVE THE POWER CORD.



-------------------
4. Update Procedure
-------------------

To update your modem drivers:

Option 1:

uninstall previous drivers (see above procedure) and reboot your system.

When the system detects the modem and asks for disk, press "Browse"
and select the updated driver disk in the floppy drive or CD-ROM
drive.

New drivers will be installed.

Option 2:

Reboot your system.

Double-click on Setup.Exe (located in the updated driver installation directory) and follow the instructions.

New drivers will be installed.


--------------------
5. Country Selection
--------------------

To change the country setting, follow these steps:

   a) Click "Start > Settings > Control Panel > Modem Settings".
   b) Select the required country from the list.
   c) Click "Ok".

or

   a) Using a terminal program (such as Hyper Terminal), issue 
      an AT+GCI command to select the desired country.

For information about the usage of AT+GCI commands, refer to an
updated version of the AT-Commands manual, available on Smart Link 
web site (www.smlink.com).

To verify the change has taken effect:

a) Open HyperTerminal and select your modem
b) Type "ATI7"
c) Verify that the correct country name is displayed


-----------------------
6. Call Progress Sounds
-----------------------

Riser card modems hardware typically support four methods 
for monitoring call progress (dialtone, DTMF dialing, etc...). 
The method you should use depends on your specific hardware:

(a) In hardware through AC-Link:
      * Simply connect speakers to the AC97 audio speaker output
      * Then enable and unmute "Telephone" or "Phone in"
        in the Playback audio mixer  from the speaker icon
        that appears in the mixer tray

(b) In software through the audio subsystem:
      * Simply connect speakers to the audio card speaker output.
      * Next, click the right mouse button on SLLights in the
        Windows System Tray while the modem is loaded in memory.
      * Select the speakers on or off as desired.
      
(c) In hardware directly through the sound card:
      * Connect the 4 pin header on the modem card to the TAM 
        header on the audio card/subsytem.

(d) In hardware using the optional buzzer that may be present on the
    modem card:
      * Nothing needs to be done to hear this. It is always on.
        You can control the buzzer volume from the 
        Control Panel/Modem/Properties/Speaker Volume.


---------------
7. Known issues
---------------

7.1 	On certain motherboards, call progress can be heard through
	the system's speakers. This option is enabled by default, and 
	can be controlled only from Windows' "Volume Control" application, 
	using the "Telephony" slider.	The 'Speaker' menu option (accessed 
	by right-clicking on the modem icon) can not mute the modem sound 
	on these motherboards.

7.3  	When some systems get into "sleep mode" and an incoming call
	is received by the modem, the modem answers but the screen stays 
	blank. This behavior is dependent on the BIOS and not on the modem.
	Some BIOS vendors choose to let the modem answer, but leave the 
	screen blank. 

7.3	The NetZero dialer tends to cause the computer to freeze
	sometimes and causes some programs such as "Zcast" to close. 
	This behavior was duplicated with other reference modems as well, 
	so it is not caused by the modem.

7.4   	In Hyperterminal, the characters sent to the modem are not
	echoed until ATZ command is being issued. This behavior was 
	duplicated with other reference modems as well, so it is not 
	caused by the modem.

7.5 	When using the following applications/online services, select
	the appropriate modem name from the following modem list:
	* Juno - "Generic 33600 modem". 
	* BitWare - "Rockwell based voice modem"

7.6	Two Smart Link modems can not be installed on the same PC
	simultaneously. Currently there is no workaround.

7.7 	Specifically on NVidia MCP chipset: when on-board audio is 
	disabled from BIOS, the modem	is also disabled. This is by chipset 
	design. Workaround: disable audio from Device Manager.
7.8	Card test is not supported on Discrete DAA Card.

------------------
8. Troubleshooting
------------------

If your modem does not work as expected:

8.1	If ERROR, NO DIALTONE or a similar message is received:

	(a)   Check whether the line is connected preperly to the modem.
	(b)   Use a telephone handset to make sure that the line is
	      active and that there is a dial tone.
	(c)   Check to see if the line is a PBX line or a direct analog
              phone line. You may need to dial 9, before the actual 
              desired telephone number (i.e. ATDT9,123-4567).
              If, after dialing 9, the modem still cannot detect the
		  PBX dialtone, try typing ATX3 before dialing.

              NOTE that PBX lines typically can only support V.34
              rates (33,600 bps, 28,800 bps, ...) and NOT V.90
              rates (49,333 bps, 50,666 bps, ...).


8.2	If dialer application (i.e. Hyperterminal) does not detect modem:

	Check whether HyperTerminal is configured to the right port.
	You can find the modem's COM port number in 
 	"Control Panel > Modems > Properties". 
	If not, press disconnect and change the port that the dialer 
	is accessing.


8.3	If you cannot hear the dialtone and DTMF dialing while the modem
	should be dialing out:
	
     	Riser card modems hardware designs typically support four
	methods for monitoring call progress (dialtone, DTMF dialing,
	etc...):

          - In hardware through AC-Link.
             * Simply connect speakers to the AC97 audio speaker
	     output.
             * Then enable and unmute "Telephone" or "Phone in"
               in the Playback audio mixer  from the speaker icon in
	     the mixer tray.
          - In software through the audio subsystem.
              * Simply connect speakers to the audio card speaker
	      output.
              * Next, click the right mouse button on SLLights in the
                Windows System Tray while the modem is loaded in
                memory.
              * Select the speakers on or off as desired.
          - In hardware directly through the sound card.
              * Connect the 4 pin header on the modem card to the
	      TAM header on the audio card/subsytem.
          - In hardware using the optional buzzer that may be
            present on the modem card.
              * Nothing needs to be done to hear this. It is always
                on. You can control the buzzer volume from the 
                Control Panel/Modem/Properties/Speaker Volume.

8.4	If the Modem has connection problem try the followings:

	(a) Enable "safe mode 1" from Start--> Setting--> Control Panel--> Modem Settings--> Modem Helper tab. 
	(b) Download a new driver from: www.smlink.com\download
	(C) Try to dial to the Internet with "Quick Connect" disabled. go to Start--> Setting--> Control Panel-->V.92 features settings--> V.92 Features tab.

--------------------
9. Disclaimers
--------------------
The following are important disclaimers as related to our products.
Proper use of our chipsets and drivers are clearly described. 

Smart Link does not guarantee product performance or accept any 
liability due to the improper usage of its drivers or chipsets.

* Modem is capable of receiving data up to 56Kbps. Actual send and
receive speeds may vary depending upon factors, such as connecting 
modem and phone line connections.

* Modem must use the appropriate US or International chipset version
for the country to which it is shipped.

* Modem must use the appropriate driver version for the operating
system in which it is being installed.

* All trademarks are property of their respective owners.
