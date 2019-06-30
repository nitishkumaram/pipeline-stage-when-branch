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

//  L17. Pipeline stage when changelog

// pipeline{
//     agent any

//     stages{
//         stage('Build'){
//             when{
//                 changelog '.*some_text.*'
//             }

//             steps{
//                 echo "====++++Hello World Changelog++++===="
//             }
//         }
//     }
// }

//  L18. Pipeline stage when changeRequest

// pipeline{
//     agent any

//         stages{
//             stage('Build'){
//                 when{
//                     changeRequest()
//                 }

//                 steps{
//                     echo "====++++Hello World Changing Request++++===="
//                 }
//             }
//         }
// }

//  L19. Pipeline stage when changeset

pipeline{
    agent any

    stages{
        stage('Build'){
            when{
                changeset glob: "*WORLD.js", caseSensitive: true
            }

            steps{
                echo "====++++Hello World when change set++++===="
            }
        }
    }
}
