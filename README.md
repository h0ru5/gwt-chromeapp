# gwt-chromeapp

A CSP-conforming linker for GWT and a wrapper for the chrome.app.* libs

## Usage
with Maven/IVY/Gradle/... 
you add it to your project's dependencies (its on maven central and sonatype OSS):

```xml
    <dependency>
			<groupId>com.github.h0ru5.gwt</groupId>
			<artifactId>gwt-chromeapp</artifactId>
			<version>x.y.z</version>
	</dependency>
```
you also need to inherit it in your .gwt.xml:
```xml
    <inherits name="com.github.h0ru5.gwt.chromeapp" />
```
It will add a CSP-Safe (content security policy) linker based on ```xsi```, allowing you to use GWT in chrome apps.

After compilation, you can include your *.nocache.js into your chrome app without having to sandbox it.


