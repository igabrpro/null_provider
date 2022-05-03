# **Terraform null_provider**

#### This repo is a guideline on HOW to use null provider in terraform using Ubuntu.

# **Repo content**
#### ```main.tf``` - Terraform configuration file

# **PreRequsits**
#### You need to have terraform cli instaled 
#### [download link](https://www.terraform.io/downloads)

# ***How to use***
#### 
    Download the repo bigabrpro/null_provider git clone https://github.com/igabrpro/null_provider.git
    Change to terraform_null_provider: cd terraform_null_provider
    Type in your terminal terraform init in order to be downloaded required providers
    Type in your terminal terraform plan in order to see the changes which terraform is going to be made
    Type in your terminal terraform apply execute changes bases on our code(main.tf)


# ***Expected results***
 
  ```
  After terrform apply you shuld get
   ==============================================================================
   null_resource.igabr: Creating...
   null_resource.igabr: Provisioning with 'local-exec'...
   null_resource.igabr (local-exec): Executing: ["/bin/sh" "-c" "uname -a"]
   null_resource.igabr (local-exec): Darwin ivangabrovski-C02Z82YYLVDQ 20.6.0 Darwin Kernel Version 20.6.0: Wed Nov 10 22:23:07 PST 2021; root:xnu-   7195.141.14~1/RELEASE_X86_64 x86_64
   null_resource.igabr: Creation complete after 0s [id=438409045189596853]
   ==============================================================================
 ```
 #### example
 ```
  vangabrovski@ivangabrovski-C02Z82YYLVDQ null_provider % terraform show
 null_resource.igabr:
 resource "null_resource" "igabr" {
    id       = "4316501647646768040"
    triggers = {
        "build_number" = "2022-05-03T12:47:17Z"
```

