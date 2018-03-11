[![license](https://img.shields.io/badge/gradle-4.6-brightgreen.svg)](https://gradle.org)
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit-license.php)

#  [FastJson](https://github.com/alibaba/fastjson)  integration  with springboot

FastJson-Spring-Boot-Starter 帮助你集成通用 [FastJson](https://github.com/alibaba/fastjson) 到 Spring Boot。

FastJson-Spring-Boot-Starter will help you use [FastJson](https://github.com/alibaba/fastjson) with Spring Boot.

## How to use

### maven

在pom.xml加入nexus资源库（解决中国访问慢的问题,已经加入中央仓库）

Add the following nexus repository(fix china access slow problem,already append to central nexus.)  to your pom.xml:

    <repositories>
        <repository>
            <id>nexus</id>
            <name>nexus</name>
            <url>http://maven.cuisongliu.com/content/groups/public</url>
            <releases>
                <enabled>true</enabled>
            </releases>
            <snapshots>
                <enabled>false</enabled>
            </snapshots>
        </repository>
    </repositories>

在pom.xml加入依赖

Add the following dependency to your pom.xml:
    
    <dependency>
       <groupId>com.cuisongliu</groupId>
       <artifactId>fastjson-spring-boot-starter</artifactId>
       <version>1.0</version>
     </dependency>

### gradle

在build.gradle加入nexus资源库（解决中国访问慢的问题,已经加入中央仓库）

Add the following nexus repository(fix china access slow problem,already append to central nexus.)  to your build.gradle:

    allprojects {
        repositories {
            mavenLocal()
            maven { url "http://maven.cuisongliu.com/content/groups/public" }
            mavenCentral()
            jcenter()
        }
    }
    
在build.gradle加入依赖

Add the following dependency to your build.gradle:
    
    compile "com.cuisongliu:fastjson-spring-boot-starter:1+"
    

## Acknowledgments

 [FastJson](https://github.com/alibaba/fastjson).