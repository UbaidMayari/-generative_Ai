# base image
FROM continuumio/miniconda3:latest

LABEL maintainer="ameen@gmail.com"

# Copy app, templates and views
COPY . /app

# Set working directory for subsequent commands
WORKDIR /app

# Install dependencies
RUN pip install -r requirements.txt

EXPOSE 8080

# Command to run when container starts
ENTRYPOINT ["python", "app/app.py"]