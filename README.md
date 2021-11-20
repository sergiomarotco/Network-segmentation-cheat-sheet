# Best-practice-for-network-segmentation
## What is this?
This project was created to publish the best practices for segmentation of the corporate network of any company. In general, the schemes in this project are suitable for any company.
## Where can I find diagrams?
Graphic diagrams are available in the [Release page](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/releases)
The schema sources are located in the [repository](https://github.com/sergiomarotco/Best-practice-for-network-segmentation)
## Level 1 of network segmentation: basic sergmentation:<br/>
![Level 1](https://user-images.githubusercontent.com/29877074/142728178-a2f7255b-71b4-4e89-991e-a0463678f5f0.jpg)
### Advantages
Basic segmentation to protect against basic targeted attacks that make it difficult for an attacker to advance on the network.
Basic isolation of the productive environment from the corporate one.

### Disadvantages
The default corporate network should be considered potentially compromised. Potentially compromised workstations of ordinary workers, as well as workstations of administrators, have basic and administrative access to the production network.

In this regard, the compromise of any workstation can theoretically lead to the exploitation of the following attack vector. An attacker compromises a workstation in the corporate network. Further, the attacker either elevates privileges in the corporate network or immediately attacks the production network with the rights that the attacker had previously obtained.

### Attack vector protection:
Installation the maximum number of information protection tools, real time monitoring suspicious events and immediate response.<br/>
OR!<br/>
Segmentation according to level 2 requirements<br/>
## Level 2 of network segmentation: adoption of basic security practices:<br/>

### Schematic symbols
Elements used in network diagrams:<br/>
![Schematic symbols](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/blob/main/Schematic%20symbols/Schematic%20symbols.jpg)<br/>
Crossing the border of the rectangle means crossing the firewall.
## Have an idea for improvement?
* Submit your pull reguest;
* Create [issue](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/issues/new);
* Start [discussion](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/discussions/new).
