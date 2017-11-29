# Creating k8s Cluster in AWS with `kops`
https://kubernetes.io/docs/getting-started-guides/kops/

## Setup

1. To install `kops` on a Mac, just

        brew install kops

2. Set up the Route 53 hosted zone for the topmost domain you want the cluster
   to serve content on.

3. The name of the cluster doesn't need to match the top-level domain from the
   Route 53 hosted zone. I like to name it something like `cluster.example.com`.

4. The S3 bucket for `kops` remote state could contain state for more than one
   cluster - best practice is to name it something like `clusters.example.com`.

