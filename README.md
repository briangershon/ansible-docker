Run Ansible via Docker.

## How to build

    docker build -t ansible-docker:latest .

## Examples

    docker run -it --rm ansible-docker:latest ansible --version

    docker run -v `pwd`/example:`pwd` -w `pwd` -it --rm ansible-docker:latest ansible-playbook example.yml

## References

Initial Alpine-based Python Docker image from https://github.com/jfloff/alpine-python/blob/master/2.7/Dockerfile
