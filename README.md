# Charts

## Adding new charts to the index
In order to add new charts, we first need to create the skeleton
- helm create [name]

We then go head and start filling out the skeleton, essentially making our sevice.

### Package all charts into tar.gz
- helm package *

### Create new index file
- helm repo index --url https://slim008.github.io/charts/ .
- git commit -am 'Updated index'; git push origin main

## Trying out new chart in repo
- helm repo update
- helm search repo [name]

## Removing charts
- Remove the tar.gz file
- Update the index
- git commit -am 'Removed chart'; git push origin main
