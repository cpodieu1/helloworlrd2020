pipeline {
    agent any
    tools {
        maven 'M2_HOME'
    }
    stages {
      stage('Build'){
        steps {
          echo "Build step"
          sh 'mvn clean'
          sh 'mvn install'
          sh 'mvn package'
        }
      
      
      }
        stage('test '){
        steps {
          echo "test step"
          sh 'mvn test'
        }
      
      
      }
        stage('deploy'){
        steps {
          echo "deploy war file"
         sshPublisher(publishers: [sshPublisherDesc(configName: 'Docker-host', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: 'docker rmi chrony:1.0; docker build -t chrony:1.0 . ; docker tag eu/chrony:1.0 ; docker pushchrony:1.0 podi podieu/chrony:1.0', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '', remoteDirectorySDF: false, removePrefix: 'webapp/target', sourceFiles: '**/*.war')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
        }
      
      
      }
    
    }

}

