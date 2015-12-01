# swagger_wiremock

First generate a swagger.json file for your JaxRs project with this Maven plugin:

            <plugin>
                <groupId>com.sebastian-daschner</groupId>
                <artifactId>jaxrs-analyzer-maven-plugin</artifactId>
                <version>0.9</version>
                <executions>
                    <execution>
                        <goals>
                            <goal>analyze-jaxrs</goal>
                        </goals>
                        <configuration>
                            <backend>swagger</backend>
                            <deployedDomain>localhost</deployedDomain>
                        </configuration>
                    </execution>
                </executions>
            </plugin>


Find the swagger.json file inside target and replace the empty swagger.json file under wiremock/json/

To build and run:  docker-compose build && docker-compose up

View your API :)
