pipeline
{
  agent any
  stages
  {
    stage ('executing commands')
    {
      steps
      {
        sh 'touch abc.txt'
        sh 'echo $JAVA_HOME'
        sh 'echo $MAVEN_HOME'
        tag = VersionNumber (versionNumberString: '${BUILD_DATE_FORMATTED, "yyyyMMdd"}-develop-${BUILDS_TODAY}')
      }
    }  
  }    
}        
      
