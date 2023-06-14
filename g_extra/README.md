# Deploy your PySpark code on Amazon EMR Serverless using Terraform and GitHub Actions

Now that you have successfully completed all the training exercises, it's time to apply all everything we've learned in a project.

## Terraform
Have a look at the Terraform documentation on Amazon EMR [Here](https://docs.aws.amazon.com/emr/latest/EMR-Serverless-UserGuide/emr-serverless.html)

Go back to you repository `getting_started_pyspark` and create a new folder `terraform`, this is where we will store
all our terraform files (.tf).

You might need to set up your AWS credentials again:
```bash
aws configure
AWS Access Key ID [None]: $YOUR_ACCES_KEY_ID
AWS Secret Access Key [None]: $YOUR_SECRET_ACCES_KEY
Default region name [None]: eu-west-1
Default output format [None]: json
```

Go step by step and always `terraform plan` to have a look at what changes will be applied to your infrastructure!

## GitHub Actions
Once you have locally tested your terraform code, it's time to automate your deployment.

You will need a new `.github` folder in your repository with a `workflows` folder that will contain as many `yml` files as needed.

Use GitHub actions to automate your deployment everytime there's a new push to `master`.

## EXTRA
Use GitHub Actions to run your Python tests before applying your Terraform code.
