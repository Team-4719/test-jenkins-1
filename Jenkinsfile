pipeline {
 agent any

 stages {
        stage('CreateVirtualEnv') {
            steps {
                virtualenv entorno_virtual
		source entorno_virtual/bin/activate
            }
        }
        stage('InstallRequirements') {
            steps {
                pip install -r requirements.txt
            }
        }        
  }

}

