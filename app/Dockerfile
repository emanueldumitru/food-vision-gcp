FROM python:3.7

# Setup the working directory
WORKDIR /app

# Copy files
COPY . /app

#Install requirements
RUN pip install -r /app/requirements.txt

# Expose port 8080
EXPOSE 8080

# Run
ENTRYPOINT ["streamlit", "run", "app.py", "--server.port=8080", "--server.address=0.0.0.0"]