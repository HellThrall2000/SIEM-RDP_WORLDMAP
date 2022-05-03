


# SIEM-RDP_WORLDMAP

>Setting up Azure Sentinel SIEM(Security Information and Event Management) and connecting it to a live virtual machine acting as a honeypot to observe live attacks from around the world on a map.


https://i.redd.it/owx6nbi7qsx61.jpg



## Installation

-Create an azure account. Go to resources page and click on template. Use my template that is uploaded as template.json file to deploy the same virtual machine.

-Make custom deployment to change account name and give a password.

-Signup at https://ipgeolocation.io/ and get an API key.


---

## Setup
-The powershell script Log_exporter.ps1 runs inside the vm. 

-Change the API key and run the script.
http://g.recordit.co/M01Q5yIuL6.gif

-The log info shows :
![loginfo](https://user-images.githubusercontent.com/86112651/166524065-8f5b1454-9a7e-4342-9453-3a3eb2dbd18a.png)

-Using microsoft sentinel go to the custom workbook and run it to view the map according to the query.
https://g.recordit.co/12AVmNax4D.gif

-The map shows the statistics of the attacks from all over the world
![map](https://user-images.githubusercontent.com/86112651/166524249-48633a92-8754-4dcf-9e5a-0b66c254b49b.png)


## Test
-Try to connect the vm from your normal pc using remote desktop but give wrong credentials. Your ip will pop up in the list of events.
## Resources at a glance
- A resource visualizer
![visualizer](https://user-images.githubusercontent.com/86112651/166525190-79da900f-04ca-4cc6-bac7-b729c12ed9d8.jpg)


## License
