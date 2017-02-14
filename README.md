#xmlstarlet in pom.xml

#### Select multi prop
	xmlstarlet sel -N my=http://maven.apache.org/POM/4.0.0 -t -m my:project -v my:groupId -o : -v my:artifactId -o : -v my:version pom.xml
#### Select prop
	xmlstarlet sel -N my=http://maven.apache.org/POM/4.0.0 -t -m my:project -v my:groupId pom.xml
#### Update prop
	xmlstarlet ed -N p=http://maven.apache.org/POM/4.0.0 -u "/p:project/p:groupId" -v "br.com.linkapp" pom.xml > pom_new.xml
