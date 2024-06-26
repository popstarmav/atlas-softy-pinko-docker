# Use the latest Ubuntu image as the base
FROM ubuntu:22.04

# Update APT and upgrade all existing packages
RUN apt-get update
RUN apt-get upgrade -y

# Install python3 and pip
RUN apt-get install -y python3 python3-pip

# Remove unnecessary files after installation
RUN apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

# Set the working directory inside the container
WORKDIR /app

# Copy the api file into the container
COPY api.py /app/api.py

# Use pip to install flask
RUN pip3 install flask

# Use pip to install flask-cors
RUN pip3 install flask-cors

# Expose port for flask
EXPOSE 5252

# run flask on exposed port
CMD ["python3", "/app/api.py"]