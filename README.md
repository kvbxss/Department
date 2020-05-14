# Department

# What we need?

- 10 PCs
- 5 Switches
- 3 Routers
- One Server
- 2 Wireless Routers
- 4 Laptops

# IP and Subnet Mask Configuration
IP shown on the picture, Subnet masks default
![Shown on the Picture](https://scontent-waw1-1.xx.fbcdn.net/v/t1.15752-9/97861212_650653202444552_9086678221553926144_n.png?_nc_cat=104&_nc_sid=b96e70&_nc_ohc=g8iWkL-okpYAX9i3rmB&_nc_ht=scontent-waw1-1.xx&oh=09de9ed7469ddc6f7a28ee935717eb96&oe=5EE380C7)


## SSH Configuration
- Switch(config)# hostname s1
- s1(config)# enable secret haslo


## Access Passwords Configuration

-	Switch>enable 
-	Switch#configure terminal 
-	Switch(config)#line console 0 
-	Switch(config-line)#password cisco 
-	Switch(config-line)#login
-	Switch(config-line)#exit
-	Switch(config)#enable password cisco 
-	Switch(config)#line vty 0 15 
-	Switch(config-line)#password cisco 
-	Switch(config-line)#login 


## Port Security Configuration

-	Switch(config)#interface fastEthernet 0/1 
-	Switch(config-if)#switchport mode access port security
-	Switch(config-if)#switchport port-security
-	Switch(config-if)#switchport port-security mac-address sticky
-	Switch(config-if)#switchport port-security maximum 1 

## MOTD
### Message of the Day Banner

-	Switch>enable 
-	Switch#configure terminal 
-	Switch(config)#banner motd x 



