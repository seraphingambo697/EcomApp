node {
    stage('Clone') {
        git 'https://github.com/seraphin-git/EcomProject.git'
    }
    stage('Build') {
        sh 'javac Main.java'
   }
   stage('Run') {
        sh 'java Main'
   }
}
