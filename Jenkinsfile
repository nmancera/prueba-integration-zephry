#!/usr/bin/env groovy

def params = [
    repository          : 'https://github.com/nmancera/prueba-integration-zephry.git',
    credentials         : 'github'
]

properties([
    pipelineTriggers([
        githubPush()
    ]),
    disableConcurrentBuilds()
])


node {
    try {
        echo 'Iniciando'
		checkout()
        zephyr()

    }
}


def zephyr{
	stage('validando zephyr'){
		// Iniciando seteo de variables
		// set accessKey="YWQ2OTVjZjEtMmY3OS0zZGU5LWEyZWUtY2Q4MDFhYmU4Y2VkIDVlNDE1ZTBjMzkzZWE5MGM5NGIyZjQ4MCBVU0VSX0RFRkFVTFRfTkFNRQ"
		// set secretKey="iyruR-clnwOVUeXoWgj91BGeLxV6LefSTh8HgV5kJuI"
		// set accountId="5e415e0c393ea90c94b2f480"	
		echo "prueba"
		}
	}
	
def checkout() {
    stage('Checkout') {
        checkout scm
    }
}
   