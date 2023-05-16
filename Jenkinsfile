pipeline {
    agent any
    
//     tools {
//         maven 'Maven-3.9.2'
//     }
    
    stages {
        stage('Build') {
            steps {
                echo 'buiding the application...'
//                 sh './maven -v'
                sh './ry.sh'
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
