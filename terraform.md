## CLI Commands

    terraform plan         # dry run
    terraform apply
    terraform apply -input=false -auto-approve tfplan           # applying previously create plan
    
    terraform refresh      # sync state with remote resources
    terraform show
    terraform destroy
    
    terraform validate     # validate .tf file
    
    terraform taint        # mark resource for recreation
    terraform untaint
    
    terraform state push   # e.g. force push state to S3 bucket
    terraform state pull > terraform.tfstate  # create a local state copy
    
    terraform force-unlock <lock-id-guid>     # Clean up leftover locks from hard-cancelled run
