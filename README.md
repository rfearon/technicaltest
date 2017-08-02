# technicaltest
Contact us scenario automated- QA works

# Prerequistes
Download JDK and set directory to JAVA_HOME environment variable
Download and install apache-maven-3.3.9 and set directory to MAVEN_HOME variable
Download IntelliJ and install 'Cucumber for Java' plugin- File>Settings>Plugins
Download junit version 4.10 and set environment variable as JUNIT_HOME
Download Git bash command editor
Download Version 37.0 of Mozilla Firefox

# Instructions how to run code
Run command in Git bash to clone project- git clone https://github.com/rfearon/technicaltest/
Extract zip folder dev2
Open project in IntelliJ and navigate to dev2>src>test>java>cucumberTest
Right-click on contactUsScenario.feature and click the Run 'Feature: contactUsScenario'
The test will then proceed to launch and you shoud the actions being performed

# Dependencies
 <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>2.47.1</version>
    </dependency>
    <dependency>
        <groupId>info.cukes</groupId>
        <artifactId>cucumber-java</artifactId>
        <version>1.2.5</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>info.cukes</groupId>
        <artifactId>cucumber-junit</artifactId>
        <version>1.2.5</version>
        <scope>test</scope>
    </dependency>

    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.11</version>
        <scope>test</scope>
    </dependency>

# Highlights
Although quite a basic test I like the actions are perforned in the browser and there is a feature file written in Gherkin so as to make it readable to someone who is not strong technically.

# Improvements
There are a few things I would've loved to improve about the test with more time. I would've liked to have covered some negative scenarios in cucumber to cover for example where the data is correct, for example an email address that doesn't exist, a number that is accidently entered as part of the name or the button being clicked with some fields as null. I would have therefore made the feature file a Scenario Outline as opposed to a Scenario and stored the data within a data table so once again it is easy to read.

I have not configured the test to be run as part of test runner where it can be executed from the command line. Also ideally with more time if this could have been paackaged up to run from a more user friendly system such as Jenkins this would be mean there would not need to be as many pre-requisites.

# Bug
I noticed when running the test the web browser opens multiple firefox browsers.

