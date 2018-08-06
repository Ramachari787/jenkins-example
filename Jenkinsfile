      

//import org.yaml.snakeyaml.Yaml
readTrusted 'config.yaml'
pipeline {
    agent any

   // stages {
        
       //  stage ('Compile Stage') {
       // stage('Central Build') {
          //  agent any
            //when { branch 'master' }
            // data = readYaml file: "config.yaml"
      //  }
       stage('Read YAML file') {
        steps {
            when { branch 'master' }
            script{ datas = readYaml (file: 'config.yaml') }
            echo datas.ear_file.deploy.toString()

        }
    }
}
