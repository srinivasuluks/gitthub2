node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'gitthub2') {

        def customImage = docker.build("srinivasuluks/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}