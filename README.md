# eclipse-sts-configurations
Recommended STS configurations for code formatter, checkstyle, etc. 

# Checkstyle
Eclipse's checktyle plugin, differs from `checkstyle.xml` used through maven's plugin when enabling `SuppressionCommentFilter` module. `checkstyle-eclipse-STS.xml` has Eclipse STS compatible configuration.
In order to allow checkstyle suppression, surround your code with these comments.
```
//CHECKSTYLE:OFF
public void someMethod(String arg1, String arg2, String arg3, String arg4) {
//CHECKSTYLE:ON
```

# Code Conventions/Formatter for the Eclipse STS
Go `to Window / Preferences`, filter by `formatter` then go to the `Java / Code Style / Formatter` option. Add the `codestyle-3.x.xml` file located in this repo. This file will apply formatter's with rules according to checkstyle configuration.
