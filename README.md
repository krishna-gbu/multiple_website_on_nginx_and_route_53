### launch ec2 instance 
### install nginx
### host multi website
### two domain name
### link domain name to instance
### setup route 53 

## launch ec2 instance 
![image](https://user-images.githubusercontent.com/40553867/204722661-bfd5d1b6-7807-4bed-93bd-962380c1d526.png)

### create instance key
![image](https://user-images.githubusercontent.com/40553867/204722827-1d81f776-edc2-4099-a85a-9172a083d029.png)

![image](https://user-images.githubusercontent.com/40553867/204722925-8c9d415b-f1cb-4d3d-b28d-bfa7c2de84dc.png)

![image](https://user-images.githubusercontent.com/40553867/204722965-394ba022-6998-4a74-8176-55436558e33d.png)
![image](https://user-images.githubusercontent.com/40553867/204722989-03ecbe70-a20c-4379-a0d9-1d05dc3407fd.png)

### launch instance 
![image](https://user-images.githubusercontent.com/40553867/204723056-88a5e887-ef40-487a-9a35-5d2460fffaa0.png)

### now connect ec2 instance with ssh 

![image](https://user-images.githubusercontent.com/40553867/204723142-d4a8d7c1-9f93-4683-9c40-864e652211cd.png)

![image](https://user-images.githubusercontent.com/40553867/204723302-8efa1f36-8508-48ab-9019-3ac25dc3835d.png)
 hit enter :pencil2:
 
![image](https://user-images.githubusercontent.com/40553867/204724911-98e09766-8609-4e45-a9cb-afea2450666b.png)

## install nodejs for reactjs
```
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash - &&\
sudo apt-get install -y nodejs
```
doc https://github.com/nodesource/distributions/blob/master/README.md
![image](https://user-images.githubusercontent.com/40553867/204736471-f404c9dc-9397-41b5-8e4c-e559047deed5.png)

## install nginx 
#### https://www.nginx.com/resources/wiki/start/topics/tutorials/install/

```
sudo apt install nginx -y
```
![image](https://user-images.githubusercontent.com/40553867/204738377-d3765dc2-3056-4fe9-9272-f5f7350f43dd.png)
![image](https://user-images.githubusercontent.com/40553867/204739523-88a7e84f-3d7c-455f-92d0-494e898122d1.png)

## in krishaa.ml website location
![image](https://user-images.githubusercontent.com/40553867/204739460-31054366-21e8-4057-bb12-e6ea441ebbc3.png)
## git clone first website
![image](https://user-images.githubusercontent.com/40553867/204739838-e910007e-6cc7-4381-845e-047779a18161.png)

![image](https://user-images.githubusercontent.com/40553867/204740007-1f0cd8b2-c8c8-4580-bfbe-cec1e1d0905b.png)

```
npm i
npm run build
```
![image](https://user-images.githubusercontent.com/40553867/204740909-ee862005-d316-42f5-8077-efe23d2dbd18.png)

#### copy build file to /var/www/krishna69.tk/html/
### remove default keyward and change location of our site 
![image](https://user-images.githubusercontent.com/40553867/205471884-512fde66-0cf5-402d-bcbf-c9dabe088318.png)

![image](https://user-images.githubusercontent.com/40553867/205471694-32a91efc-a09a-4c7f-9d95-340025073512.png)

![image](https://user-images.githubusercontent.com/40553867/205471703-7134f34f-70a3-49fb-8dba-2a59ea99b1d3.png)

#### copy build to /var/www/krishaa.ml/html/

![image](https://user-images.githubusercontent.com/40553867/205472363-47de3adc-c566-432c-b41c-b585e9f5a3b0.png)

#### remove default and change location of root 
![image](https://user-images.githubusercontent.com/40553867/205472408-7b553f43-216c-4f4e-89c8-1501510d48ca.png)

![image](https://user-images.githubusercontent.com/40553867/205472448-614d4280-1eaa-4e37-93e2-aa7051484097.png)

## ssl
#### https://www.nginx.com/blog/using-free-ssltls-certificates-from-lets-encrypt-with-nginx/

```
sudo apt install certbot python3-certbot-nginx -y
```

```
sudo certbot --nginx -d krishna69.kt -d www.krishna69.kt
```
![image](https://user-images.githubusercontent.com/40553867/205502320-912bdff8-bb78-4cd9-8862-20b80e70fe31.png)

![image](https://user-images.githubusercontent.com/40553867/205502338-40dfaece-86d8-4ed2-9328-2a57dab36c9a.png)

```
sudo certbot --nginx -d krishaa.ml -d www.krishaa.ml
```
#### if error this type means our dns not configure with instance ip
![image](https://user-images.githubusercontent.com/40553867/205502411-4ae261d5-2f55-406d-b85a-cad971cd5200.png)
![image](https://user-images.githubusercontent.com/40553867/205502483-fab80cbd-ec1c-4fcb-9c34-a52b2f827ed3.png)

![image](https://user-images.githubusercontent.com/40553867/205502451-6405d00a-dab6-4133-95f6-c14f81183a38.png)

![image](https://user-images.githubusercontent.com/40553867/205502553-329097d4-ba30-4dd9-a7cf-fc9cf7b59317.png)

### route 53 setup in previous project
https://github.com/krishna-gbu/add_ssl_in_website_nginx_and_route_53
