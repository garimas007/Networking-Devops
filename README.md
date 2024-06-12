<H3>Project Statement -</H3>
  - deploy the server in 2 availability zones by using "auto scalling group" and "application load balancer". 
  - server receive requests through load balancer.
  - server connect to internet by using NAT gateway.
  - deploy NAT gateway in both zones. <br>
<H3>Solutions - </H3><br>

creating vpc : <br>
<img width="359" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/4d2be84e-79d9-4414-8125-7b283f2b7862"><br>

NAT gateway : <br>
<img width="344" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/dec1c834-6685-4d76-8994-1e6951b01f9b"><br>

subnet configuration map : <br>
<img width="775" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/7360ce4d-7d2c-418c-8d99-7feb2f181164"><br>

creating Auto Scaling Group : <br>
<img width="557" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/5c6063ef-f004-40be-a536-9877fd122040"><br>

<img width="529" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/e35fdaa0-fbd3-48ac-937f-d7c33f4c49f7"><br>

<img width="550" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/3665cb1e-89de-44aa-bd73-45bc64661d77"><br>

<img width="554" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/48d5cc55-48f7-4bf3-9633-4a16afe1668a"><br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/462e18b7-be0d-43a2-8fce-41446284e651) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/a27b5c05-5579-44c9-850d-7bdb9230a966) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/4bb16330-c2ea-4ffd-b3c4-648c66ce48e5) <br>

![image](https://github.com/garimas007/Networking-Devops/assets/146625788/93c52c2d-c46d-4d77-94ce-739116fe0443) <br>

**Bastion-Host (Bridge between public and private subnet)** : <br>
