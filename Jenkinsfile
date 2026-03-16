pipeline {
 agent any

 stages {

  stage('Clone') {
   steps {
    git branch: 'main', url: 'https://github.com/Fazil711/File-Encrypter.git'
   }
  }

  stage('Build') {
   steps {
    sh '''
    echo "Building Java project..."
    ls
    cd "Password Protection"
    mkdir -p build
    javac -d build src/*.java
    '''
   }
  }

 }
}
