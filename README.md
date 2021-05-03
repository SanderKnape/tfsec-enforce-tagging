# Shift left AWS tag enforcement with Terraform and tfsec

This is a sample repository that showcases how to combine [Terraform](https://www.terraform.io/) with [tfsec](https://github.com/tfsec/tfsec) to enforce tagging on all AWS resources that support it.

It makes use of the [default_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs#default_tags) property that can be set on the AWS provider configuration. A [custom tfsec check](https://tfsec.dev/docs/custom_checks/) enforces that this property is set.

Check out the [pull request](https://github.com/SanderKnape/tfsec/pull/1) that shows the feedback that is given in a comment when a non-compliant change is introduced.

For more information on this setup, check out my blog post: [Shift left AWS tag enforcement with Terraform and tfsec](https://sanderknape.com/2021/05/shift-left-aws-tag-enforcement-terraform-tfsec/)
