# Jenkins One

Launch a Jenkins instance on Docker.

## Create Jenkins Container

1. Create the container
    ```sh
    $ docker-compose -p jenkins_one up -d
    ```
2. Get the initial admin password from container initialization logs
    ```sh
    $ docker container logs jenkins_one_jenkins_blueocean_1

    ...
    Please use the following password to proceed to installation:

    89797dce076d48dc8ed640f2a14ad0ae

    This may also be found at: /var/jenkins_home/secrets/initialAdminPassword
    ...
    ```


## Notes

 - [Jenkins Docker Install Guide](https://jenkins.io/doc/book/installing/#docker)
 - [Build a Node.js and React app with npm](https://jenkins.io/doc/tutorials/build-a-node-js-and-react-app-with-npm/)
