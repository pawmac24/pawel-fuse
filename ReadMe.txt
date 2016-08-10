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

//W przegladarce wpisac adres do restfulowego serwisu np:
http://localhost:9090/route/summaryservice/customer/A234567


//deploy
1. Uruchomic fuse
fuse
2. W konsoli karafa wpisac:
fabric:create --wait-for-provisioning
3. Otworzyć konsolę
http://localhost:8181
4. Utworzyc kontener democontainer w konsoli jboss fuse i dodac full profile
5. mvn clean install
6. mvn fabric8:deploy

https://www.youtube.com/watch?v=dQGkAQCotPE&list=PLIS-R80eiu1sYyXHoCD7VlLQwHkuIwEdr&index=5
