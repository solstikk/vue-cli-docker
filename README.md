# vue-cli-init-docker
Initialize projects with vue cli without having to install anything but docker locally.

1. Initialize "my-project" with the vue template "webpack":

  `docker run --name vue-cli-init -i gunnarbr/vue-cli-init-docker webpack my-project`

2. Copy the initialized project files to the host:

  `docker cp vue-cli-init:/my-project ./`

3. Remove the container with the initialized project:

    `docker rm vue-cli-init`

Your files should now be available in the my-project folder.
