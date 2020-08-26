all: HelloWorld.java
	javac -cp $$(for i in $$(find /usr/share/lwjgl/ -name '*.jar'); do echo -n $$i: ; done). HelloWorld.java
run:
	java -cp $$(for i in $$(find /usr/share/lwjgl/ -name '*.jar'); do echo -n $$i: ; done). HelloWorld
jar: HelloWorld.class manifest.txt
	jar cvfm  app.jar manifest.txt HelloWorld.class
jar-run: app.jar
	java -jar app.jar
clean:
	rm *.class
