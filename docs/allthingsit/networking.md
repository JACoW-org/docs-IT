# Networking

A conference venue's capability and limitations needs to be clearly understood

* Communicate expectations clearly, aggree upon them and put the guaranetees in writing (e.g. Service-level-agreement in contract)
* Investigate their system and do not simply believe their claims
* Asses what level of service they can or cannot offer
* Design your network in a way that conference mission critical networks (e.g. proceedings office, presentation management) can not be impacted by convenience networks (e.g. internet browsing, public WiFi) for example
    * Seperate Networks or 
    * Management through VLANs 

## Wired

@TODO review spec recommendations (GBit etc.)

* Network infrastructure at a conference site MUST comfortably allow for the required bandwidth
* Things to look for
    * Local Area Network (LAN) - from computer to switch (min 100 Mbs / rec. 1000 Mbs)
    * Network Backbone - from switch to switch, switch to router, and router to switch (rec. 1000 Mbs+) and enough routing capacity for the number of connections
    * Internet Connection - from the router to Internet Service Provider (ISP) (rec. 500 Mbs+)
    * Prepare a backup/failover, either a second ISP or something that you can use to provide a bare minimum internet to the proceedings office (e.g. 5G router) 

## Wireless

* Remember most participants, exhibitors and editors have more than one devices
* Weaknesses should be addressed in advance!
    * Adding access points
    * Portable access points
    * Worst case: Bring in a third party wireless through a company 
* Use reliable (enterprise grade) wireless devices 

## Wireless vs. Wired:

Wirless performance has become very good with recent WiFi standards. While it is still safer using wired network for the proceedings office and any conference critical system, huge IPAC conferences like 2024 used wireless sucessfully.

The main reason we are still a bit sceptic about wireless is, often the venues are not up to the task of providing a stable wireless system for the amount of users, especially if you also count in the delegates and industry.

WiFi technology is well mature and stable if set up correct and it can be used for the editing room if carefully planned (e.g. seperate wireless network and even access points). It can save costs and can reduce installation time by removing wiring time. 

To be on the safe side, agree with the venue on a service level and make it part of the contract. Write down how many devices you expect to have connected at once (e.g. a delegate might arrive with laptop, phone and a tablet, that would already be three devices for one person) and that conference critical systems should have priority over the guest / delegate connections.

However, keep in mind that the wirless/air interface can be disturbed by a lot of things and a cable connection not as easily.