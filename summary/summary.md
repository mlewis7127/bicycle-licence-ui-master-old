<a id="top"></a>

<p style="font-size: 24px;"><img src="./qct-icons/transform-logo.svg" style="margin-right: 15px; vertical-align: middle;"></img><b>Code Transformation Summary by Amazon Q </b></p>
<p><img src="./qct-icons/transform-variables-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Lines of code in your application: 2444 <p>
<p><img src="./qct-icons/transform-clock-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Transformation duration: 18 min(s) <p>
<p><img src="./qct-icons/transform-dependencies-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Planned dependencies replaced: 1 of 2 <p>
<p><img src="./qct-icons/transform-dependencyAnalyzer-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Additional dependencies added: 8 <p>
<p><img src="./qct-icons/transform-smartStepInto-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Planned deprecated code instances replaced: 0 of 0 <p>
<p><img src="./qct-icons/transform-listFiles-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Files changed: 7 <p>
<p><img src="./qct-icons/transform-build-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Build status in Java 17: <span style="color: #00CC00">SUCCEEDED</span> <p>

### Table of Contents

1. <a href="#build-log-summary">Build log summary</a> 
1. <a href="#planned-dependencies-replaced">Planned dependencies replaced</a> 
1. <a href="#additional-dependencies-added">Additional dependencies added</a> 
1. <a href="#deprecated-code-replaced">Deprecated code replaced</a> 
1. <a href="#other-changes">Other changes</a> 
1. <a href="#all-files-changed">All files changed</a> 
1. <a href="#next-steps">Next steps</a> 


### Build log summary <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="build-log-summary"></a>

Amazon Q successfully built the upgraded code in Java 17. Here is a relevant snippet from the build log. To view the full build log, open [`buildCommandOutput.log`](./buildCommandOutput.log)

```
The Maven build was successful in compiling, testing, packaging and repackaging the Java 17 application. No tests were found to run. The compile step showed an unchecked warning in the QLDBAjaxController class that should be reviewed.
```


### Planned dependencies replaced <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="planned-dependencies-replaced"></a>

Amazon Q updated the following dependencies that it identified in the transformation plan

| Dependency | Action | Previous version in Java 8 | Current version in Java 17 |
|--------------|--------|--------|--------|
| `org.springframework.boot:spring-boot-starter-parent` | Updated | 2.1.8.RELEASE | 3.2.7 |

### Additional dependencies added <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="additional-dependencies-added"></a>

Amazon Q updated the following additional dependencies during the upgrade

| Dependency | Action | Previous version in Java 8 | Current version in Java 17 |
|--------------|--------|--------|--------|
| `com.amazonaws:aws-java-sdk-core` | Updated | 1.11.628 | 1.12.486 |
| `com.amazonaws:aws-java-sdk-dynamodb` | Updated | 1.11.603 | 1.12.543 |
| `com.amazonaws:aws-java-sdk-qldb` | Updated | 1.11.693 | 1.12.543 |
| `com.amazonaws:aws-lambda-java-core` | Updated | 1.2.0 | 1.2.1 |
| `com.fasterxml.jackson.core:jackson-core` | Updated | 2.10.3 | 2.12.5 |
| `com.fasterxml.jackson.dataformat:jackson-dataformat-ion` | Updated | 2.10.3 | - |
| `org.apache.maven.plugins:maven-shade-plugin` | Updated | 2.4.3 | 3.3.0 |
| `org.projectlombok:lombok` | Updated | 1.18.12 | 1.18.20 |

### Deprecated code replaced <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="deprecated-code-replaced"></a>

Amazon Q replaced the following instances of deprecated code.

| Deprecated code | Files changed |
|----------------|----------------|


### Other changes <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="other-changes"></a>



### All files changed <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="all-files-changed"></a>

| File | Action |
|----------------|--------|
| [bicycle-licence-ledger-consumer/pom.xml](../bicycle-licence-ledger-consumer/pom.xml) | Updated |
| [pom.xml](../pom.xml) | Updated |
| [src/main/java/uk/gov/dvla/poc/controllers/HomeController.java](../src/main/java/uk/gov/dvla/poc/controllers/HomeController.java) | Updated |
| [src/main/java/uk/gov/dvla/poc/controllers/QLDBAjaxController.java](../src/main/java/uk/gov/dvla/poc/controllers/QLDBAjaxController.java) | Updated |
| [src/main/java/uk/gov/dvla/poc/repository/BicycleLicenceQLDBRepository.java](../src/main/java/uk/gov/dvla/poc/repository/BicycleLicenceQLDBRepository.java) | Updated |
| [src/main/java/uk/gov/dvla/poc/repository/LedgerConnection.java](../src/main/java/uk/gov/dvla/poc/repository/LedgerConnection.java) | Updated |
| [src/main/java/uk/gov/dvla/poc/repository/LicenceActivityDynamoRepository.java](../src/main/java/uk/gov/dvla/poc/repository/LicenceActivityDynamoRepository.java) | Updated |

### Next steps <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="next-steps"></a>

1. Please review and accept the code changes using the diff viewer.If you are using a Private Repository, please ensure that updated dependencies are available.
1. 
1. In order to successfully verify these changes on your machine, you will need to change your project to Java 17. We verified the changes using [Amazon Corretto Java 17](https://docs.aws.amazon.com/corretto/latest/corretto-17-ug/what-is-corretto-17.html
) build environment.