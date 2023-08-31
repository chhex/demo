Demos a Openrewrite Error with Maven Multi Module Projects and Profiles

To reproduce:

1

```.\mvnw.cmd clean package

```

2

```.\mvnw.cmd clean package -P!InclB

```

3

```.\mvnw.cmd rewrite:run

```

4

```.\mvnw.cmd rewrite:run -P!InclB

```

-> 1 : Maven builds and tests both Modules -> correct

-> 2 : Maven builds and tests on Module A -> correct

-> 3 : Openrewrite runs rules on both Modules -> correct

-> 4 : Openrewrite run rules on both Modules, but should them only on Module A -> wrong

