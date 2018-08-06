//mydata = readYaml file: "config.yml"
@Grab('org.yaml:snakeyaml:1.17')
import org.yaml.snakeyaml.Yaml
import org.yaml.snakeyaml.DumperOptions
import static org.yaml.snakeyaml.DumperOptions.FlowStyle.BLOCK

node {
    yaml = readYaml file: "config.yml"
    //yaml.data.info = 'hello world!'
    //writeFile file:"test.yml", text:yamlToString(yaml)
}
