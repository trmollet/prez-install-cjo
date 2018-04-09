Check that at least one developer knows **Java** language :

````java
boolean atLeastOneKnowsJava = team.stream()
                .map(d -> d.getLanguages())
                .flatMap(l -> l.stream())
                .anyMatch(l -> "java".equals(l));
````