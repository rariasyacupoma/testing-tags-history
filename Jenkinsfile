@Library('cbdc-jenkins-libs@CBDC-4016/rollback-deployment-tag') _

properties([[$class: 'JiraProjectProperty'], buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '5'))])

wdeployCommonServicesProject([
  name: 'testing-git-tags',
  namespace: 'testing-git-tags',
  envType: ENV_TYPE,
  dockerTag: DOCKER_TAG,
  useHistoricalGitTag: true,
  isRollbackDeployment: IS_ROLLBACK_DEPLOYMENT
])