# Convertor App

This is a Python application that converts images to a PDF file.

## Build and Run

To build the Docker image, use the following command:

```bash
docker build -t my-converter .

```wsl
docker run -v $(pwd)/images:/app/images -v $(pwd)/output:/app/output my-converter images
docker run -v $(pwd)/images:/app/images -v $(pwd)/output:/app/output -e PDF_NAME=mypics my-converter images