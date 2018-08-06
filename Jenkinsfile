
@Grab('org.yaml:snakeyaml:1.17')
import org.yaml.snakeyaml.Yaml
readTrusted 'config.yaml'
pipeline {
    agent any

    stages {
        
       //  stage ('Compile Stage') {
        stage('Central Build') {
            agent any
            when { branch 'master' }
             data = readYaml file: "config.yaml"
        }
             

          //  steps {
               // withMaven(maven : 'maven-3.5.3') {
               //     sh 'mvn clean compile'
              //  }
           // }
      //  }

       // stage ('Testing Stage') {

            //steps {
                //withMaven(maven : 'maven-3.5.3') {
                 //   sh 'mvn test'
                //}
           // }
      //  }


       // stage ('Deployment Stage') {
           // steps {
               // withMaven(maven : 'maven-3.5.3') {
                 //   sh 'mvn deploy'
                // }
           // }
       // }

            stage ('Validation Stage') {
            steps {
               bat 'inspec exec https://github.com/Ramachari787/inspec/archive/Ram.zip'
                    
  }
}
}
}
