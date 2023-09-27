# Accelerator Log

## Options
```json
{
  "bsGitBranch" : "main",
  "bsGitRepository" : "github.com?owner=x95castle1&repo=official-official",
  "conventionImageRegistry" : "registry.harbor.learn.tapsme.org/convention-service/official-official",
  "conventionPrefix" : "x95castle1.org",
  "packageLongDescription" : "awesome things",
  "packageMaintainer" : "dont-email-me@example.com",
  "packageName" : "official-official.tap.example.com",
  "packageShortDescription" : "enrich some stuff",
  "projectName" : "official-official",
  "releasePackageImageRegistry" : "registry.harbor.learn.tapsme.org/convention-service/official-official-repo-bundle",
  "stagingPackageImageRegistry" : "harbor-repo.vmware.com/tanzu_practice/conventions/official-official-repo-bundle"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ engine.transformations[0].validated.delegate (Chain)
┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Combo)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore]
┃ ┃ ┃ ┃ ┃ ┃ Debug .DS_Store didn't match [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug Makefile matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/.DS_Store matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/certificates.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/cluster-pod-convention.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/data-values-schema.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/deployment.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/namespace.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/openshift.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/overlay/add_namespace.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/reg-cred.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/config/service.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/package-build.yml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/package-resources.yml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug carvel/packagerepository/pkgrepo-build.yml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug convention.jpeg didn't match [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug examples/.DS_Store matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug examples/package/gitops/install-values.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug examples/package/gitops/packageinstall.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug examples/package/gitops/packagerepository.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug examples/package/values.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug examples/workload/workload-probes.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug go.mod matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug go.sum matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug hack/go.mod matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug hack/go.sum matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug hack/tools.go matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug install-server/server-it.yaml matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pkg/conventions/conventions.go matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pkg/conventions/conventions_test.go matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pkg/conventions/testdata/boms/bom.cdx.not_springboot.json matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pkg/conventions/testdata/templates/readinessProbe.json matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug server.go matched [**/*.go, **/go.mod, **/go.sum, pkg/**/*.json, README.md, Makefile, install-server/**, carvel/**, examples/**, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [ARTIFACT_ID_PLACEHOLDER->official-official]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [CONVENTION_IMAGE_REGISTRY_PLACEHOLDER_URL->registry.harbor.lear...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[3] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [STAGING_PACKAGE_IMAGE_REGISTRY_PLACEHOLDER_URL->harbor-repo.vmware.c...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[4] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [RELEASE_PACKAGE_IMAGE_REGISTRY_PLACEHOLDER_URL->registry.harbor.lear...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[5] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [PACKAGE_NAME_PLACEHOLDER->official-official.ta...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[6] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [PACKAGE_SHORT_NAME_PLACEHOLDER->official-official]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[7] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [PACKAGE_SHORT_NAME_PLACEHOLDER->official-official]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[8] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [PACKAGE_SUFFIX_PLACEHOLDER->tap.example.com]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[9] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [PACKAGE_LONG_DESCRIPTION_PLACEHOLDER->awesome things]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[10] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [PACKAGE_SHORT_DESCRIPTION_PLACEHOLDER->enrich some stuff]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[11] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [PACKAGE_MAINTAINERS_PLACEHOLDER->dont-email-me@exampl...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[12] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [CONVENTION_PREFIX_PLACEHOLDER->x95castle1.org]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[13] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [STAGING_REGISTRY_HOST->harbor-repo.vmware.c...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[14] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [RELEASE_REGISTRY_HOST->registry.harbor.lear...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[15] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [CONVENTION_IMAGE_REGISTRY_HOST->registry.harbor.lear...(truncated)]
┃ ┗ ┗ ╺ engine.transformations[0].validated.delegate.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
