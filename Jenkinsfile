def AGENT_LABEL = null

pipeline{
	agent {
		if (${AGENT_LABEL} == null){
			label any
		}
		
	}

stages{
stage('welcome 1st stage') {
	steps{
	echo 'welcome to 1st stage'
	sh "printenv | sort"
	}
}
}
}
