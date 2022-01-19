### Releasing a new version of the chart
1. Before release new chart, run following to test helm chart
   1. ```helm template .\microservice -f {{ values.yaml }}```
   2. ```helm lint```
2. Bump the version in [Chart.yaml][chart]
3. Generate and publish the chart
   1. ```helm package .\microservice\```
4. Create the Release in Github
   1. Click Draft a new release
   2. 