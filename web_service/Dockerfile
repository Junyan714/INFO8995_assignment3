# Use a minimal Python image
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Installation
RUN apt-get update && apt-get install -y curl && pip install Flask && apt-get clean

# Copy application files
COPY app.py config.txt /app/

# Expose the port
EXPOSE 5000

# Run the app
CMD ["python", "app.py"]

