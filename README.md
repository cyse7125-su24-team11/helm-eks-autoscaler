# helm-eks-autoscaler



helm repo add autoscaler 'https://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@raw.githubusercontent.com/cyse7125-su24-team11/helm-eks-autoscaler/main/'


helm repo add autoscaler 'https://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@www.github.com/cyse7125-su24-team11/ca-helm-registry/main/'  --debug

helm repo add autoscaler 'https://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@www.github.com/anibahs/ca-helm-registry/main/'  --debug

helm repo add autoscaler --username anibahs --password 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 'https://www.github.com/cyse7125-su24-team11/ca-helm-registry/main/' --debug

helm repo add autoscaler --username anibahs --password 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 'https://www.github.com/anibahs/ca-helm-registry/main/' --debug

curl --fail-with-body --request POST \
     --form 'chart=@autoscaler-0.1.0.tgz' \
     --user anibahs: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 \
    'https://www.github.com/cyse7125-su24-team11/ca-helm-registry/main/'




helm install autoscaler autoscaler --set caRoleArn=<caRoleArn> --set-file dockerconfigjson=/Users/shabinasingh/.docker/config.json


helm uninstall autoscaler