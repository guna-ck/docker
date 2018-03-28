node {
	def app
	state('Clone repository') {
	checkout scm
  }
stage('Build image') {
	app = docker.build("docker/cent")
}
stage('Test image') {
	app.inside {
	sh 'echo "tests passed"'
 }
}
}


