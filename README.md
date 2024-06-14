<H3>Project Statement -</H3>
  - deploy the server in 2 availability zones by using "auto scalling group" and "application load balancer". 
  - server receive requests through load balancer.
  - server connect to internet by using NAT gateway.
  - deploy NAT gateway in both zones. <br>
<H3>Solutions - </H3><br>

**creating vpc :** <br>
<img width="359" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/4d2be84e-79d9-4414-8125-7b283f2b7862"><br>

**NAT gateway :** <br>
<img width="344" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/dec1c834-6685-4d76-8994-1e6951b01f9b"><br>

**subnet configuration map :** <br>
<img width="775" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/7360ce4d-7d2c-418c-8d99-7feb2f181164"><br>

**creating Launch Template for ASG :** <br>
<img width="557" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/5c6063ef-f004-40be-a536-9877fd122040"><br>

<img width="529" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/e35fdaa0-fbd3-48ac-937f-d7c33f4c49f7"><br>

<img width="550" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/3665cb1e-89de-44aa-bd73-45bc64661d77"><br>

<img width="554" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/48d5cc55-48f7-4bf3-9633-4a16afe1668a"><br>

**creating Auto Scaling Group :** <br>
![image](https://github.com/garimas007/Networking-Devops/assets/146625788/462e18b7-be0d-43a2-8fce-41446284e651) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/a27b5c05-5579-44c9-850d-7bdb9230a966) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/4bb16330-c2ea-4ffd-b3c4-648c66ce48e5) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/93c52c2d-c46d-4d77-94ce-739116fe0443) <br>

**Bastion-Host (Bridge between public and private subnet)** : <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/ed20836e-cfea-4977-9964-07a51e257505) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/48fb1f31-1623-4d1c-b8be-91ba7002e3a2) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/4b17c8b2-1779-4eff-b707-f59c9b027c1f) <br>

**SCP**: <br>
scp -i C:\Users\admin\Downloads\bastionhostdevopsnetwork.pem C:\Users\admin\Downloads\devopsnetwork.pem ubuntu@(public-ip-of-bastion-host):/home/ubuntu <br>
change the pem file permisiion to 400 for making it secure <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/449275ae-d034-40cc-9792-00468e081d59) <br>

**creating application load balancer :** <br>
Target Group for both private instance to creaate load balancer. <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/030a1550-ebcd-425c-8748-59c9190b394f) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/0bb58dc2-0d56-4819-9c33-d257645cc4f9) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/a93a4486-31bd-477b-95b6-d553593ffd75) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/d24518a9-0af4-4687-bc4b-89c6c0b9d873) <br>

**ASG :** <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/d744e143-0f16-4d9f-8d12-d2fc40a18624) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/bed3fb71-f9d8-493a-945e-cc87b1057e25) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/f002e33a-3a20-4de3-a91c-2ba1598d5d31) <br>

