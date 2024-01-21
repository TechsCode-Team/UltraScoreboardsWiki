# Ultra Scoreboards API Documentation

## Introduction

The Ultra Scoreboards API allows you to integrate the scoreboards system and other features of Ultra Scoreboards into your plugin. This documentations provides information on how to import the API library, find the latest version, obtain the API instance, and how to use the API instance.

## Importing the API

We provide importation of the API’s using our personally hosted library repository manager. This allows you to import the API using Maven and Gradle for easy access around the world.
<br>

To add the Ultra Scoreboards API library to your project you need to add the following information to your `package.xml`.

To use the Ultra Scoreboards API, add the following repository and dependency information to your project’s build file:

```xml
<repositories>
    <repository>
        <id>techscode</id>
        <url>https://repo.techscode.com/repository/techscode-apis/</url>
    </repository>
</repositories>

<dependency>
    <groupId>me.TechsCode</groupId>
    <artifactId>UltraScoreboardsAPI</artifactId>
    <version>VERSION</version>
    <scope>provided</scope>
</dependency>
```

Make sure to replace `VERSION` with the desired version. You can browse available versions **[here](https://repo.techscode.com/#browse/browse:techscode-apis:me%2FTechsCode%2FUltraScoreboardsAPI)**.

## Getting the API Instance

To obtain an instance of the Ultra Scoreboards API, use the following method:

```java
UltraScoreboardsAPI api = UltraScoreboards.getAPI();
```

This instance provides various methods for managing economic features, which are explained in detail on the other pages of this API documentation.