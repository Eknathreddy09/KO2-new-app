# Accelerator Log

## Options
```json
{
  "deploymentType" : "workload",
  "message" : "World",
  "projectName" : "ko2-app-hello"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┗ ┗ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [hello-world->ko2-app-hello]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'none') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[4].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [tap/catalog-info.yaml]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [tap/catalog-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-world->ko2-app-hello]
┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[5].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [tap/workload.yaml]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-world->ko2-app-hello, World->World]
┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].merge.transformations[0].sources[5].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┏ README (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(Append))
┃ ┃ ┃ ┃ README.merge (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┏ README.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [hello-world->ko2-app-hello]
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [tap/DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[2].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[2].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-world->ko2-app-hello]
┃ ┃ ┃ ┃ ┗ ┗ ┗ ╺ README.merge.transformations[0].sources[2].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┗ ┗ ╺ README.merge.transformations[1] (UniquePath)
┃ ┗ ╺ engine.transformations[0].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
