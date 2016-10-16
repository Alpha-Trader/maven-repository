# maven-repository
Contains all maven artifacts related to the www.alpha-trader.com browsergame.

## How do I use this repository?

Simple, add the following lines to your project pom.xml:

    <repositories>
        <repository>
            <id>alpha-trader-repository</id>
            <url>https://raw.githubusercontent.com/Alpha-Trader/maven-repository/master/</url>
            <snapshots>
                <enabled>true</enabled>
                <updatePolicy>always</updatePolicy>
            </snapshots>
        </repository>
    </repositories>
    
Now you can include all the artifacts you need by declaring it in the dependencies, e.g. the entry for the API wrapper:

    <dependency>                                                                
        <groupId>com.alphatrader.rest</groupId>                                                  
        <artifactId>atrest-java</artifactId>                                            
        <version>0.9.0</version>                                                   
    </dependency>
