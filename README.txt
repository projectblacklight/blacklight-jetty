HYDRA-JETTY
--------------------------
This is a copy of jetty pre-installed with various applications needed by hydra applications.
Most notably, these include fedora (http://fedora-commons.org/) and solr (http://lucene.apache.org/solr/).  

To run, use 

  java -jar start.jar

in this directory.  Note that java 1.6 must be invoked by the “java” command 
because Fedora requires it.

When jetty is finished initializing itself, Solr is available at 

  	http://localhost:8983/solr/admin/

and fedora is available at 

	http://localhost:8983/fedora/

You can see a list of all installed applications at http://localhost:8983

You can also change the port jetty starts on by editing the file etc/jetty.xml and changing this line to indicate a different port number:

<Set name="port"><SystemProperty name="jetty.port" default="8983"/></Set>


