
Demos a Openrewrite Error with Maven Multi Module Projects

To reproduce: 

1 .\mvnw.cmd clean package
2 .\mvnw.cmd clean package -P!InclB
3 .\mvnw.cmd rewrite:run
4 .\mvnw.cmd rewrite:run -P!InclB
