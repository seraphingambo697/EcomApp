node {
  def app
    stage('Clone') {
        checkout scm
    }
    stage('Build image') {
        app = docker.build("seraph/nginx")
   }
   stage('Run image') {
        docker.image('seraph/ngnix').withRun('-p 80:80') { c -> 
        
        sh 'docker ps'
        
        sh 'curl localhost'
        }
   }
}
