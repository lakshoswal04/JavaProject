pipeline{
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage("Build"){
            steps{
            bat 'mvn -B -DskipTests clean package'
            }
        }
            stage("Test"){
                steps{
                    bat 'mvn test'
                }
            }
            stage("Deliver"){
                steps{
                    echo "delivering..."
                         // bat '/deliver.sh'
                
                }
            }
        
    }
}
