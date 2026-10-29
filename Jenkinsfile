node{
    git branch: 'main', url: 'https://github.com/mohamedahmedfayed2002/projenkins.git'
    stage ('build'){
        try{
        sh 'echo "build stage"'
        } catch (Exception e) {
            sh"build stage failed"
            throw e
        }
    }
    stage ('Test'){
        if (env.BRANCH_NAME == "Feat") {
            sh 'echo "test stage"'
            return
        }
        else {
            sh 'echo "skipe test stage"'
        }
    }
    
}