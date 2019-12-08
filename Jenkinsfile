node {
   
   stage('Preparation') { 
       git credentialsId: 'github', url: 'https://github.com/pdpwarriors/node-jenkins-app-example.git'
   }
   stage('code execution') { 
       nodejs('nodejs13.3') {
    sh 'npm install'
}
   }
   stage('code test') { 
       nodejs('nodejs13.3') {
    sh 'npm test'
}
   }
    stage('code test') { 
       nodejs('nodejs13.3') {
    sh 'npm sonar:sonar'
}
   }
}
