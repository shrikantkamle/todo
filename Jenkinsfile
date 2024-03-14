pipeline {

agent any
stages {
    stage ("build"){
        steps{
            sh 'docker build . -t node-todo-app'
        }
    }
    stage ("run"){
        steps{
            sh 'docker run -d -p 8000:8000 --name node-todo-app node-todo-app'
        }
    }    
}

}