def AGENT_LABEL = null

node('master'){
	stage('set agent'){
		if (env.JOB_NAME == scmcheckjob1 ){
			AGENT_LABEL = 'any'
		} 
		else {
			println("master")
			AGENT_LABEL = 'any'
			println AGENT_LABEL
		}
	}
}


pipeline{
	agent $AGENT_LABEL
stages{
stage('welcome 1st stage') {
	steps{
	echo 'welcome to 1st stage'
	sh "printenv | sort"
	}
}
}
}
