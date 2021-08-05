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
                sh 'rm -f /var/www/sajeel-pipeline/index.html'
                sh 'scp index.html /var/www/sajeel-pipeline'
            }
        }         
    }           
 }