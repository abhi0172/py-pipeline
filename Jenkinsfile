pipeline {
	agent {
		label 'python-pipeline'
		}
	stages {
		stage ("pull scm python test") {
			steps {
				git branch: 'python', url: 'https://github.com/abhi0172/py-pipeline.git'
				}
			}
		stage ("Build") {
			steps {
				sh 'python3 -V'
				sh 'python3 cp.py'
				}
			}
		stage ("Test") {
			steps {
				sh 'python3 test.py'
				}
			}
		}
	}
