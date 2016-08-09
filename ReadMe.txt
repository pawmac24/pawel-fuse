Camel Router Project for Blueprint (OSGi)
=========================================

To build this project use

    mvn install

To run the project you can execute the following Maven goal

    mvn camel:run

To deploy the project in OSGi. For example using Apache ServiceMix
or Apache Karaf. You can run the following command from its shell:

    osgi:install -s mvn:com.mydemo/pawel-fuse/1.0.0-SNAPSHOT

For more help see the Apache Camel documentation

    http://camel.apache.org/


//Ewentualnie do generowania plikow z xsd

xjc -d src/main/java -p com.mydemo.pawelfuse.model data/xsd/HouseInfo.xsd data/xsd/CustInfo.xsd