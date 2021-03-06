=====
About
=====

This is a Python module which allows you to interact with a Cisco Mobility Express controller to retrieve data, make configuration changes, etc. Features currently include:

- Getting information about associated clients, such as a list of clients with details, connection scores, and connection speeds
- Getting a list of and details about registered APs
- Restarting APs
- Blinking or toggling AP LEDs
- System information, such as the Mobility Express version, platforms, etc. 

 
Implementation Notes
--------------------

`gen-enpoints.py` programmatically generates the base functions for each API call in `_me_api.py` by interrogating the Mobility Express Web UI and identifying and parsing potential calls from the front-end to the back-end. Then these functions are front-ended by simple manually written-methods in `ciscomeapi.py` to provide more context and niceties like docstrings. So far just a few of these methods have been created, more coming soon. 

This project is not affiliated with or supported by Cisco Systems in any way. It uses private, undocumented, and unsupported web calls and therefore may not work as expected and may cease to function with a future update of Mobility Express. Caveat emptor!
