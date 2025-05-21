# Multi-Container-Application-with-Docker-Compose

1.	Create the Flask Application:
-	Write a Python Flask application (app.py) that increments a counter each time the page is refreshed. The Flask app should use Redis to store the counter value.
2.	Create the Dockerfile:
-	In the same directory, create a Dockerfile to containerize the Flask application.
3.	Set Up Redis Service:
-	Use Docker Compose to define a Redis service alongside the Flask application.
4.	Define Services in docker-compose.yml:
-	Create a docker-compose.yml file to define both the Flask app and Redis services.
5.	Test the Application:
-	Run docker-compose up to start both containers.
-	Access http://localhost in your browser and verify that the visit counter increments on page refresh.

  🔧 Prerequisites -

  # For Docker
sudo apt update && sudo apt install -y docker.io
sudo systemctl start docker
sudo systemctl enable docker

# For Docker Compose
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" \
-o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

# Test the Application
sudo docker-compose up -d

- Mapping the internal port 5000 (Flask app) to the external port 80 means you can simply access your app via http://<public-ip> instead of http://<public-ip>:5000.

- sudo docker-compose up -d --build

![image](https://github.com/user-attachments/assets/033e3d1e-c253-4400-94be-44da2c52e13e)



