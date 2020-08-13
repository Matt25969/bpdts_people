# README

## Instructions

To deploy the application first ensure that you have Docker installed, you can find instructions for a basic Ubuntu distro here:
https://docs.docker.com/engine/install/ubuntu/

You then need to run the following commands to start the Docker container:
```sh
docker build -t people .
docker run -p 5000:5000 people
```

Once the Container is in a running state you can hit the API with:
```sh
curl 127.0.0.1:5000/people/peopleInLondon
```

## Assumptions

- The result of the API call is an array of relevant people, this array could be further iterated over and manipulated
- 60 miles within a radius on London is assumed to be between 50 - 52 Latitude and -1 - 1 Longitude
