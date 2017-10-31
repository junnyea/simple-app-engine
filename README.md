# simple-app-engine

This example demonstrate how to deploy a Spring Boot Application to Google App Engine.

1. Download Spring Boot App from https://spring.io/guides/gs/rest-service/
2. Add app.yaml to src/main/appengine/app.yaml (Needed by AppEngine)
3. Add in plugin for in build.gradle
  a. dependencies {
  classpath("com.google.cloud.tools:appengine-gradle-plugin:1.3.0") //Added for Google App Engine
  }
  b. apply plugin: 'com.google.cloud.tools.appengine' //Added for Google App Engine
4. Git Clone to AppEngine
5. Run GAE commands <br>
  a. Test: Gradle bootRun <br>
  b. Deploy: Gradle appengineDeploy
  
  
  Alternatively, you may check out this git.
  
  Go Google Cloud Shell
  1. git clone https://github.com/junnyea/simple-app-engine.git
  2. Gradle appenginedeploy
  
  ** Prerequities
  1. Install latest gradle in Google Shell e.g. gradle update
      a. use SDKMAN for installation : e.g. curl -s "https://get.sdkman.io" | bash
      b. sdk install gradle 4.2.1
  2. Latest Java Version
