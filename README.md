# azureArc

https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-arc/

# 1. Download AzureCLI at Master in Kubernetes Cluster
```
$ curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

# 2. Login Azure Portal thru azCLI
```
$ az login
```

# 3. Download azCLI's extension for onboarding my Onprem Kubernetes Cluster to azureArc
```
$ az extension add --name connectedk8s
$ az account set --subscription XXXXXXXX-XXXXX-XXXX-XXXX-XXXXXXXXXXXX
$ az connectedk8s connect --name myfirstazurearc --resource-group XXXXX-XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX --location japaneast --tags Datacenter=onprem City=tokyo
```
