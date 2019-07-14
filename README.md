# ansi_ec2_apache_2
export AWS_ACCESS_KEY_ID= 
export AWS_SECRET_ACCESS_KEY=

ansible-playbook -i ./hosts spinawsec2.yml 

Other way to run ansible playbook--
ansible-playbook spinawsec2.yml -e instance_type=t2.micro -e security_group=WebServers -e image=ami-0080e4c5bc078760e -e region=us-east-1 -e keypair=NVirginia -e count=1
