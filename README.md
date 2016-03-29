 Assembly Descriptor for [WireMock](http://wiremock.org/) Stubs JAR
==============
 
 WireMock [stubs](http://wiremock.org/stubbing.html) are JSON documents placed in a file with a `.json` extension under the `mappings` directory.
 
### Usage

 
 ```
 <plugin>
     <artifactId>maven-assembly-plugin</artifactId>
     <version>2.6</version>
     <dependencies>
         <dependency>
             <groupId>io.codearte.accurest</groupId>
             <artifactId>stubs-assembly-descriptor</artifactId>
             <version>1.0</version>
         </dependency>
     </dependencies>
     <executions>
         <execution>
             <phase>package</phase>
             <goals>
                 <goal>single</goal>
             </goals>
         </execution>
     </executions>
     <configuration>
         <descriptorRefs>
             <descriptorRef>stubs</descriptorRef>
         </descriptorRefs>
     </configuration>
 </plugin>
 ```