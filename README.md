# Atlassian Agent

#### Support (almost any version):
* JIRA Software
* JIRA Core
* JIRA Service Desk
* JIRA plugin: Capture
* JIRA plugin: Training
* JIRA plugin: Portfolio
* Confluence
* Confluence plugin: Questions
* Confluence plugin: Team Calendars
* Bamboo
* Bitbucket
* FishEye
* Crowd
* Crucible

## Instructions for use

### Advantage
* Supports almost all products of Atlassian family, and supports plug-ins at the same time.
* Support DataCenter mode.
* Compared with the traditional crack, you can easily upgrade your service without having to crack it again.
* Provide java-based command line keygen, which is more convenient to use in the terminal environment.
* Open source projects, you know what you did when you cracked it.

### Download
* Download the release package of this project directly.

### Compile by yourself
* Clone the source code of this project, and the pom.xml `mvn package` can be compiled after execution in the same level directory .
> it works with JAVA 8 (openjdk-8-jdk)
```
  $ mvn compile
  $ mvn package
  $ java -jar target/atlassian-agent-jar-with-dependencies.jar
====================================================
=======        Atlassian Crack Agent         =======
=======           https://zhile.io           =======
=======          QQ Group: 30347511          =======
====================================================

KeyGen usage: java -jar
       /root/atlassian-agent/target/atlassian-agent-jar-with-dependencies.
       jar [-d] [-h] -m <arg> [-n <arg>] -o <arg> -p <arg> -s <arg>
 -d,--datacenter           Data center license[default: false]
 -h,--help                 Print help message
 -m,--mail <arg>           License email
 -n,--name <arg>           License name[default: <license email>]
 -o,--organisation <arg>   License organisation
 -p,--product <arg>        License product, support:
                           [crowd: Crowd]
                           [questions: Questions plugin for Confluence]
                           [crucible: Crucible]
                           [capture: Capture plugin for JIRA]
                           [conf: Confluence]
                           [training: Training plugin for JIRA]
                           [bitbucket: Bitbucket]
                           [tc: Team Calendars plugin for Confluence]
                           [bamboo: Bamboo]
                           [fisheye: FishEye]
                           [portfolio: Portfolio plugin for JIRA]
                           [jc: JIRA Core]
                           [jsd: JIRA Service Desk]
                           [jira: JIRA Software(common jira)]
 -s,--serverid <arg>       License server ID

================================================================================

# Crack agent usage: append -javaagent arg to system environment: CATALINA_OPTS.
# Example(execute this command or append it to setenv.sh/setenv.bat file): 

  export CATALINA_OPTS="-javaagent:/root/atlassian-agent/target/atlassian-agent-jar-with-dependencies.jar ${CATALINA_OPTS}"

# Then start your confluence/jira server.


```
* If you don’t know what I’m talking about, it’s best to download my compiled package directly.

### Using help
* If you have already obtained it `atlassian-agent.jar`, you can try to execute it and `java -jar atlassian-agent.jar` see the help output.
* The help here uses Atlassian's Confluence service as an example.

### Configure Agent
1. Put it `atlassian-agent-jar-with-dependencies.jar` in a location that you will not delete randomly (all Atlassian services on your server can share the same one `atlassian-agent.jar`).
2. Set the environment variable `CATALINA_OPTS` (this is actually the environment variable of Tomcat, used to specify the `-javaagent` parameters attached when starting the java program), and attach the parameters. Specifically, you can do this:
   * You can put: `export CATALINA_OPTS="-javaagent:/path/to/atlassian-agent-jar-with-dependencies.jar ${CATALINA_OPTS}"` such commands in `.bashrc` or `.bash_profile` such files.
   * You can put: `export CATALINA_OPTS="-javaagent:/path/to/atlassian-agent-jar-with-dependencies.jar ${CATALINA_OPTS}"` such a command in `bin目录` the `setenv.sh` or under the service installation `setenv.bat`（windows）.
   * You can also directly execute the command line: `CATALINA_OPTS="-javaagent:/path/to/atlassian-agent-jar-with-dependencies.jar" /path/to/start-confluence.sh` to start your service.
   * Or you know other ways to modify environment variables, but if you have irrelevant Tomcat services on your machine, it is not recommended to modify global `CATALINA_OPTS` environment variables.
3. If you want to verify whether the configuration is successful, you can do this:
   * Execute similar commands: `ps aux | grep java` find the corresponding process to see if the `-javaagent` parameters are correctly attached.
   * Similar to the software installation directory `/path/to/confluence/logs/catalina.out` : `========= agent working =========` The output of `:` should be found in the Tomcat log .
 
### Use KeyGen
* You have to confirm that the agent has been configured, refer to the above instructions
* When you try to execute `java -jar /path/to/atlassian-agent-jar-with-dependencies.jar` it, you should be able to see the output of the KeyGen parameter help.
* Please take a closer look at the function of each parameter, especially `-p` the value range of the parameter.
* When Atlassian service is installed, you should see a server id similar to: `AAAA-BBBB-CCCC-DDDD` , please pay attention.
* Running KeyGen with correct parameters will output the calculated activation code on the terminal.
* Copy the generated activation code to activate the service you want to use.

### Affirm
* This project is only for personal study and research purposes, and must not be used for commercial purposes!
* For commercial use, please purchase genuine from [Atlassian](https://www.atlassian.com) , thank you for your cooperation!
* This project uses an `GNU General Public License v3.0` open source license!
* It is not allowed to say that my code is poorly written. For me, it `PHP` is the best language in the world (to argue against it).


### communicate with
* Issue an issue to this project.
* You are welcome to improve this project together, please send a PR.
* You can join the QQ group: 30347511 and chat with me in real time.
* Visit the website: [https://zhile.io](https://zhile.io) Leave me a message.
