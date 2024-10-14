FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy everything into /app
COPY . .

# Install Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 8080 for the API
EXPOSE 8080

# Run the FastAPI app with Uvicorn
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8080"]


# to run the postgresql database image
# docker run --name database --network project-net -p 5432:5432 -e POSTGRES_DB=student -e POSTGRES_PASSWORD=password -e POSTGRES_USER=postgres -d postgres

# to build the api image
# docker build -t project1-api .

# to run the api image
# docker run --name project1-api-run --network project-net -p 8080:8080 -d project1-api