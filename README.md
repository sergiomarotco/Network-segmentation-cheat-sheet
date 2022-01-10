![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=sergiomarotco&show_icons=true&theme=radical)
# Best-practice-for-network-segmentation
## What is this?
This project was created to publish the best practices for segmentation of the corporate network of any company. In general, the schemes in this project are suitable for any company.

## Where can I find diagrams?
Graphic diagrams are available in the [Release page](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/releases)</br>
The schema sources are located in the [repository](https://github.com/sergiomarotco/Best-practice-for-network-segmentation)

## Schematic symbols
Elements used in network diagrams:<br/>
![Schematic symbols](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/blob/main/Schematic%20symbols/Schematic%20symbols.jpg)<br/>
Crossing the border of the rectangle means crossing the firewall.

## Level 1 of network segmentation: basic segmentation<br/>
![Level 1](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/releases/download/2.1/Network.segmentation.Level.1.jpg)

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
![Level 2](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/releases/download/2.1/Network.segmentation.Level.2.jpg)

### Advantages
More network segments in the corporate network.<br/>
Full duplication of the main supporting infrastructure for production network such as:
1. mail relays;
2. time servers;
3. other services, if available.<br/>

Safer software development. Recommended implementing DevSecOps at least Level 1 of the [DSOMM](https://dsomm.timo-pagel.de/index.php), what requires the introduction of a separate storage of secrets for passwords, tokens, cryptographic keys, logins, etc., additional servers for SAST, DAST, fuzzing, SCA and another DevSecOps tools.
In case of problems in the supporting infrastructure in the corporate segment, this will not affect the production environment.
It is a little harder for an attacker to compromise a production environment.<br/>
Or you can implement at least Level 2 of the [SLSA](https://slsa.dev).

### Disadvantages
As a result, this leads to the following problems:
1. increasing the cost of ownership and the cost of final services to customers;
2. high complexity of maintenance.

## Level 3 of network segmentation: high adoption of security practices<br/>
The company's management (CEO) understands the role of cybersecurity in the life of the company. Information security risk becomes one of the company's operational risks. Depending on the size of the company, the minimum size of an information security unit is 15-20 employees.
![Level 3](https://github.com/sergiomarotco/network-segmentation-cheet-sheet/releases/download/3.0/Network.segmentation.Level.3.jpg)

### Advantages
Implementing security services such us;
1. security operation center (SIEM, IRP, SOAR, SGRC);
2. data leak prevention;
3. phishing protection;
4. sanbox;
5. intrusion prevention system;
6. vulnerability scanner;
7. endpoint protection;
8. web application firewall;
9. backup server.

### Disadvantages
High costs of information security tools and information security specialists

## Level 4 of network segmentation: advanced deployment of security practices at scale<br/>
Stay with us, click "Watch". In the meantime, implement segmentation at level 2 :)

### Advantages
Implementing security services such us:
1. privileged Access Management;
2. internal phishing training server;
3. compliance server (configuration assessment).

Now the attacker will not be able to attack the production network, because now a potentially compromised workstation in the corporate network basically does not have network access to the industrial. Related problems:
1. separate workstations for access to the production network - yes, now you will have 2 computers on your desktop :)
2. other LDAP catalog or Domain controller for production network;
3. firewall analyzer, network equipment analyzer;
4. netflow analyzer.

### Disadvantages
Now you will have 2 computers on your desktop if you need access to production network.

## Have an idea for improvement?
* Submit your pull reguest;
* Create [issue](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/issues/new);
* Start [discussion](https://github.com/sergiomarotco/Best-practice-for-network-segmentation/discussions/new).
