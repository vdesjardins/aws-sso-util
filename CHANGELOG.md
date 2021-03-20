# Changelog

* [`aws-sso-util`](#aws-sso-util)
* [`aws-sso-lib`](#aws-sso-lib)

## `aws-sso-util`

### v4.23

* Added [`aws-sso-util check`](docs/check.md) for diagnosing issues.
* Added additional aliases for AWS SSO instance configuration environment variables for `aws-sso-util configure`:
  * `AWS_SSO_CONFIGURE_DEFAULT_SSO_START_URL`
  * `AWS_SSO_CONFIGURE_DEFAULT_SSO_REGION`
* Changed verbose logging:
  * `-v` sets DEBUG for the command, INFO for `aws-sso-util` and `aws-sso-lib`
  * `-vv` sets DEBUG for the command and `aws-sso-util`, INFO for `aws-sso-lib`
  * `-vvv` sets DEBUG for the command, `aws-sso-util`, and `aws-sso-lib`
  * `-vvvv` sets DEBUG for the root logger (i.e., also boto3/botocore)
* Fixed bug with errors on finding AWS SSO instances

## `aws-sso-lib`

### v1.7

* Added more logging to `aws_sso_lib.config.find_instances()`
