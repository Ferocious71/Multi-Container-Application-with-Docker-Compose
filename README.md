# Multi-Container-Application-with-Docker-Compose

1.	Create the Flask Application:
○	Write a Python Flask application (app.py) that increments a counter each time the page is refreshed. The Flask app should use Redis to store the counter value.
2.	Create the Dockerfile:
○	In the same directory, create a Dockerfile to containerize the Flask application.
3.	Set Up Redis Service:
○	Use Docker Compose to define a Redis service alongside the Flask application.
4.	Define Services in docker-compose.yml:
○	Create a docker-compose.yml file to define both the Flask app and Redis services.
5.	Test the Application:
○	Run docker-compose up to start both containers.
○	Access http://localhost:5000 in your browser and verify that the visit counter increments on page refresh.
