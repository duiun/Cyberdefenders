1, Identifying the geographical origin of the attack facilitates the implementation of geo-blocking measures and the analysis of threat intelligence. From which city did the attack originate?
First, to determine the location of the attack, we need to identify the victim’s IP address. To do this, we can filter TCP packets with the SYN flag set, since the client typically initiates the connection by sending a SYN packet to the server. This allows us to identify the victim’s IP address and subsequently determine its geographical location
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e729a7cb-984f-49fa-bcd7-f3c4edfa1640" />
Based on this, we can see that the IP address `117.11.88.124` sends the initial SYN packet to `24.49.63.79`, indicating that 117.11.88.124 is the victim’s IP address.

