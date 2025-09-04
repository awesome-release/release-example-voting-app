FROM python:2.7-alpine

WORKDIR /app

# Copy application files
COPY . .

# Install dependencies
RUN pip install -r requirements.txt

# Expose application port
EXPOSE 80

# Start the app
CMD ["gunicorn", "app:app", "-b", "0.0.0.0:80"]
