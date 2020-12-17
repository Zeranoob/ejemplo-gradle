pipeline {
	agent any 

	parameters { choice(name: 'herramienta', choices: ['gradle','maven'], description: '') }

	stages {
		stage('Pipelines') {
			steps {
				script {

					params.herramienta // -> gradle o maven

					if(params.herramienta == 'gradle'){
						//invocacion a gradle.groovy
					} else {
						//invocacion a maven.groovy	
					def ejecucion = (params.herramienta == 'gradle') ? (load 'gradle.groovy') : (load 'maven.groovy')
				}
			}
		}
	}
}
