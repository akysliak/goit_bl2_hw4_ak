To start the program, call:

    python main.py

To create a docker image, volume and start a docker container, run:

    docker build . -t simple-server
    docker volume create storage
    docker run -it --rm -p 3000:3000 -v storage:/app/storage simple-server
