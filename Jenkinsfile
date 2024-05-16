pipeline { 
     agent any 
     stages { 
          stage("Compile") { 
               steps {
                    sh "chmod 777 gradlew"
                    sh "./gradlew compileJava" 
               } 
          }
            stage("Build") {
                         steps {
                              sh "./gradlew build"
                         }
                    }

          stage("Unit test") { 
               steps { 
                    sh "./gradlew test" 
               } 
          } 
     } 
} 
