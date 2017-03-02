# Docker Pushmi-Pullyu

A script to copy a Docker image directly to a remote host without using Docker 
Hub or a hosted registry.

The implementation pushes the image to a temporary local registry then pulls 
it to the remote host through an SSH tunnel. This takes advantage of Docker's 
layer-based cache to avoid superfluous network I/O.

![Dr. Dolittle's pushmi-pullyu](pushmi-pullyu.png)
