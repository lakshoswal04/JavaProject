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
                    script{
                   
                    echo "delivering..."
                           // bat './deliver.sh'
                      // bat  './scripts/deliver.bat'
                    }
                }
            }
        
    }
}
