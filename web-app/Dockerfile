FROM python:3.9-slim

# Install curl
# RUN apt-get update && apt-get install -y curl

# Set the working directory in the container
WORKDIR /app

# Copy everything into /app in the container
COPY . .

# Install Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose Flask's default port
EXPOSE 5000

# Run the app with Python
CMD ["python", "app.py"]

# to build the web-app image
# docker build -t web-app-image ./web-app


# to run the web-app container
# docker run -d --name web-app --network project-net -e API_URL=http://api:8081 -p 8090:5000 web-app-image