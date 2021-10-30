## Clone the repo

    git clone https://github.com/eginnovations/helm-charts.git
    cd helm-charts

## Make your chart changes inside of egagent directory  

    helm lint eagent
    mkdir -p repos/new_charts
    helm package -u -d repos/new_charts egagent
    helm repo index repos/new_charts --url "https://eginnovations.github.io/helm-charts/repos/stable/" --merge index.yaml 

# Update original repo

    mv repos/new_charts/egagent-*.tgz repos/stable
    mv repos/new_charts/index.yaml index.yaml
    rm  -rf repos/new_charts

# Create commit on repo

    pushd .
    git add -A
    git commit -m "updated charts"
    git push
    popd
