
| #   | OSI                | Function                                                                                                                                                                                      | Examples                                      |
| --- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| 7   | APLICATION LAYER   | Provides network services directly to end-users or applications.                                                                                                                              | HTTP, FTP, IRC, SSH, DNS                      |
| 6   | PRESENTATION LAYER | Translater data between the application layer and a lower layers. Responsible for data format translation, encryption, and compression to ensure thatt data is presented in a readable forma. | SSL/TLS, JPEG, GIF, SSH, IMAP                 |
| 5   | SESSION LAYER      | Manages sessions or connections between applicacions. Handles synchronization, dialog controlm and token management. (Interhost communication)                                                | APIs, NetBIOS, RPC                            |
| 4   | TRANSPORT LAYER    | Ensures end-to-end communication and provides flow control                                                                                                                                    | TCP, UDP                                      |
| 3   | NETWORK LAYER      | Responsible for logical addressing and routing. (Logical Addressing)                                                                                                                          | IP, ICMP, IPSec                               |
| 2   | DATA LINK LAYER    | Manages access to the physical medium and provides error detection. Responsible for framing, addressing and error checking of data frames. (Physical addressing)                              | Ethernet, PPP, Switchet, etc.                 |
| 1   | PHYSICAL LAYER     | Deals whit the physical connection between devices                                                                                                                                            | USB, Ethernet Cables, Coax, Fiber, Hubs, etc. |