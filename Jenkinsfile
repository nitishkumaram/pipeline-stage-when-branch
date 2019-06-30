// 
//  L18. Pipeline stage when changeRequest

pipeline{
    agent any{

        stages{
            stage('Build'){
                when{
                    changeRequest()
                }

                steps{
                    echo "====++++Hello World Changing Request++++===="
                }
            }
        }
    }
}
