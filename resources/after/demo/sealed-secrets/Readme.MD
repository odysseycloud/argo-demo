

kubeseal <mysecret.json >mysealedsecret.json 

kubeseal <resources/after/demo/sealed-secrets/aws.yaml >resources/after/demo/sealed-secrets/aws-dns-creds-kube-infra.enc.yaml --controller-namespace secrets --format yaml

if you want a cluster wide secret add flag 
--scope cluster-wide
while creating the secret

kubeseal <resources/after/demo/sealed-secrets/github.yaml >resources/after/demo/sealed-secrets/github-private-repo-token.enc.yaml --controller-namespace secrets --format yaml