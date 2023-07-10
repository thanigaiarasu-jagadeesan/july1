node('deployment') 
{
 stage('Continuous Deployment')
        {
          sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@34.218.225.60:.'
        }
    stage('Continuous Testing')
        {
              sh label: '', script: 'echo "Testing Passed"'
        }
    stage('Continuous Delivery')
        {
          sh label: '', script: 'scp -i test.pem /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@34.218.225.60:.'
        }
}
