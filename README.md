# Optimization-of-WAN-


![main screenshots](https://user-images.githubusercontent.com/43333447/50071490-c8f11900-0186-11e9-9160-430bb62ea1a7.png)

## Router Nagpur configuration:
---
![router nagpur](https://user-images.githubusercontent.com/43333447/50085608-62ccbc00-01af-11e9-919f-b119af34334d.png)
---
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
### RIP (Routing information protocol) configuration in Nagpur router:
---
    config terminal
    router rip
    network 192.168.10.0
    network 192.168.20.0
    exit 
    wr
---
### Check Interface in Nagpur Router:     
  ---
  ![sh ip in br](https://user-images.githubusercontent.com/43333447/50085380-bd194d00-01ae-11e9-806e-7e671584ca29.png)
  ---
### Routing information :
---
![show ip protocols](https://user-images.githubusercontent.com/43333447/50085507-1e412080-01af-11e9-97cf-20de786f70b7.png)
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
## RIP (Routing information protocol) configuration in Pune router:
---
    config terminal
    router rip
    network 192.168.20.0
    network 192.168.30.0
    network 192.168.40.0
    exit
    exit 
    wr

## Router Mumbai configuration 

### Fastethernet 0/0 configuration
---

    config terminal
    int f0/0
    no shut 
    ip add 192.168.50.1 255.255.255.0
    exit 
    wr
 ---   
### Mumbai serial interface 1/2 configuration 
---
    int s1/2
    no shut 
    ip add 192.168.40.2 255.255.255.0
    exit  
    wr
---
### Mumbai router password and line configuration:
---
    config terminal 
    enable pass a
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
## RIP (Routing information protocol) configuation in Mumbai Router:
---
    config terminal
    router rip 
    network 192.168.40.0
    network 192.168.50.0
    exit 
    exit 
    wr
---

   
   
   
   
