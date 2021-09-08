

kubeseal <mysecret.json >mysealedsecret.json 

kubeseal <aws.yaml >aws-dns-creds-kube-infra.enc.yaml --controller-namespace kube-secrets --format yaml

if you want a cluster wide secret add flag 
--scope cluster-wide
while creating the secret

kubeseal <github.yaml >github-private-repo-token.enc.yaml --controller-namespace kube-secrets --format yaml