pipeline {
    agent any
    
    tools {
        maven 'maven'
    }
    
    stages {
        stage('Build') {
            steps {
                echo 'buiding the application...'
                sh 'mvn install'
//                 sh './ry.sh'
            }
        }
        
        stage("test"){
            steps {
                echo 'testing the application...'
            }
        }
        stage("deploy"){
            steps {
                echo 'deploying the application...'
            }
        }
    }
    
//      post {
//         always {
//             echo 'One way or another, I have finished'
//             mail to: 'jianhuazhang66@163.com',
//              subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
//              body: "Something is wrong with ${env.BUILD_URL}"
//         }
//      }
}
