# Optitrack_natnet
Simple Python script to connect to the Optitrack Motion Capture System.

* In the script **optitrack_test.py**, edit the **clientAddress** and the **optitrackServerAddress**, as well as the **id** of the rigid body.
* Run the script:

    ``
     $ python optitrack_test.py
    ``
 

**Note:** for Linux or MacOS, modify the line 280 of the **NatNetClient.py** file, replacing
``result.bind((self.local_ip_address, port))`` for ``result.bind((self.multicast_address, port))``