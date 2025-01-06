
# Add API using Maven

```xml
<repositories>
  <repository>
      <id>luckydrops-repo</id>
      <url>https://pingu-io.github.io/luckydrops-api/</url>
  </repository>
</repositories>
```

```xml
<dependencies>
  <dependency>
      <groupId>io.pingu</groupId>
      <artifactId>luckydrops-api</artifactId>
      <version>1.14</version>
  </dependency>
</dependencies>
```
# How to use the API

```java
LuckyDropsAPI luckyDropsAPI = LuckyDropsAPI.getApi();

Location location = new Location(Bukkit.getWorld("world"), 0.0, 0.0, 0.0);
Template template = new Template("templateid", 10, "e0a443e0eca7f5d30622dd937f1e5ea2cdf15d10c27a199c68a7ce09c39f6b69");

luckyDropsAPI.spawnLuckyDrop(location, "luckydropid", template);    
luckyDropsAPI.removeLuckyDrop("luckydropid");
```
