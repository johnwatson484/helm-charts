# Helm Charts
Helm chart repository

## Package Helm chart
`helm package PATH_TO_CHART`

## Add to repository
```
# clone repository
git clone https://github.com/johnwatson484/helm-charts.git

# COPY PACKAGE TO REPOSITORY ROOT

# re-index repository
helm repo index . --merge ./index.yaml

# commit changes
git add .
git commit -m "Chart added"
git push
```

## Use chart from repository
```
# add helm repository
helm repo add helm repo add johnwatson https://johnwatson484.github.io/helm-charts/

# update helm repo index
helm repo update

# apply chart
helm install DEPLOYMENT_NAME johnwatson/HELM_CHART_NAME
```
