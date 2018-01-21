# VLAN-BOREAL-LAB

# L3 Inter-VLAN routing

https://www.cisco.com/c/en/us/support/docs/lan-switching/inter-vlan-routing/41860-howto-L3-intervlanrouting.html

# Configure VLAN

https://www.cisco.com/c/en/us/td/docs/switches/datacenter/nexus5000/sw/configuration/guide/cli/CLIConfigurationGuide/VLANs.html

## Statut

La solution de créer les VLANs pourrait fonctionner avec NAT

Un exemple ci-dessous avec DHCP  
https://seansblag.com/2009/12/configuring-a-cisco-router-with-intervlan-routing-and-natpat/


# ------------


Creation de VLAN pour les besoins de laboratoire au college Boreal Toronto

![alt tag](https://github.com/CollegeBoreal/VLAN-BOREAL-LAB/blob/master/VLAN-LAB.png)


## A revoir le port sortant 
```
routeur_lab(config)#int g0/1
routeur_lab(config-subif)#ip address 10.13.237.14 255.255.255.128
routeur_lab(config-subif)#no sh
routeur_lab(config)#ip route 0.0.0.0 0.0.0.0 g0/1
```
