node('download') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/thanigaiarasu-jagadeesan/july1.git'
	}
    stage('Continuous Build') 
	{
    sh label: '', script: 'mvn package'
	}
   }
