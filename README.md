###  Web server EC2 instance with nginx installed

NGINX EC2 instance accesible via:

http://web-lb-303821509.us-east-2.elb.amazonaws.com

### Prerequisites

Requires terraform version 1.9.5 or higher.

HashiCorp Terraform Installation Instructions: 

https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli

Requires AWS CLI, AWS Account Access, Environmental Variables configured for AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY and AWS_DEFAULT_REGION

https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

https://docs.aws.amazon.com/cli/v1/userguide/cli-configure-envvars.html

### Requirements

.gitignore file with:

```bash
# Local .terraform dir
.terraform/*

# terraform state files
*.tfstate
*.tfstate.*

# terraform variable files
*.tfvars
```

### Instructions

```bash
terraform plan 
terraform apply 
```

### Terrafrom Verbose
```
Apply complete! Resources: 15 added, 0 changed, 0 destroyed.

Outputs:

lb_dns_name = "web-lb-303821509.us-east-2.elb.amazonaws.com"
```

### Post Cleanup
```bash
terraform destroy 
```

### License

Copyright 2024 

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
