pipeline
{
agent any
stages{

    stage('scm checkout'){
        steps{ sh 'echo code_is_downloading'}
    }

    stage('build the code'){
        steps{
            sh 'echo code_is_building'
            sh 'echo code_is_passed' }
    }
	
    stage('deploy to dev envt'){
	steps{ sh 'echo deploy_artifact_to_dev_envt'}
    }
    stage('Deploy to QA envt'){
	steps{ input 'Please approve QA deployment' }
	
	}
    stage('Deploy to QA Envt'){
	steps{ sh'echo deploying_to_QA_envt'}
	}		
     }

}
