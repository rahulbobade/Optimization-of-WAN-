# Optimization-of-WAN-


![main screenshots](https://user-images.githubusercontent.com/43333447/50071490-c8f11900-0186-11e9-9160-430bb62ea1a7.png)

## Router Nagpur configuration:

### First interface 0/0 configuration

---

    config terminal

    interface Fastethernet 0/0

    no shut

    ip add 192.168.10.1 255.255.255.0

    exit

    exit

    wr 

---

### Serial interface 1/1 configuration:
---
    config terminal
  
    interface serial 1/1
   
    no shut 
   
    clock rate 64000
   
    ip add 192.168.20.1 255.255.255.0
    exit 
    
    exit 
    
    wr
    
   ---
   ### Password and line configuration in Nagpur router:
   ---
    config terminal 
    enable pass a
    enable sec b 
    line vty 0 1276
    pass a
    login
    exit 
    line aux 
    pass a
    login
    exit 
    line con 0 
    pass a
    login
    exit
    wr
    ---
  
   ## Router pune configuration:
 ### Fastethernet config
 ---
    config terminal
    interface f0/0
    no shut 
    ip add 192.168.30.1 255.255.255.0
    exit 
 ---
 
### Serial interface 1/2 configuration 

 ---
 
    config terminal 
    int s1/2
    no shut 
    ip add 192.168.20.2 255.255.255.0
   
---
    
### Serial interface 1/1 configuration
---
    config terminal
    int s1/1
    no shut
    clock rate 64000
    ip add 192.168.40.1 255.255.255.0
    exit 
    exit 
    wr
---
### Router pune password and line configuration 
---
    config terminal
    enbale pass a
    enable sec b
    line vty 0 1276
    pass a
    login
    exit 
    line con 0 
    pass a
    login
    exit 
    line aux 0 
    pass a
    login
    exit 
    wr 
---
   
   
   
   
