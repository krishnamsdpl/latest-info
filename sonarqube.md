Azure DevOps server - build agents
If you are using Microsoft-hosted build agents then there is nothing else to install. The extension will work with all of the hosted agents (Windows, Linux, and macOS).

If you are self-hosting the build agents, make sure you have at least the minimum SonarQube-supported version of Java installed.

Adding a new SonarQube service endpoint
After installing your extension, you need to declare your SonarQube server as a service endpoint in your Azure DevOps project settings:

In Azure DevOps, go to Project Settings > Service connections.

Select New service connection and then select SonarQube from the service connection list.
Enter your SonarQube Server URL, an authentication token, and a memorable Service connection name. Then, select Save to save your connection.


Configuring branch analysis
After adding your SonarQube service endpoint, you'll need to configure branch analysis. You'll use the following tasks in your build definitions to analyze your projects:

Prepare analysis configuration: This task configures the required settings before executing the build.
Run code analysis (Not used in Maven or Gradle projects): This task executes the analysis of source code.
Publish quality gate result: This task displays the quality gate status in the build summary letting you know if your code meets quality standards for production.
This task may increase your build time as your pipeline has to wait for SonarQube to process the analysis report. It is highly recommended but optional.
