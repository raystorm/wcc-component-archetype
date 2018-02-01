WCC-Component-Archetype
=======================

This is a [Maven Archetype](https://maven.apache.org/guides/introduction/introduction-to-archetypes.html) designed to make spinning up new [components](https://docs.oracle.com/middleware/12213/wcc/webcenter-content-develop/GUID-3259ABFD-F7F8-4F89-8CA1-C622870878CF.htm#WCCDV139) for [Oracle WebCenter Content](http://www.oracle.com/technetwork/middleware/webcenter/content/downloads/index.html) (WCC) faster and easier.

It creates a basic repository layout, `pom.xml` file and common template files. Eliminating the need to use [ComponentWizard](https://docs.oracle.com/middleware/12213/wcc/webcenter-content-develop/GUID-3259ABFD-F7F8-4F89-8CA1-C622870878CF.htm#GUID-84A0079F-FB2A-4649-95E9-DDD95A0F25F4) to create basic components.

**Note** This generates Maven projects that use the following:

```xml
<depencency>
  <groupId>org.ucmtwine</groupId>
  <artifactId>ucm-maven-plugin</artifactId>
</dependency>
```

Which means it also assumes the [ucm-maven-plugin](https://github.com/raystorm/ucm-maven-plugin) dependencies (as seen below) are available at the same Maven coordinates.

```xml
<dependency>
  <groupId>com.oracle.weblogic</groupId>
  <artifactId>wlfullclient</artifactId>
  <version>10.3.6</version>
  <optional>true</optional>
</dependency>
```
