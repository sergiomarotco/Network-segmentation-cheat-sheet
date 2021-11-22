# Best-practice-for-network-segmentation
## What is this?
This project was created to publish the best practices for segmentation of the corporate network of any company. In general, the schemes in this project are suitable for any company.
## Where can I find diagrams?
Graphic diagrams are available in the [Release page](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/releases)
The schema sources are located in the [repository](https://github.com/sergiomarotco/Best-practice-for-network-segmentation)
## Level 1 of network segmentation: basic sergmentation<br/>
![Level 1](https://user-images.githubusercontent.com/29877074/142885564-3ea11fd1-c6ab-4e8c-8c31-8d0b9e32b3d6.jpg)
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
## Level 2 of network segmentation: adoption of basic security practices<br/>
![Level 2](https://user-images.githubusercontent.com/29877074/142885564-3ea11fd1-c6ab-4e8c-8c31-8d0b9e32b3d6.jpg)
### Advantages
More network segments in the corporate network.<br/>
Full duplication of the main supporting infrastructure for production network such as:
1. mail relays;
2. time servers;
3. other services, if available.<br/>

Safer software development. Recommended implementing DevSecOps at least Level 1 of the [DSOMM](https://dsomm.timo-pagel.de/index.php), what requires the introduction of a separate storage of secrets for passwords, tokens, cryptographic keys, logins, etc., additional servers for SAST, DAST, fuzzing, SCA and another DevSecOps tools.
In case of problems in the supporting infrastructure in the corporate segment, this will not affect the production environment.
It is a little harder for an attacker to compromise a production environment.

### Disadvantages
As a result, this leads to the following problems:
1. increasing the cost of ownership and the cost of final services to customers;
2. high complexity of maintenance.

## Level 3 of network segmentation: High adoption of security practices<br/>
Stay with us, click "Watch". In the meantime, implement segmentation at level 2 :)

## Level 4 of network segmentation: Advanced deployment of security practices at scale<br/>
Stay with us, click "Watch". In the meantime, implement segmentation at level 2 :)

## Schematic symbols
Elements used in network diagrams:<br/>
![Schematic symbols](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/blob/main/Schematic%20symbols/Schematic%20symbols.jpg)<br/>
Crossing the border of the rectangle means crossing the firewall.
## Have an idea for improvement?
* Submit your pull reguest;
* Create [issue](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/issues/new);
* Start [discussion](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/discussions/new).
