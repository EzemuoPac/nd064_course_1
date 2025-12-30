FROM python:3.8

LABEL maintainer="your-email@example.com"

# Set the working directory
WORKDIR /app

# Copy application files
COPY . /app

# Install dependencies
RUN pip install -r requirements.txt

# Initialize the database
RUN python init_db.py

# Expose port 3111
EXPOSE 3111

# Run the application
CMD ["python", "app.py"]