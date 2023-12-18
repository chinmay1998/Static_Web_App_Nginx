Static Website Deployment on Nginx
	Launch a Jenkin instance
•	Install Jenkins and configure.
•	Allow 8080 port in the Security group.
•	su – Jenkins
•	ssh-keygen
•	ssh-copy-id ubuntu@public_ip_of_Nginx
•	
	Launch a Nginx instance
•	Install Nginxapt-get install nginx -y
•	Allow 80 port in the Security group.
•	vim /etc/ssh/sshd_config
•	PasswordAuthentication yes
•	sudo service ssh restart
•	sudo passwd ubuntu(set a password)
•	chmod 777 /var/www/html
