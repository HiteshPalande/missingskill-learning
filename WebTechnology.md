



















# WEB TECHNOLOGY

























----





#### IP Address 



IP address is just like an ID given to the system which  is connected to the internet. Used for identifying number and other for addressing purpose.

IP addresses are managed by Internet Assigned Number Authority (IANA) and five different Regional Internet Registries(RIR). For better understanding of IP we can take example of Courier Boy.

Suppose a courier boy needs to deliver a courier, so he will look for particular building which is having some name and in that building he will again look for a particular flat number, so exactly happens with browser as it searches for the website server and IP Address. So here in this example building name is like IP address and flat number is like Port.

 

![courierboy](https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/courierboy.jpg)



There are two types of IPs

1) IPv4
2) IPv6

IPV4 has limitations of IPs so IPv6 was introduced in 2004-05 but IPv4 is more popular in terms of networking.



##### Different Classes of IP

**1. CLASS A**

-  0-127(0.0.0.0 to 127.255.255.255)

  Here IP 127 is reserved and called as a loopback address

**2. CLASS B**

- 128.0.0.0 to 191.255.0.0

  These IPs are used for the Internet

**3. CLASS C**

- 192.0.0.0 to 223.255.255.0

  These IPs are used for Local Network

**4. CLASS D**

- 224.0.0.0 to 239.255.255.255

  These IPs are not used and are reserved

**5. CLASS E**

- 240.0.0.0 to 255.255.255.255

  These IPs are not used



#### Web Ports

A port is always associated with the IP of the host Port number is a 16 bit number ranging from 0 to 65535 in which 0 is reserved and cannot be used.

Internet Assigned Number Authority (IANA) is responsible for the registration of the commonly used ports. Ranges & uses of the ports are

- 0-1023

  These ports are used by systems, in Linux machines no other application can be run in 0-1023 port.

- 1024-49150

  These ports are reserved for Application, generally user uses ports from 3000-9999

- 49151-65535

  These are open ports but even if they are open only system can be used these ports



#### Different Types of Browser 

- Brave
- Edge
- Google chrome
- Mozilla Firefox
- Opera 
- Safari



#### Different Types of WEB Servers 

- Apache
- Lite Speed
- Microsoft Internet Information Services
- Nginx



#### HTTP and HTTPS 

HTTP stands for Hypertext Transfer Protocol and was first public in 1991, we can see these whenever we type any website just like http://www.mtnl.com HTTP generally runs over port 80.

 HTTPS which stands for Hypertext Transfer Protocol Secure  as the name suggests HTTPS was built over HTTP but was a bit more secure version of the HTTP.

HTTPS runs on 443 port. We can remember IP address of a application as we use domain name, this domain name is given by IANA.



#### HTTP Verbs 

- **GET** :  Used for fetching  data
- **POST** : Sends the data to the server
- **DELETE** : To delete data
- **OPTION** : Used in Queries
- **HEAD** : Used in Queries
- **PUT** : To send data



#### Difference between HTTP and HTTPS

|                   HTTP                   |                   HTTPS                   |
| :--------------------------------------: | :---------------------------------------: |
|       Hypertext Transfer Protocol        |    Hypertext Transfer Protocol Secure     |
|         Sends data over port 80          |         Sends data over port 443          |
|               Less secure                |                More Secure                |
| data is not encrypted while sending data | Data is encrypted while transferring data |



#### HTTP Headers 

Every request or response has a header, this header includes some basic information, url, method etc. Server & browser communicates using headers.

According to request header and response header browser decides what to do. In simple word HTTP headers are the types of data which the browser of the app sends to the server and based on the server may or may do something and in response the server  sends the back different headers on which browser decides what to display.



#### HTTP Ports

HTTP response status codes are the specific code which indicates if the request has been successful or not.

- **100** :  Indicates that so far everything is alright.
- **200** :  All successful responses indicates by this server
- **300** : Anything that requires migration then this series is used
- **400** :  This series is for user authentication or user check, used for user specific requirement 
- **500** : Indicates problems at server level



#### Software Licensing 

Without Software License we cannot work in industry, it gives legal protection to the user of software. Whenever we use a software or an application for our purpose and after modifying or developing it if we try to publish it under our own r brand and if the software which we use has licensing under different owners then  they can sue us on using there license. So to avoid this we should always check the license of the software.

Software with different license

- **Apache 2.0 License** : Apache is a free software license. A user can use these software for any purpose and also can modify it if needed. It is most popular and widely used all around the world backed up with a strong community. 
- **MIT** : MIT is another free license software available to all users for free. It also allows the user to reuse within proprietary software, providing that either all copies of the licensed software include a copy of the MIT License terms and the copyright notice.
-  **BSD**  : BSD Licenses are a type of licenses which allows users to use their software with minimum restrictions that is in software should clearly mention a copy of the original copyright statement.



#### Databases 

Basically there are two types of databases 

1. Relational Database
2. Non Relational Database



**1. Relational Database**

- MySQL
- SQL
- PostgreSQL
- MariaDB

**2. Non Relation Database**

- MongoDB
- Redis
- Cassandra
- Neo.js



#### Cloud Provider 

- AWS 

- Azure

- Digital Ocean

- Google

- Heroku

- Linode

- Vultr

  

















---









  



 





























































