Gradle JAXB plugin
==================

Fork of JaxB Gradle Plugin from [Stian Hegglund] (http://github.com/stianh/gradle-jaxb-plugin)
to deploy a 'released' version of latest HEAD in my [own public Github repository] (http://tomask-de.github.io/).


Usage
-----

    apply plugin: 'jaxb'

    dependencies {
      jaxb 'com.sun.xml.bind:jaxb-xjc:2.2.4-1'
    }

    buildscript {
      repositories {
        maven {
            http://tomask-de.github.com/repo/releases
        }
        mavenCentral()
      }
      dependencies {
        classpath 'de.tomask.gradle.jaxb:gradle-jaxb-plugin:2.1'
      }
    }
