# Variables
JC = javac
JV = java
CP = .:sodium.jar:swidgets-jdk-11.jar:swidgets.jar
JAVAFLAGS = -cp $(CP)
JCFLAGS = -Xlint:unchecked

# Targets
all: Example GpsGui

GpsGui: GpsGui.class
Example: Example.class

GpsGui.class: GpsGui.java
	$(JC) $(JAVAFLAGS) $(JCFLAGS) $<

Example.class: Example.java
	$(JC) $(JAVAFLAGS) $(JCFLAGS) $<

run: all
	$(JV) $(JAVAFLAGS) Example
	$(JV) $(JAVAFLAGS) GpsGui

gui: 
	$(JV) $(JAVAFLAGS) GpsGui

exp: 
	$(JV) $(JAVAFLAGS) Example

clean:
	rm -f *.class

.PHONY: all run clean
