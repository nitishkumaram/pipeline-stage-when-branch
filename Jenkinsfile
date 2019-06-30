// pipeline{
//     agent any

//     stages{
//         stage('Build Master'){
//             when{
//                 branch 'master'
//             }
//             steps{
//                 echo "====++++Building master++++===="
//             }
//         }

//         stage('Build Dev'){
//             when{
//                 branch 'dev'
//             }
//             steps{
//                 echo "====++++Building Dev++++===="
//             }
//         }
//     }
// }

//  Pipeline stage when changelog

pipeline{
    agent any

    stages{
        stage('Build'){
            when{
                changelog '.*some_text.*'
            }

            steps{
                echo "====++++Hello World Changelog++++===="
            }
        }
    }
}
