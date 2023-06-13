def AGENT_LABEL = null

node('built-in'){
	stage('set agent'){
		if (env.JOB_NAME == 'scmcheckjob1' ){
			AGENT_LABEL = 'built-in'
		} 
		else {
			println("master")
			AGENT_LABEL = 'built-in'
			println AGENT_LABEL
		}
	}
}


pipeline{
	agent { label AGENT_LABEL }
stages{
stage('welcome 1st stage') {
	steps{
	echo 'welcome to 1st stage'
	sh "printenv | sort"
	}
}
}
}
