# helm-eks-autoscaler



helm package autoscaler
helm repo index . 

cp autoscaler-0.1.0.tgz ../../Submissions/helm/ca-helm-registry 
cp index.yaml ../../Submissions/helm/ca-helm-registry 


git add .
git commit -m 'feat: New chart version'
git push


helm repo add autoscaler-repo-main 'https://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@raw.githubusercontent.com/cyse7125-su24-team11/ca-helm-registry/main/'

helm repo update





helm install autoscaler autoscaler --set caRoleArn=arn:aws:iam::533267343403:role/eks-ca --set-file dockerconfigjson=/Users/shabinasingh/.docker/config.json


helm uninstall autoscaler