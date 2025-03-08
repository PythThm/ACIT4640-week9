# Instructions
#### Import Key pair
`ssh-keygen -t ed25519 -C "something" -f ~/.ssh/<key-name>`\
Run the import key script with the location of your key\
`./import_lab_key ~/.ssh/<key-name>.pub`\

#### Packer
Make sure you have a default vpc, and can access your account by either using environmental variables or set up aws credentials
Do the following command in the parent folder\
`packer init packer/`\
`packer build packer/`\
If encounter "Gathering Facts" error, in the provisioner block add `use_proxy=false`

#### Terraform
Go to the terraform directory
`terraform init`\
`terraform validate`\
`terraform plan`\
`terraform apply`
