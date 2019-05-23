# AutomatizacionDesarrolloSoftware
Linea de automatización de desarrollo de software

Repositorio relacionado con el uso de JUnit, Cucumber y JMeter para el desarrollo de una calculadora en JAVA

## Integrantes:
Jaime Santana Santana - 20132020212


Oscar Hernandez Cepeda - 20152020019


Juan Sanchez Mancilla - 20152020020


-----------------------------------------------------------------------------------------------------

# Para el archivo BeanShell-Sampler.jmx


Use Eclipse External Tool


Eclipse menu: Run -> External Tools -> External Tools Configuration...


The dialog External Tools Configuration opens


From the tree on the left select Program


Use left mouse button and select from the mouse menu New or use the left icon (above the tree) and select New launch configuration


On the right side of the tree, opens the panel, where details of this new lauch configuration can be filled in


Enter as Name: JMeter sample


Enter as Location: The location where JMeter is installed (on windows something like C:\Program Files\apache\jmeter\bin\jmeter.bat) (on Linux like /opt/apache/jmeter/bin/jmeter)


Enter as Working Directory: ${workspace_loc:/jmeter-project} (use the button Browse Workspance..., to select the project, in your workspace where the JMeter script are located. Here the project jmeter-project is shown)


Close the dialog by using the button Run, which should launch JMeter.


Info The icon Stop, does not work, as this actually launches a script, which launches the Java application JMeter.


Optionally add parameters


Enter as Arguments: -t src\test\jmeter\sample.jmx (the path of the JMeter script to launch)


Enter as Arguments: -q src\test\jmeter\environment.properties (some external properties file, use ${__P(key-name)})
