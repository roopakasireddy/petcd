pipeline {
	agent any
    stages {
        stage('deploy-to-cluster ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=sureshkiran/my-pet --set image.tag=latest'
            }           
        }
    }
}
