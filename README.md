
# Project 9 Obstalce Detector
This is Obstalce as well as proximity detector will reflected if there is any obstacle nearby.


## Introduction
The atProtocol is the underlying network protocol used by the atPlatform. The atPlatform provides people, entities, and things with unique identifiers called atSigns.

Each atSign creates its own public and private cryptographic key pair. The private keys are kept private and public keys made available globally through the atProtocol.

The atProtocol provides verbs for interacting with fully qualified atSigns and the data in their secondary servers.


## Prerequisites 
There are two requirements for developing with at_java on your machine.

Java 8 or higher

Maven

A code editor

## Creating an instance of AtClient
To create an instance of AtClient, use one of the factory methods. Note: you must have the .atKeys file in the ~/.atsign/keys directory. You can generate a .atKeys file from using the Register CLI or Onboaring CLI if you already own the atSign.

String ATSIGN_STR = "@bob";
AtSign atSign = new AtSign(ATSIGN_STR);
AtClient atClient = null;
try {
    atClient = AtClient.withRemoteSecondary(atSign);
} catch (AtException e) {
    System.err.println(e);
    e.printStackTrace();
}
## How to start the project
1. Clone the GitHub repo
2. Open the code in a suitable java code editor.
3. Open the src file.
4. run java



## Working of the project
Once the project set up is done then you will be able to see the new screen with option to check the proximity and motion detection buttons.
when you will click on proximity button a new window will appear that will show if any obstacle is in proximity with a boolean value.
And the option button with obstacle detection will show is there any obstacle near using a boolean value
 
