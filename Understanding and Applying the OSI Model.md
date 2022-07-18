# ***note: this project is not finished yet***

# Understanding and Applying the OSI Model
An independent learning project by Sean Lehey.

## Table of Contents

[Part 1: The Purpose of the OSI Model](#part-1-the-purpose-of-the-osi-model)   
[Part 2: Understanding the Seven Layers](#part-2-understanding-the-seven-layers)   
[Part 3: Real-World Applications](#part-3-real-world-applications)   


## Acknowledgements

1. Jeremy's IT Lab's [Videos](https://www.youtube.com/watch?v=t-ai8JzhHuY) on the [OSI Model](https://www.youtube.com/watch?v=7nmYoL0t2tU).   
2. The Cisco CCNA [Official Cert Guide](https://www.pearson.com/us/higher-education/program/Odom-CCNA-200-301-Official-Cert-Guide-Library/PGM2166706.html) from Pearson.   
3. TryHackMe's [Introduction to Networking](https://tryhackme.com/room/introtonetworking) room.
4. This [archived encapsulation and protocol chart](https://web.archive.org/web/20120529200700/http://www.wildpackets.com/elements/misc/WP_encapsulation_chart.pdf) from the now defunct WildPackets.com.


## Part 1: The Purpose of the OSI Model

The OSI Model, or, Open Systems Interconnection Model, is a descriptive model which creates an outline for and categorizes networking protocols and standards. It solves the problem of having two devices from different manufacturers being unable to communicate with one another due to different communication standards or protocols. All modern devices are developed and manufactured with the OSI Model in mind so that they may *interconnect*, as the name of the model prescribes. With this project, I wanted to create a study resource which I can reference while studying for my CCNA. In the following sections, we'll define each layer of the OSI Model, how that layer relates to day-to-day networking activities, and at the end, we'll work through a practical interview question that I've encountered multiple times.

### Memorizing the Layers

Many people use mnemonics in an effort to memorize things, and one helpful mnemonic that I came across for the OSI Model is as follows:  

| Mnemonic  | OSI Layer  | #  |
|---|---|---|
| **A**ll  | **A**pplication  | 7  |
| **P**eople  | **P**resentation  | 6  |
| **S**eem  | **S**ession  | 5  |
| **T**o  | **T**ransport  | 4  |
| **N**eed  | **N**etwork  | 3  |
| **D**ata  | **D**ata-Link  | 2  |
| **P**rocessing  | **P**hysical  | 1  |

Each layer represents a different step in the process of interconnection, and as such, each layer is associated with different devices, protocols, and PDUs (Protocol Data Unit), which we'll touch on in the next section. Let's move on to each individual layer and learn their distinct functions.

### Encapsulation
As a unit of data is processed through the layers of the OSI Model, it may pick up some additional data from other layers. This process is known as encapsulation, which will be useful to know later on in this project.

### De-Encapsulation
De-encapsulation is the processing of stripping the encapsulated data as it moves up the OSI model after arriving at the machine receiving the data. So, a machine sending data encapsulates information as it moves *down* the OSI stack (a vertical visualization of the OSI Model), and a machine receiving data de-encapsulates it as it moves *up* the OSI stack.<sup>[1]</sup>

## Part 2: Understanding the Seven Layers

### Layer 7: Application Layer

| Common Protocols<sup>[4]</sup>  | HTTP  | HTTPS  | SMTP  | DNS  | SSH  | Telnet  |
|---|---|---|---|---|---|---|
| **Port Numbers**  | **80**  | **443**  | **25**  | **53**  | **22**  | **23**  |

The application layer is commonly described as the layer closest to the end user.<sup>[1]</sup> It utilizes protocols like HTTP (80), HTTPS (443), and more to communicate with applications like your web browser in order to load or transmit application data across devices. As suggested by the presence of SSH and Telnet in the above table, it also allows for secure and unsecure remote access into a device.

### Layer 6: Presentation Layer

The presentation layer represents the process through which data is translated to the appropriate format so as to be readable by the application layer. The presentation layer is also where encryption (when sending data) and decryption (when receiving data) takes place.

### Layer 5: Session Layer

The session layer creates, manages, and terminates connections between the local application and the remote application.<sup>[1]</sup> A site like Google creates and terminates millions of sessions per day.

### Layer 4: Transport Layer
*Note: This layer's protocol data unit is called a **Segment***.   

The transport layer *segments* and *reassembles* data for communication between end hosts. It is also responsible for end-to-end, or host-to-host, communication. A layer 4 header is added to every segment of data at this layer.<sup>[1]</sup>

### Layer 3: Network Layer
*Note: This layer's protocol data unit is called a **Packet***.   

The network layer establishes connectivity between end hosts on different networks<sup>[1]</sup>. This layer also provides logical addressing in the form of IP addresses.<sup>[1]</sup> An example of a layer 3 device is a router.

### Layer 2: Data-Link Layer
*Note: This Layer's protocol data unit is called a **Frame***.   



### Layer 1: Physical Layer
*Note: This Layer's protocol data unit is called a  **Bit***.   



The physical layer includes, simply enough, *physical devices* used in networking like hubs, repeaters, and network cables. Those network cables create a physical connection between devices by way of their ports, using electrical signals in the wire.

## Part 3: Real-World Applications

Feel free to check out some other projects on my [profile](https://github.com/seanlehey)!
