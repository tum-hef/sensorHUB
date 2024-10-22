# sensorHUB
The sensorHUB stack builds upon existing backend solutions from data management and identity and access management, and puts a new graphical web application into the center of the architecture, aiming to enhance the latest technology stack towards a novel, user-friendly IoT project solution. The sensorHUB’s graphical web application represents a new front-end application for managing IoT projects. Its streamlined navigation ensures simplicity, allowing users to reach their intended destinations in a few clicks. 

The primary features include the management and visualization of IoT data. The app further provides a knowledge section, which includes essential training material on the provided software services. Interfaces to complementary IoT software (here: Node-RED) and optional forwarding of login tokens complement the default functionalities. Aligned with our requirements on interoperability, scalability and open-source, the data-related core of the sensorHUB stack represents a scalable cluster of Docker-containerized FROST-servers. 

The original sources of IoT data adding data to the [FROST-Servers](https://github.com/FraunhoferIOSB/FROST-Server) can be manifold; the post requests however need to fulfil the SensorThings API (STA), which can be done directly from an external source or indirectly by transforming third-party data formats into STA using optionally provided instances of the Extract-Transform-Load (ETL)-software [Node-RED](https://nodered.org/). By integrating [Keycloak](https://www.keycloak.org/) into our application, we ensure that data and interactions are protected in accordance with users’ access rights. Keycloak provides authentication to the sensorHUB web application and secures its routes by requiring users to authenticate themselves. Due to its decentral approach, further modules implementing the required authentication interface
can be easily integrated. 

In addition, several supportive components were required to guarantee the scalability and func tioning of the network communication and server administration. Each sub-component is hosted as web application and can therefore be addressed using HTTP/S network communication. For mor details, see the related ISPRS publication sensorHUB - a novel, open-source Software Stack for enhanced Accessibility and secure Interoperability in IoT Project Management available at [ISPRS archives](10.5194/isprs-archives-xlviii-4-2024-197-2024).

![iot_stack_concept](https://github.com/user-attachments/assets/e0a7ed49-ff79-41b6-b2c7-406c281329ed)

# Version
We provide two versions of sensorHUB:
- sensorHUB_LITE (see [repository](https://github.com/tum-hef/sensorHUB_LITE)): a HTTP-based version for developing, testing and non-operational purposes on local machines 
- sensorHUB_PRO (see [repository](https://github.com/tum-hef/sensorHUB_PRO)): a HTTPS-based version for more operational uses with domain-based routes 

Both versions, relate to the sensorHUB web application, which is provided in a separate [repository](https://github.com/HEFLoRa/WEB_APP/). 

## Authors
David Gackstetter, Parid Varoshi, Syed Saad Zahidi

Contact: david.gackstetter@tum.de


## License

Copyright (C) 2024 Technical University of Munich, Arcisstr. 11, 80333 Munich, Germany.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Lesser General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
