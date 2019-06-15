# AutomatizacionDesarrolloSoftware
Linea de automatización de desarrollo de software

Repositorio relacionado con el uso de JUnit, Cucumber y JMeter para el desarrollo de una calculadora en JAVA

## Integrantes:
Jaime Santana Santana - 20132020212


Oscar Hernandez Cepeda - 20152020019


Juan Sanchez Mancilla - 20152020020


-----------------------------------------------------------------------------------------------------

# Para el archivo BeanShell-Sampler.jmx


Usando: Eclipse External Tool


Enter as Arguments: -t src\test\jmeter\sample.jmx (the path of the JMeter script to launch)


Enter as Arguments: -q src\test\jmeter\environment.properties (some external properties file, use ${__P(key-name)})

# Entorno Docker

Para el uso y prueba del sistema se utiliza el entorno docker, por el cual se descarga una imagen y se almacena en un contenedor para su uso posterior, en este caso se procede asi:

Ejecucion de comandos:

sudo docker pull jsantanas/jenkinsud:version2

sudo docker run --name temporal jsantanas/jenkinsud /bin/true

sudo docker cp temporal:/jenkins_data.tar.bz2 /jenkins_data.tar.bz2

sudo docker rm temporal

sudo sudo docker volume create --name jenkins_data

sudo cat jenkins_data.tar.bz2 | docker run -i -v jenkins_data:/volume --rm loomchild/volume-backup restore -

docker run --name jenkinsgestion -d -v jenkins_data:/var/jenkins_home -p 8080:8080 -p 50000:50000 jsantanas/jenkinsud:version2

