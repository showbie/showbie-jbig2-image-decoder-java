JBIG2-Image-Decoder
=============================

This is a fork of [JPedal's JBIG2 library](http://www.jpedal.org/support_JBIG.php), 
which aims to improve the performance of the original code.

Results
-----------------------------

Version 1 (09.10.2011):

In all samples we have tested, the decoding speed has increased at least by 
factor 2.5.
In some examples a speed up by factor 4.5 was observed.

There is still lot of room for improvements especially in the combine method 
in JBIG2Bitmap, which is most time consuming. 

## Showbie Maven Central
 ```xml
<dependency>
    <groupId>com.showbie</groupId>
    <artifactId>showbie-jbig2-image-decoder</artifactId>
    <version>1.0.0-SNAPSHOT</version>
</dependency>
```

Publishing to Showbie's github maven central please ensure you created your personal access token. Follow these instructions located here: https://github.com/showbie/maven-central-repository

To publish enter the following command:

GITHUB_REGISTRY_USERNAME=<username> GITHUB_REGISTRY_TOKEN=<your personal access token> mvn deploy
