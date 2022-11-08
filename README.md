# Huawei Cloud Project

## Case: Communicate VPCs Each Other
### You are expected to set up a network structure by using HUAWEI CLOUD’s basic services. This application will consist of VPC, VPC-Peering, ECS and RDS. This guide provides high level instructions to complete your DEMO case.

- Step 1. Create three VPCs with different IP pool.

- Step 2. Create a Secuirty Group and allow this security group for every incoming request.

- Step 3. Create two ECS’, one in 1. VPC one in 2. VPC

- Step 4. Create database (use RDS for mysql) in 3.VPC

- Step 5. Use “Remote Login” for ECS’ and try to ping other ECS and RDS.

- Step 6. Create VPC-Peering between 1.VPC-2.VPC, 1.VPC-3.VPC and 2.VPC-3.VPC

- Step 7. Add routing rules to use VPC-Peerings.

- Step 8. Use “Remote Login” for ECS’ and try to ping other ECS and RDS again.
##
##  So let's start

### 1. First, let's set up Vpc with 3 different CID addresses

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/2.png?raw=true)<br/><br/>

### 2. Security group-> Inbound rules-> Allow command post I allow new security groups

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/3.png?raw=true)<br/><br/>

### 3. I created two ECS's, one on VPC 1 and one on VPC 2

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/5.png?raw=true)<br/><br/>

### 4. Create database (use RDS for mysql) in 3.VPC

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/4.png?raw=true)<br/><br/>

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/6.png?raw=true)<br/><br/>

### 5. I tried using “Remote Login” for ECS and pinging other ECS and RDS but failed.

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/8.png?raw=true)<br/><br/>

### 6. Create VPC-Peering between 1.VPC-2.VPC, 1.VPC-3.VPC and 2.VPC-3.VPC

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/9.png?raw=true)<br/><br/>

### 7. To use VPC-Peerings I have given the routing rules with Route table-> Add route

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/10.png?raw=true)<br/><br/>

### 8. By pinging the ECS and RDS again, I see that the pinging was successful.

![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/11.png?raw=true)<br/><br/>
![This is an image](https://github.com/enessoztrk/Huawei_Cloud_Project/blob/main/img/12.png?raw=true)<br/><br/>
