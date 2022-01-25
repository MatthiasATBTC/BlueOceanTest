pipeline {
  agent any
  stages {
    stage('gctsExecuteABAPUnitTests') {
        steps {    
       /* gctsDeploy(
          script: this,
          host: 'http://slaa9114.btcdev.btc-ag.int:8000',
          client: '100',
          abapCredentialsId: 'ABAPUserPasswordCredentialsId',
          repository: 'rereifsc-gcts4',
          remoteRepositoryURL: "https://github.com/rereifsc/gCTS4",
          verbose: true
        )
        */
          gctsExecuteABAPUnitTests(
          script: this,
          host: 'https://slaa9114.btcdev.btc-ag.int:8000',
          client: '100',
          abapCredentialsId: 'ABAPUserPasswordCredentialsId',
          repository: 'rereifsc-gcts4',
          scope: 'localChangedObjects',
          commit: "${GIT_COMMIT}",
          workspace: "${WORKSPACE}"
          )
      }
    }
  }
}
