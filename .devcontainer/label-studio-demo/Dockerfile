# Use a lightweight Python 3.10 image
FROM heartexlabs/label-studio:develop

# Set the working directory inside the container
WORKDIR /app

# Copy all files from the host to the container's "/app" directory
COPY ./ ./

# Expose port 8080 for the Label Studio web interface
EXPOSE 8080

ENV LABEL_STUDIO_DEPLOYMENT_TYPE=docker
ENV USE_ENFORCE_CSRF_CHECKS=0
ENV SESSION_COOKIE_SAMESITE=None
ENV CSRF_COOKIE_SAMESITE=None
ENV SESSION_COOKIE_SECURE=1

CMD exec label-studio --host=$SPACE_HOST