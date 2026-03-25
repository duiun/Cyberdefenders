1, Identifying the geographical origin of the attack facilitates the implementation of geo-blocking measures and the analysis of threat intelligence. From which city did the attack originate?
First, to determine the location of the attack, we need to identify the victim’s IP address. To do this, we can filter TCP packets with the SYN flag set, since the client typically initiates the connection by sending a SYN packet to the server. This allows us to identify the victim’s IP address and subsequently determine its geographical location
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e729a7cb-984f-49fa-bcd7-f3c4edfa1640" />
Based on this, we can see that the IP address `117.11.88.124` sends the initial SYN packet to `24.49.63.79`, indicating that `117.11.88.124` is the victim’s IP address.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8ef0d34f-52a0-46ac-8049-e49bd0de72fa" />
Once the victim’s IP address is identified, we can determine its geographical location is `Tianjin`.

2, Knowing the attacker's User-Agent assists in creating robust filtering rules. What's the attacker's Full User-Agent?
The User-Agent is a field in the HTTP protocol used by the client to identify itself (it can be a tool or a browser) to the server, so it can be found in the HTTP request header.
Based on this, we can follow and read the HTTP stream and find out the `User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/115.0`.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/21c7abbf-fc82-46df-bc65-757df6ad21b2" />
