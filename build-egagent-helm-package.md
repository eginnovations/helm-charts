# eG Agent Helm Package Building Steps
## Clone the repo

    git clone https://github.com/eginnovations/helm-charts.git
    cd helm-charts

## Make your chart changes inside of egagent directory  

    helm lint egagent
    mkdir -p repos/new_charts
    helm package -u -d repos/new_charts egagent
    helm repo index repos/new_charts --url "https://eginnovations.github.io/helm-charts/repos/stable/" --merge index.yaml 

## Update original repo

    mv repos/new_charts/egagent-*.tgz repos/stable
    mv repos/new_charts/index.yaml index.yaml
    rm  -rf repos/new_charts

## Create commit on repo

    git add -A
    git commit -m "updated charts"
    git push


## (For Testing Purpose) Create YAML Output using local repo

	helm template egagent ./egagent --namespace egagent --set EG_MANAGER=<MANAGER_IP>  --set EG_MANAGER_PORT=<MANAGER_PORT>  --set EG_MANAGER_SSL=<true/false> --output-dir ./egagent-helm-output

	