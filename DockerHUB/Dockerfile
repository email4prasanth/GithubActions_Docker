# # Trying to build java image
# # check DockerHUB changed
# FROM openjdk:17-jdk-alpine
# WORKDIR /app
# COPY test-app.jar /app/test-app.jar
# CMD ["java","-jar","test-app.jar"]
# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any necessary dependencies listed in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 80 available to the world outside this container
EXPOSE 80

# Define environment variable
ENV NAME World

# Run app.py when the container launches
CMD ["python", "app.py"]

