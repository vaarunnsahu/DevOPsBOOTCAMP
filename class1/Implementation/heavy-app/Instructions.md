docker-compose build
docker-compose up -d

or 
docker-compose up --build 

# Access the app

Main application: http://localhost:8080

Monitoring dashboard: http://localhost:8000

# CPU-intensive stress
docker-compose run --rm -e STRESS_LEVEL=cpu-intensive stress-generator

# Memory-intensive stress
docker-compose run --rm -e STRESS_LEVEL=memory-intensive stress-generator

# Extreme stress (everything)
docker-compose run --rm -e STRESS_LEVEL=extreme stress-generator