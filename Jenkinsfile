// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent {
        kubernetes {
            // label "jenkins"
            namespace "jenkins-kub-quota"
            yamlFile 'kubernetesPod.yaml' 
            defaultContainer 'jnlp'
        }
    }
    stages {
        stage('build') {
            steps {
                echo "BUILDIG WITH CONTAINER WITH MULTIPLE CONTAINERS"
            }
        }
    }
}

