# Nextcloud in Docker  

This project demonstrates the deployment of the open-source Nextcloud platform using Docker. Nextcloud is a robust, self-hosted file-sharing and collaboration solution, ensuring data privacy and control. This setup provides a containerized environment for quick deployment and scalability.  

---

## Table of Contents  
1. [About the Project](#about-the-project)  
2. [Technologies Used](#technologies-used)  
3. [Prerequisites](#prerequisites)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Troubleshooting](#troubleshooting)  

---

## About the Project  
This project deploys a Nextcloud instance using Docker containers, leveraging the official Nextcloud Docker image from Docker Hub. This system provides an easy-to-use, private cloud storage platform, allowing users to manage files and collaborate securely in an isolated and lightweight environment.  

---

## Technologies Used  
- **Nextcloud**: Open-source file-sharing and collaboration platform.
![Screenshot 2024-12-07 232337](https://github.com/user-attachments/assets/10ab0531-d079-425d-bee2-842db7806894)
![Screenshot 2024-12-07 234614](https://github.com/user-attachments/assets/7ec0bed8-ab97-4b39-a293-065dc928ec4d)

- **Docker**: Containerization platform.
![Screenshot 2024-12-07 233728](https://github.com/user-attachments/assets/d892e6b6-15bd-468f-916a-7cff6878a11d)

- **Docker Hub**: Source for the official Nextcloud image.  

---

## Prerequisites  
Ensure the following software is installed on your machine:  
- Docker (version 20.10 or later recommended).
![Screenshot 2024-12-07 232750](https://github.com/user-attachments/assets/9600202f-0248-4b8d-9bb9-fcdc10b948f8)

---

## Installation  

### 1. Clone the Repository  
Clone this repository to your local machine:  
```bash  
git clone https://github.com/akanksha1711/Docker  
cd Docker  
```  

### 2. Pull the Nextcloud Docker Image  
The required image is pulled automatically when the container is created.  

### 3. Run the Docker Container  
Use the following commands to set up and run the Nextcloud container:  

#### Option 1: Create a default Nextcloud container  
```bash  
docker run -d --name nextcloud -p 8080:80 nextcloud  
```  

### 4. Access Nextcloud  
Open a web browser and go to:  
```  
http://localhost:8080  
```  
Follow the setup instructions to configure the Nextcloud instance.  

---

## Usage  
1. Navigate to the Nextcloud interface via your browser.  
2. Log in to the system using the credentials set during the setup process.  
3. Upload files, create folders, and manage user accounts.  
4. Explore Nextcloud's apps for extended functionality, such as calendar, notes, or tasks.  

---

## Troubleshooting  

1. **Port Conflict**: Ensure port `8080` is not in use by another application.  
   - If the port is busy, change the port mapping when running the container (e.g., `-p 8081:80`).  

2. **Stopping the Container**: To stop the container, use:  
   ```bash  
   docker stop nextcloud  
   ```  

3. **Removing the Container**: To remove the container, use:  
   ```bash  
   docker rm nextcloud  
   ```  

4. **Logs**: Check logs for debugging:  
   ```bash  
   docker logs nextcloud  
   ```  

---
