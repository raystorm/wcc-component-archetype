WCC-Component-Archetype
=======================

This is a Maven Archetype designed to make spinning up new components for 
Oracle WebCenter Content (WCC) faster and easier.

It creates a basic repository layout, `pom.xml` file and common template files.
Eliminating the need to use ComponentWizard to create basic components.

**Note** This generates maven projects that use

```xml
<depencency>
  <groupId>org.ucmtwine</groupId>
  <artifactId>ucm-maven-plugin</artifactId>
</dependency>
```

Which means it also assumes the `ucm-maven-plugin` dependencies are available at the same maven coordinates.

```xml
<dependency>
  <groupId>com.oracle.wcc</groupId>
  <artifactId>idcserver</artifactId>
  <version>11.1.1</version>
  <scope>provided</scope>
</dependency>
<dependency>
  <groupId>com.oracle.wcc</groupId>
  <artifactId>ridc</artifactId>
  <version>[11.1.1,12.0.0.0)</version>
</dependency>
<dependency>
  <groupId>com.oracle.weblogic</groupId>
  <artifactId>wlfullclient</artifactId>
  <version>10.3.6</version>
  <optional>true</optional>
</dependency>
```
