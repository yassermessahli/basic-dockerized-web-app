FROM python:3.9-slim

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
# docker build -t project1-client .

# to run the web-app container
# docker run --name project1-client-run -d -p 8090:5000 project1-client