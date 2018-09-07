node {
    try {
        stage('Checkout') {
              // To be added to shared libraries
              //
              //checkout scm
              //checkout changelog: false, poll: false, \
              //scm: [$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: \
              //   [[$class: 'ScmName', name: 'gradle']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'Database', \
              //   url: 'https://github.com/spineo/groovy-gradle-project.git']]]
        }
        
        stage('Clean') {
            sh "./gradlew clean"
        }
        
        stage('Build') {
           echo 'Build'
        }

        stage('Testing') {
            echo 'Testing'
        }

        stage('Staging') {
            echo 'Deploy Stage'
        }
        stage('Deploy') {
            echo 'Deploy Stage'
        }
  } catch (e) {
    currentBuild.result = "FAILED"
    throw e
  } finally {
    echo 'Success'
  }
}
