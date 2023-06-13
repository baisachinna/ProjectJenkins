pipeline{
	agent {
		def AGENT_LABEL = null
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
