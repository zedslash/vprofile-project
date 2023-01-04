pipeline {
    
	agent any
/*	
	tools {
        maven 'MAVEN3'
		jdk "OracleJDK"
    }
*/	
    environment {
        SNAP_REPO = 'project-snapshot'
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'admin123'
		RELEASE_REPO = 'project-release'
		CENTRAL_REPO = 'project-maven_central'
        NEXUSIP = '10.1.12.154'
		NEXUSPORT = '8081'
		NEXUS_GRP_REPO = 'Project_maven_groupes'
        NEXUS_CREDENTIAL_ID = 'nexuslogin'
    }
	
    stages{
        
        stage('BUILD'){
            steps {
                sh 'mvn -s setting.xml -DskipTests install'
            }
        }
    }


}
