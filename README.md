Project Statement -
  - deploy the server in 2 availability zones by using "auto scalling group" and "application load balancer". 
  - server receive requests through load balancer.
  - server connect to internet by using NAT gateway.
  - deploy NAT gateway in both zones. <br>
Solutions - <br>

creating vpc : <br>
<img width="359" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/4d2be84e-79d9-4414-8125-7b283f2b7862"><br>

NAT gateway : <br>
<img width="344" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/dec1c834-6685-4d76-8994-1e6951b01f9b"><br>

subnet configuration map : <br>
<img width="775" alt="image" src="https://github.com/garimas007/Networking-Devops/assets/146625788/7360ce4d-7d2c-418c-8d99-7feb2f181164"><br>

creating Auto Scaling Group : <br>
