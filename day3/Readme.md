
# Day 3 - VPC Lab

## Goal
Custom VPC (10.0.0.0/16) with public subnet (10.0.1.0/24), IGW, route 0.0.0.0/0 → IGW, EC2 + Nginx.

## ASCII Diagram
VPC 10.0.0.0/16
  └─ Public Subnet 10.0.1.0/24
       └─ EC2 (nginx, SG: 22,80)
Internet ↔ IGW ↔ RouteTable(0.0.0.0/0)

## Steps
- Created VPC & public subnet
- Attached IGW and added default route
- Launched EC2 with public IP
- Installed nginx and verified from browser

## Verify
- Browser: http://13.201.6.197
- Screenshots: 
<img width="1154" height="329" alt="image" src="https://github.com/user-attachments/assets/2731313f-5e68-464c-a336-97e33cb164d0" />

<img width="1919" height="860" alt="image" src="https://github.com/user-attachments/assets/cd32d559-d7bf-4751-8b48-eb4ca2cf8fb9" />

<img width="1919" height="887" alt="image" src="https://github.com/user-attachments/assets/214ee8a5-a1f7-452e-afaf-84dfc0bb97fb" />


