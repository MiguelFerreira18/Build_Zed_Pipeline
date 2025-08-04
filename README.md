# Simple Jenkins pipeline to build Zed code editor

## What it does?
- Checks out the Zed repository from GitHub.
- Builds the Zed code editor as a release executable.

## What it does not do?
**Does not install the needed dependencies for Zed**:
- Cargo
- Windows SDK
- C++ Build Tools
- CMake


## How to use it?
1. Make sure Java 17 is installed
2. Start the Jenkins war file with ```java -jar jenkins.war```
3. Open your web browser and go to `http://localhost:8080` to access the Jenkins dashboard.
4. Use ```ZED``` as User name and ```ZED1234``` as the password to log in.
5. Run the existing pipeline job if you don't want to create a new one.
6. Check the artifacts in the build job or the ``` <USER>/.jenkins/workspace/Build Zed/target/release ``` directory.

<details>
<summary>Configuration</summary>
<b>Note</b>: If you don't want to use this repository as the source for your pipeline, you can fork this repo, then change the github url in the configuration tab of the pipeline to your repository. (I won't be changing the configs of the jenkins.war so forking shouldn't ever break your own config.)

</details>



## Work for the future until Zed is available as a binary release
- Install dependencies during the pipeline

