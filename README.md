# Getting Started with IaC on AWS using Terraform and GitHub Actions

📚 A course brought to you by the [Data Minded Academy].

## Context

These are the exercises used in the course *Data Pipeline Part 2 at DSTI*.  
The course has been developed by instructors at Data Minded. The
exercises are meant to be completed in the lexicographical order determined by
name of their parent folders. That is, exercises inside the folder `b_foo`
should be completed before those in `c_bar`, but both should come after those
of `a_foo_bar`.

## Course objectives

- Introduce good data engineering practices.
- Illustrate better infrastructure management with Terraform and GitHub Actions.
- Illustrate Terraform concepts, like modules, tfstate & providers.
  Not limited to these three though.
- Use GitHub Actions to automate your deployments.

## Intended audience

- People interesteed on DevOps practices applied to Data Engineering or soon to be working with Terraform/GitHub Actions.
- Familiar with AWS and IaC

## Approach

Lecturer first sets the foundations right for Infrastructure as Code and
gradually builds up to Terraform and GitHub Actions.

There is a high degree of participation expected from the students: they
will need to write code themselves and reason on topics, so that they can
better retain the knowledge.

Note: this course is not about writing the best code possible. There are
many ways to skin a cat, in this course we show one (or sometimes a few), which
should be suitable for the level of the participants.

## Getting started

## Install Terraform

To install Terraform, we recommend using a version manager such as tfswitch or tfenv.

Specifically for Windows, follow this step by step tutorial we've prepared: [Click Here](https://app.tango.us/app/workflow/Downloading-Terraform-on-Windows--A-Quick-Tutorial-63634416f09348c4857f64e3804235a2)

For the exercises, we'll be using Terraform versions `>=1.0.0`

## Prerequisites
### Have an AWS account - use the free trial

In order for Terraform to deploy infrastructure on AWS, Terraform needs to make authenticated API requests on your behalf.
You will need the `AWS_ACCES_KEY_ID` and `AWS_SECRET_ACCESS_KEY` from your account.

First make sure that you have the [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)
installed. Then run `aws configure` and fill in the access keys and configure the region and output format as follows:

```bash
aws configure
AWS Access Key ID [None]: $YOUR_ACCES_KEY_ID
AWS Secret Access Key [None]: $YOUR_SECRET_ACCES_KEY
Default region name [None]: eu-west-1
Default output format [None]: json
```

## Ready... Set... Go

You should now be able to start with the exercises. `cd` your way into the first exercise folder (`a_provider_config`),
read the instructions in each [README.md](a_provider_config/README.md) and try to write some Terraform code to solve the problem. Don't worry, 
the majority of the code you can find in or adapt from the [Terraform provider documentation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)! 
Good luck, and remember: `terrafrom init`, `terraform plan`, and `terrafrom apply` all the things!

P.S.: Exercise `h_extra` will be very useful in your project since you'll have to deploy it in EMR in AWS and automate
the deployment.

Have a look at the Terraform documentation on Amazon EMR [Here](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/emr_cluster)

[Data Minded Academy]: https://www.dataminded.academy/
