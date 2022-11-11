# Deploy a high-availability web app using CloudFormation
## Diagram

<div align="center">
    <img src="diagram/cloud-architecture.jpeg" />
</div>

## Prerequisites
AWS account with Iam role for webapp and a bucket already deployed having the webapp code. Don't forget to adapt the userData to match your webapp sources location

## How to Run
Run the following commands:

```
sh create.sh Dev0thNetwork network.yaml network-params.json
sh create.sh Dev0thServers servers.yaml servers-params.json
```

Last thing: Remember to delete your CloudFormation stack when you're done to avoid recurring charges!

```
sh delete.sh Dev0thServers
sh delete.sh Dev0thNetwork
```


