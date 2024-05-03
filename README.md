# Container-MonitorX - Streamlined Monitoring for Containers
Container MonitorX is a project focused🎯on a container monitoring system using prometheus and grafana.The system offers real-time insights into container performance,assisting administrators in maintaining optimal resource utilization and addressing issues promptly.With a user-friendly grafana dashboard📊,Container MonitorX simplifies the monitoring process,providing key metrics📈for efficient container management.


📌 **Platform Used - AWS**

📌 **Tools Used - Docker,Docker Swarm,Prometheus,Grafana,cAdvisor**


🌐**Ports Numbers** - *Docker Swarm: 2377*,*Prometheus: 9090*,*Grafana: 3000*,*cAdvisor: 8080*,*Docker Deamon: 9323*,*Email Server – SMTP Gmail: 587*


![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/eae869a6-9d56-41d0-b3f7-a41ede164d4c)

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/5b807f23-146c-4448-adcd-8f7bab887425)



📌**Implementation**

📌**Create VPC**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/fff948fb-722e-4b48-bf79-06117c0f628b)

**VPC Successfully Created:**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/e00b0758-bd08-4710-838f-13f2826826cd)



📌 **Create EC2 Instances**

**Docker-Cluster-Master-1:**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/f6e28f61-7fea-4302-985c-49ac65643f2c)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/584834cf-a4fa-49dc-9b8b-90a792f53aa8)


**Docker-Cluster-Master-2**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/c944b0ec-d41e-4fd7-b340-d36908c29588)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/045b7762-4dca-41b6-95ae-f3ce23393959)


**Docker-Cluster-Node-1**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/ef64a775-2ed2-40f7-9395-c2e929af5b56)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/f7dc1e4a-b255-475d-a840-66b17d4dde66)


**Docker-Cluster-Node-2**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/372b224a-e17a-4935-9daa-ef2da0fbe1ff)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/c85275a7-f8ba-4873-848e-4ac231e4f408)


**Docker-Cluster-Node-3**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/7c980c55-b35d-4d8f-b230-a68b97eb53ea)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/150328a6-62bb-47cc-ab13-b64c8295cbca)


 📌**Prometheus-Grafana-server**
 
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/6c929c6c-2739-4220-8f4b-3569ab6bbec6)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/d0a7c227-c1bb-4ab2-a4cb-55fbfeb16cb1)


📌 **ALL EC2 Instances**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/8fff0201-e61a-44e1-ba21-e6e2f70d185c)


📌 **Connect to every docker node using private key and run shell script that contains docker installation steps:**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/11e81d64-bc0c-41c5-b93c-818bdc21f8ad)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/0f2bc990-1574-4464-8248-a9f789c14d32)



📌 **NOTE: Install Docker, Grafana and Prometheus Using above given scripts**



⚡**Make script executable by running: chmod +x install_docker.sh**

⚡**Then you can run script: ./install_docker.sh**


📌**Docker service running successfully**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/41c66ae4-450a-4b7c-b1c2-b689715ef7e6)



📌**Security Group for Docker Swarm Cluster Master and Nodes**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/fb2bca94-1d0c-4198-beba-84f2d46c1067)



📌**Docker Swarm installation**

> sudo docker swarm init --advertise-addr 10.0.137.150 (Master IP)
(A token will get generated)
> sudo docker node ls
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/71497ab1-dd52-4263-96d7-6b0b1c8889a5)


📌**Docker Swarm with 2 Master and 3 Worker Nodes**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/5a98f090-3263-4143-bb79-c08d7fd7d024)


📌**Prometheus Installation using Shell Script**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/7d6ad8c7-d5bc-4413-9441-11e001473ae5)


📌**Prometheus Service running successfully**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/7d9c9ed4-1aab-4870-88e3-8c46c91078f1)


📌**Grafana Installation using Shell Script**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/f4ac6c2b-d7ea-4274-93de-1c98300dedf3)


📌**Grafana Service running successfully**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/7bd75aec-4807-4cdf-8171-6d01daa62aa4)


📌**To access Interface Prometheus and Grafana**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/99c5524a-7d88-4c6e-a331-d7c94cce6eac)


📌**Prometheus Interface**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/673b18fa-c103-4cae-930d-5487517e9be2)


📌**Grafana Interface**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/bb12964a-109c-4c1c-bbfa-e3f5129dd26b)



📌**Run cAdvisor container on every node to get metrics**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/97a4cc1a-d593-47fa-8f27-a68526955c71)
![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/c61f742f-09b8-4b84-82e4-9fd13bc07099)


📌**Prometheus Configuration File**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/c2406eee-c36b-4d93-ad27-0bc11b80d6d2)


📌**Prometheus Interface Connection**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/1b82e914-33ef-4f54-b53b-7d2cda0605e4)


📌**Connect Grafana to Prometheus**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/abdcb95a-b81d-47c4-8339-df25cb6994ea)


📌**Grafana Dashboard**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/aec0511e-9e2c-4954-b4d0-a56cf9edccce)


📌**SMTP Configuration for getting alert emails**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/bce18066-a91d-4910-a02f-7ba4d76a946e)


📌**Alert if any node goes down**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/0c978540-1d34-4bf7-a406-c0eb76fc46a6)


📌**Get Email if any nodes goes down**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/cf9b08d2-fd1d-4e5c-8e02-d81400d036d7)


📌**After resolve the alert**

![image](https://github.com/veenaparate/Container-MonitorX/assets/120020040/78da3dab-cfe0-4d09-bc1b-3952543667a6)



📌**Conclusion:**

In conclusion,the successful establishment of a Docker Swarm Cluster intergrated with prometheus and grafana for monitoring and alerting within a secure Virtual Private Cloud (VPC) on AWS represents a significant achievement in building a robust and scalable infrastructure for containerized applications.

*This setup offers several key benefits like Scalability, Observability, Alerting, Security, Automation.*











