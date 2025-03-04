# Use the official Label Studio image
FROM heartexlabs/label-studio:latest

# Set working directory
WORKDIR /label-studio

# Create necessary directories and set permissions
RUN mkdir -p /label-studio/data/media \
    && mkdir -p /label-studio/data/export \
    && mkdir -p /label-studio/data/uploads \
    && mkdir -p /label-studio/config \
    && chmod -R 777 /label-studio/data /label-studio/config

# Set environment variables
ENV LABEL_STUDIO_LOCAL_FILES_SERVING_ENABLED=true
ENV LABEL_STUDIO_LOCAL_FILES_DOCUMENT_ROOT=/label-studio/data

# Start Label Studio when the container runs
CMD ["label-studio"]