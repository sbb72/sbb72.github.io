# Home Lab

### Introduction
This is a quick ramble about my home lab.

I used William Lam [virtuallyghetto link](https://www.virtuallyghetto.com/home-lab) site alot to help choose my hardware. I'd recommend his site and following him on Twitter if you're interested on home labs, loads of good information.

After reviewing various different hardware vedours I decided on Supermicro SYS-E300-9D-8CN8TP due to the on boaord nics and the physical size of the hardware.

### Delivery has arrived!
A couple of pictures of the hardware before I started to unbox it.

![](pics/nuc.png? "nuc")
![](pics/supermicro_boxed.png? "supermirco")

### Hardware list

| Hardware | Make                                           | Make               | Comments                                                                                                                           |
| -------- | ---------------------------------------------- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------- |
| Server   | SUPERMICRO Server system                       | SYS-E300-9D-8CN8TP | Link to full description [SYS-E300-9D-8CN8TP Specs](https://www.supermicro.com/en/products/system/Mini-ITX/SYS-E300-9D-8CN8TP.cfm) |
| Memory   | Samsung 32GB DDR4 2666MHz LP ECC Registered x2 | M393A4K40CB2-CTD   |
| Disk     | Supermicro 64GB SATADOM                        | SSD-DM064-SMCMVN1  | Used to install ESXi                                                                                                               |
| Disk     | Samsung 256GB PM981 M.2 PCIe NVMe              | MZVLB256HAHQ-00000 | Cache disk for vSAN                                                                                                                |
| Disk     | Intel 660p 1TB M.2 PCIe QLC 3D                 | SSDPEKNW010T8X1    | Capacity Disk for vSAN                                                                                                             |
| Disk     | Intel 660p 1TB M.2 PCIe QLC 3D                 | SSDPEKNW010T8X1    | Capacity Disk for vSAN                                                                                                             |




![](pics/cables_esxi.png? "cables")


