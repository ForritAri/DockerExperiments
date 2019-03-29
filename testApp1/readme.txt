
# Build the image
docker build -t arivesteinsson/myfirstapp .
docker images

# Run the image in a container
docker run -p 8888:5000 --name myfirstapp arivesteinsson/myfirstapp


# Push to the registry
docker login
docker push YOUR_USERNAME/myfirstapp

# Clean up
docker rm -f myfirstapp