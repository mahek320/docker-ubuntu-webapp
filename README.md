# 🚀 Deploy a Web Application in Docker Container 🐳  

## 📌 Project Overview  
In this project, we will:  
✅ Pull the **Ubuntu image** from Docker Hub.  
✅ Launch a **web application** inside a Docker container.  
✅ Expose the application on **port 8080**.  
✅ Ensure the application is **globally accessible** over the internet.  

Step 1: 

i. Launch an EC2 instance for docker and connect it to the terminal. 

<img src="https://github.com/user-attachments/assets/87b3d44a-79eb-4e2f-be82-6e456913d543" width="500"/><br><br>

ii. Add the listed protocols in the security group of your instance. 

<img src="https://github.com/user-attachments/assets/ad01c011-6722-4725-a868-e86bb7c53c6c" width="500"/><br><br>

iii. Connect to the terminal of your instance and set the hostname to docker.

<img src="https://github.com/user-attachments/assets/5cf409e3-086c-49c7-b207-a3d550f6e283" width="500"/><br><br>

iv. Run the below docker commands on the terminal to install docker.
<br>

```sh
    yum update -y 
    sudo yum install -y yum utils 
    sudo yum install docker -y 
    sudo systemctl start docker
    sudo systemctl enable docker
```
<br>
<img src="https://github.com/user-attachments/assets/36a63a79-d5c6-4d92-98a9-eb6c8e5ee28d" width="500"/><br><br>


v. We will now pull the unbuntu image using docker run command.


<img src="https://github.com/user-attachments/assets/b6aaa61a-b075-40ad-803f-0de1a8f69f17" width="500"/><br><br>


vi. We will now install and update the apache package. 
<br>
```sh
apt update -y
apt install apache2 -y
```


vii. We will change the directory and create a new html file in the terminal.



<img src="https://github.com/user-attachments/assets/6df4c9ed-7cde-45d9-b122-d1b0483633b4" width="500"/><br><br>


viii. We will start the apache after creating the html file in the same directory.
<br>
```sh
service apache start
```
<br>

ix. We will check the list of containers created using command 
<br>
```sh
docker ps -a
```
<br>
<img src="https://github.com/user-attachments/assets/1dd5fa48-6672-4857-8f93-549b94d4675c" width="500"/><br><br>


x. We will then copy the public IP address from the created instance and add :8080 after the IP address.
<br>

<img src="https://github.com/user-attachments/assets/55779084-952c-40b5-9395-d2cf01acec49" width="500"/><br><br>






