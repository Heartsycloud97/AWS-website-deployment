 🚀 AWS Infrastructure in 3 Hours



One command. Two servers. Production-ready infrastructure

[Full story on Medium]



 💥 What This Does

Deploys a load-balanced website across 2 AWS servers with one Ansible command.


      Internet
          ↓
  Load Balancer
     ↙       ↘
  EC2 #1   EC2 #2


Refresh the page → watch the server IP change. That's real load balancing. 🔄


 ⚡ Quick Start

1. Clone it
bash
git clone https://github.com/Heartsycloud95/aws-website-deployment.git
cd aws-website-deployment


2. Add your servers to inventory.ini
ini
[webservers]
webserver1 ansible_host=YOUR_IP_1 ansible_user=ubuntu ansible_ssh_private_key_file=~/.ssh/key.pem
webserver2 ansible_host=YOUR_IP_2 ansible_user=ubuntu ansible_ssh_private_key_file=~/.ssh/key.pem

[webservers:vars]
ansible_python_interpreter=/usr/bin/python3


3. Deploy
bash
ansible-playbook -i inventory.ini deploy-website.yml


Done: Visit your ALB DNS or EC2 IP. 🎉


 🎯 Skills Unlocked

✅ AWS EC2 & Load Balancing  
✅ Ansible Automation  
✅ NGINX Configuration  
✅ Infrastructure as Code  

The difference? Most tutorials show one server. This builds scalable infrastructure.



💰 Cost

With Free Tier: $0/month  
After: ~$38/month  
Worth it? Absolutely. 💎

---

🛠️ Stack

AWS EC2 • Application Load Balancer • S3 • Ansible • NGINX



🔥 Why This Matters

This isn't a toy project. This is production-grade architecture used by real companies.

EC2 vs S3? Load balancing? High availability? You'll get it by doing it.

Full Tutorial

[Read the complete guide on Medium] with screenshots, mistakes, and lessons learned.


🚨 Troubleshooting

403 Error? → Security group needs port 80  
Ansible fails? → chmod 400 your-key.pem  
Unhealthy targets? → Check NGINX is running


 💬 Connect

⭐ Star if this helped you!  
Questions? Open an issue or find me on Medium



From zero AWS knowledge to deployed infrastructure in one weekend.

Built with ☕ and determination
