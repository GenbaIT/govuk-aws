## Project: app-gatling

Gatling node


## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| asg_desired_capacity | The autoscaling groups desired capacity | string | `0` | no |
| asg_max_size | The autoscaling groups max_size | string | `0` | no |
| asg_min_size | The autoscaling groups max_size | string | `0` | no |
| aws_environment | AWS Environment | string | - | yes |
| aws_region | AWS region | string | `eu-west-1` | no |
| ebs_encrypted | Whether or not the EBS volume is encrypted | string | - | yes |
| elb_external_certname | The ACM cert domain name to find the ARN of | string | - | yes |
| external_domain_name | The domain name of the external DNS records, it could be different from the zone name | string | - | yes |
| external_zone_name | The name of the Route53 zone that contains external records | string | - | yes |
| instance_ami_filter_name | Name to use to find AMI images | string | `` | no |
| instance_type | Instance type used for EC2 resources | string | `m5.2xlarge` | no |
| office_ips | An array of CIDR blocks that will be allowed offsite access. | list | - | yes |
| remote_state_bucket | S3 bucket we store our terraform state in | string | - | yes |
| remote_state_infra_monitoring_key_stack | Override stackname path to infra_monitoring remote state | string | `` | no |
| remote_state_infra_networking_key_stack | Override infra_networking remote state path | string | `` | no |
| remote_state_infra_root_dns_zones_key_stack | Override stackname path to infra_root_dns_zones remote state | string | `` | no |
| remote_state_infra_security_groups_key_stack | Override infra_security_groups stackname path to infra_vpc remote state | string | `` | no |
| remote_state_infra_stack_dns_zones_key_stack | Override stackname path to infra_stack_dns_zones remote state | string | `` | no |
| remote_state_infra_vpc_key_stack | Override infra_vpc remote state path | string | `` | no |
| stackname | Stackname | string | - | yes |
| user_data_snippets | List of user-data snippets | list | - | yes |

## Outputs

| Name | Description |
|------|-------------|
| instance_iam_role_name | name of the instance iam role |

