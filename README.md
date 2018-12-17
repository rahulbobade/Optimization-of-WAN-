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
   ---
   ![router pune](https://user-images.githubusercontent.com/43333447/50085703-9d365900-01af-11e9-84bd-c1fc18ab0664.png)
---
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
    exit
    exit 
    wr
   
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
### Routing protocol information:
---
![sh ip proto](https://user-images.githubusercontent.com/43333447/50085864-2188dc00-01b0-11e9-874c-9892789d3cba.png)
---

### Router interfaces :
---
![sh ip inter brief](https://user-images.githubusercontent.com/43333447/50085971-89d7bd80-01b0-11e9-8f9d-7ad212dbfb87.png)
---

## Router Mumbai configuration 
---
![router mumbai](https://user-images.githubusercontent.com/43333447/50085737-c1923580-01af-11e9-81b0-cf077249b778.png)
---

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
### Routing protocols information :
---
![sh ip proto](https://user-images.githubusercontent.com/43333447/50086069-ca373b80-01b0-11e9-9cbb-60a2c054ae6b.png)

---
### Interfaces on router Mumbai :
---
![sh ip int brief](https://user-images.githubusercontent.com/43333447/50086138-fbb00700-01b0-11e9-8700-353baa0accf0.png)

---
### Ping result from pc1 to pc3 via router Nagpur-pune-Mumbai :
---
![ping result via nagpur - mumbai router](https://user-images.githubusercontent.com/43333447/50086295-6103f800-01b1-11e9-857b-3c4b2b2f1ce8.png)
---
### Ping result from pc2 to pc3 via router Pune-Mumbai :
---
![ping result](https://user-images.githubusercontent.com/43333447/50086359-a0324900-01b1-11e9-9e25-90c207a81453.png)

---
### Ping result from pc3 to pc 1 via router Mumbai-pune-nagpur :
---
![ping result](https://user-images.githubusercontent.com/43333447/50086419-d40d6e80-01b1-11e9-871c-08b3065c0e13.png)

---

*ALL RESULT CHECK FROM GNS3*
