# terraform-aws-organization


This Terraform module creates a simple AWS Organization.

Deploy this module to your _master_ account.

This module verifies if the AWS organization exists, if not, It creates.

The following resources will be created:
- Identity and Access Management(IAM) policies for the organization

<!--- BEGIN_TF_DOCS --->

## Requirements

| Name | Version |
|------|---------|
| terraform | >= 0.12.0 |

## Providers

| Name | Version |
|------|---------|
| aws | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| already\_exists | Whether the organization already exists or needs to be created | `bool` | `false` | no |
| enable\_aws\_sso | Whether the AWS SSO needs to be enabled when creating a new organisation | `bool` | `false` | no |
| name | Name for this organization (not actually used in API call) | `any` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| id | ID of organization created |
| name | n/a |
| roots\_id | Roots of organization created |

<!--- END_TF_DOCS --->

## Authors

## License
