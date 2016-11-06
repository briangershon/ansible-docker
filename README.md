# About

Run Ansible via Docker.

## Give it a try

    docker run -it --rm brianfive/ansible-docker ansible --version
    docker run -v `pwd`/example:`pwd` -w `pwd` -it --rm brianfive/ansible-docker ansible-playbook example.yml

## How to build docker image

    docker build -t ansible-docker .
    docker images
    docker tag <image-hash-goes-here> brianfive/ansible-docker:latest
    docker push brianfive/ansible-docker

## References

Initial Alpine-based Python Docker image from https://github.com/jfloff/alpine-python/blob/master/2.7/Dockerfile
