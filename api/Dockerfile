FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy everything into /app
COPY . .

# Install Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 8080 for the API
EXPOSE 8081

# Run the FastAPI app with Uvicorn
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8081"]


# to run the postgresql database image
# docker run --name database --network project-net -p 5432:5432 -e POSTGRES_DB=student -e POSTGRES_PASSWORD=password -e POSTGRES_USER=postgres -d postgres

# to build the api image
# docker build -t api-image ./api


# to run the api image
# docker run --name api-run --network project-net -p 8081:8081 -d api-image