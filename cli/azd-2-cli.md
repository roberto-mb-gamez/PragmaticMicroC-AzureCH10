# Get the TenantID
> az account show --query tenantId -o tsv

# Get the SubscriptionID
> az account show --query id -o tsv

8236d71b-1da4-4562-9ccb-b6fbdbbdac67

# Create environment
> azd env new codebreaker-08-prod

# List all environments
> azd env list

# Select environment
> azd env select codebreaker-08-dev

# Show configuration for an environment
> azd env get-values

# Update env configuration
> azd env set AZURE_LOCATION eastus2

# Create federated account for environment
> azd pipeline config --auth-type federated --principal-name github-codebreaker-prod