# Understanding and Applying the OSI Model
An independent learning project by Sean Lehey.

## Table of Contents

[Part 1: The Purpose of the OSI Model](#part-1-the-purpose-of-the-osi-model)   
[Part 2: Identifying the Seven Layers](#part-2-identifying-the-seven-layers)   
[Part 3: Real-World Applications](#part-3-real-world-applications)   


## Acknowledgements

Jeremy's IT Lab's [Videos](https://www.youtube.com/watch?v=t-ai8JzhHuY) on the [OSI Model](https://www.youtube.com/watch?v=7nmYoL0t2tU).   
The Cisco CCNA [Official Cert Guide from](https://www.pearson.com/us/higher-education/program/Odom-CCNA-200-301-Official-Cert-Guide-Library/PGM2166706.html) Pearson.   
TryHackMe's [Introduction to Networking](https://tryhackme.com/room/introtonetworking) room.


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

### Term to Know: Encapsulation
As a unit of data is processed across the layers of the OSI Model, it may pick up some additional data from other layers. This process is known as encapsulation, which will be useful to know later on in this project.

## Part 2: Identifying the Seven Layers

### Layer 7: Application Layer

The application layer interacts with software applications, like your web browser, for instance [jitref]. It utilizes protocols like HTTP and HTTPS in order to send or receive web traffic data. 

### Layer 6: Presentation Layer

### Layer 5: Session Layer

### Layer 4: Transport Layer

### Layer 3: Network Layer

### Layer 2: Data-Link Layer

### Layer 1: Physical Layer


## Part 3: Real-World Applications


