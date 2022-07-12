pipeline {
	agent any
	stages {
		stage('scan') {
			steps {

				sh "docker run -v ${workspace}:/src --workdir /src returncorp/semgrep-agent:v1 semgrep-agent --config p/ci"
			}
		}
	}
}
