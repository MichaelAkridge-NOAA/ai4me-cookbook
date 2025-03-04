# Use a lightweight Python 3.10 image
FROM python:3.10-slim

# Set the working directory inside the container
WORKDIR /app

# Copy all files from the host to the container's "/app" directory
COPY ./ ./

# Install Label Studio and dependencies
RUN pip install label-studio

# Expose port 8080 for the Label Studio web interface
EXPOSE 8080

# Command to run Label Studio
ENTRYPOINT ["label-studio", "start", "--port", "8080", "--host", "0.0.0.0"]