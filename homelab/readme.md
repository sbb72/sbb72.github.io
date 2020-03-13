# Home Lab

## Introduction
This is a quick ramble about my home lab.

I used William Lam [virtuallyghetto link](https://www.virtuallyghetto.com/home-lab) site a lot to help choose my hardware configuration.I'd recommend his site and following him on Twitter if you're interested on home labs (and all things to do with virtualisation), lots of good information.
After reviewing various different hardware vedours I decided on Supermicro SYS-E300-9D-8CN8TP due to the on board nics and the physical size of the hardware.

### Delivery has arrived!
A couple of pictures of the hardware before I started to unbox it.

![](pics/nuc.png? "nuc")
![](pics/supermicro_boxed.png? "supermirco")

## Hardware list
I wanted to install ESXi, vCenter and vSAN so I opted for 2 x Supermicro Server system  SYS-E300-9D-8CN8TP and one Intel NUC Hades Canyon to create vSAN ROBO.  The Supermicro servers are used as the vSAN nodes, the Intel NUC is used for the vSAN Witness etc.  Below is a list of the hardware components:

#### Supermicro Server system  SYS-E300-9D-8CN8TP

I've got 2 Supermicro servers,  link to full description [SYS-E300-9D-8CN8TP Specs](https://www.supermicro.com/en/products/system/Mini-ITX/SYS-E300-9D-8CN8TP.cfm) 

| Hardware | Model                                          | Part No            | Comments               |
| -------- | ---------------------------------------------- | ------------------ | ---------------------- |
| Server   | SUPERMICRO Server system                       | SYS-E300-9D-8CN8TP | vSAN Nodes             |
| Memory   | Samsung 32GB DDR4 2666MHz LP ECC Registered x2 | M393A4K40CB2-CTD   | 64 GB of memory        |
| Disk     | Supermicro 64GB SATADOM                        | SSD-DM064-SMCMVN1  | Used to install ESXi   |
| Disk     | Samsung 256GB PM981 M.2 PCIe NVMe              | MZVLB256HAHQ-00000 | Cache disk for vSAN    |
| Disk     | Intel 660p 1TB M.2 PCIe QLC 3D                 | SSDPEKNW010T8X1    | Capacity Disk for vSAN |
| Disk     | Intel 660p 1TB M.2 PCIe QLC 3D                 | SSDPEKNW010T8X1    | Capacity Disk for vSAN |

#### Intel NUC	Hades Canyon

One Intel NUC	Hades Canyon node.

| Hardware | Model                                      | Part No      | Comments                                                   |
| -------- | ------------------------------------------ | ------------ | ---------------------------------------------------------- |
| Server   | Intel NUC                                  | Hades Canyon | Used host vSAN Witness (and other VMs not in vSAN Cluster) |
| Memory   | Crucial 32GB Kit (16GBx2) DDR4-2400 SODIMM |              | 32 GB of Memory                                            |
| Disk     | WD Green M.2 SSD 240GB 7mm SATA Gen 3      | WDS240G2G0B  | ESXi installed on this SSD                                 |
| Disk     | Crucial P1 1TB 3D NAND NVMe PCIe M.2 SSD   | CT1000P1SSD8 | Capacity SSD                                               |


## What does it look like?

Below is a picture on what the hardware looks like, I still need to buy \ create a shelving unit because the servers get quite hot on top of each other.

![](pics/allservers.png? "servers")


### Still need to document \ blog about the following:
* Configuration of the software stack installed.
* Network configuration.
* Shelving \ cabin for the servers and the switch.  #legovsan looks interesting :-)

