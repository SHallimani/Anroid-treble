# Anroid-treble
Android Project Treble - Blessing or Treble??

Here we are discussing on the Nww Android Project Treble Architecture


Before digging and understanding on Treble, lets get's clear our Android Architecture trouble's

Android Architecture Before Oreo (8.0)
--------------------------------------

               ---------------------------------------            --------------------------------
		   |  Android Native Application         |            |                               |
		   |   Chrome, Maps, Calculator          |            |        Our Apps               |
		   |  Browser, Contacts,  Calender       |            |    Downloaded from Appstore   |
		   | Gallery, Settings, Phone, launcher  |            |                               |
 		   |            and more etc....         |            |                               |
		   ---------------------------------------            ---------------------------------
               \                                     /            \                               /
                \     Android Framework Api's       /              \    Android Framework Api's  /
                 \                                 /                \                           /
   -------------------------------------------------------------------------------------------------------------------------
		Android Application communicates with Framework over the Google Exported API's 
			                     These Application uses Binder RPS calls (AIDL)
   -------------------------------------------------------------------------------------------------------------------------
                                                      \/ Framework API's   ====================================> CTS 
   -------------------------------------------------------------------------------------------------------------------------
       Android Framework Services which running continuously as Daemons services to provide services to Application         
    
	Power Manager,   Activity Manager,     BroadCast Manager, Surface Flinger Manager, Location Manager                
    Battery Manager, Notification Manager, Sensor manager,    Package Manager,         Storage Manager
	                                          & Many More Service Provider Managers
   --------------------------------------------------------------------------------------------------------------------------
                                                     \/
   --------------------------------------------------------------------------------------------------------------------------
