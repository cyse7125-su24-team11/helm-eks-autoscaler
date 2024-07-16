# helm-eks-autoscaler


helm repo add helm-registry 'https://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@raw.githubusercontent.com/cyse7125-su24-team11/helm-eks-autoscaler/main/charts'



helm install autoscaler autoscaler --set caRoleArn=<caRoleArn> --set-file dockerconfigjson=/Users/shabinasingh/.docker/config.json
