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
   ---
