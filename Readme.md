
#Cucumber Features from maven command line Example
to run the default configured <code>@CucumberOptions</code>

###Cucumber 6.10.4

to run the tests using maven, a simple `mvn clean test` will execute all the annotated `@RunWith` tests

to run other feature files then the ones defined in `@CucumberOptions` it is possible overwrite the folder/file location using

`mvn clean test -Dcucumber.features=otherFeature`

###Cucumber 4.8.1

if you need to run an older version of cucumber, setting cucumber.version on `pom.xml` to 4.8.1 f.e. the execution of distinct tests can be achieved with the command:

`mvn clean test -Dcucumber.options="otherFeature"`
