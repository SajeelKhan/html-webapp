pipeline { 
agent any 

    tools{
        nodejs 'node-16'
    }

    stages { 
        stage ('Build') { 
            steps {
                echo 'This is Build stage'
            }
 
        }
        stage ('Test') { 
            steps {
                echo 'This is Test stage'
            }
        
        }
        stage ('Deploy') { 
            steps{
                echo 'This is Deploy stage'
                sh 'cd /var/www/sajeel-pipeline'
                sh 'rm index.html'
                sh 'cp index.html /var/www/sajeel-pipeline'
            }
        }         
    }           
 }