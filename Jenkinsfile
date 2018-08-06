        stage('Read YAML file') {
        steps {
            script{ datas = readYaml (file: 'config.yaml') }
            echo datas.ear_file.deploy.toString()

        }
    }
}
