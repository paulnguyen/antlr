

# ANTLR 

* https://www.antlr.org/
* https://www.antlr.org/tools.html


## Downloads & Source

* https://www.antlr.org/download.html
* https://github.com/antlr/antlr4


## OS X Setup


	$ cd /usr/local/lib
	$ sudo curl -O https://www.antlr.org/download/antlr-4.7.2-complete.jar
	$ export CLASSPATH=".:/usr/local/lib/antlr-4.7.2-complete.jar:$CLASSPATH"
	$ alias antlr4='java -jar /usr/local/lib/antlr-4.7.2-complete.jar'
	$ alias grun='java org.antlr.v4.gui.TestRig'


## Java Target

	ANTLR tool and Java Target

	    Complete ANTLR 4.7.2 Java binaries jar. Complete ANTLR 4.7.2 tool, Java runtime and ST 4.0.8, which lets you run the tool and the generated code.
	    ANTLR 4.7.2 distribution (zip). Everything you need to build the tool and Java runtime from source.
	    ANTLR 4.7.2 Java runtime binaries jar. Only what's needed for building and executing parsers/lexers generated in Java. 

	The Java jars are OSGi compatible so you should be able to use them within Eclipse.

	To use maven, refer to group ID org.antlr and artifact ID antlr4 for the tool itself and antlr4-runtime for the Java runtime library in your pom.xml file. The latest version is 4.7.2:

	<dependency> 
	  <groupId>org.antlr</groupId> 
	  <artifactId>antlr4</artifactId> 
	  <version>4.7.2</version> 
	</dependency> 


	See ANTLR 4 Maven plugin, ANTLR 4 Maven plug-in usage, and ANTLR 4 Maven Plugin API.

	ANTLR v4 is written in ANTLR v3.5.2 and StringTemplate 4.0.8. In antlr-4.7.2-complete.jar, you'll find everything you need to run the ANTLR tool and make its generated parsers work.


## Go Target

	Go Target

	Install it on your GOPATH via: go get github.com/antlr/antlr4/runtime/Go/antlr 