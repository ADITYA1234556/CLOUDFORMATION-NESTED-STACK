To note:
The servers need JAVA-VERSION-11 or newer

The nexus server can fail because of insufficient memory based on your system specifications. 

The default values of java heapsize are under sudo nano /opt/nexus/bin/nexus.vmoptions
Find for the 
-Xms2703M
-Xmx2703M
And replace the minimum and maximum java virtual machine heapsize with below and restart nexus
-Xms512M
-Xmx1024M
