mackerel-plugin-aws-kinesis-firehose
=======================

AWS Kinesis Firehose metrics plugin for mackerel.io agent.

## Synopsis

```shell
mackerel-plugin-aws-kinesis-firehose -identifier=<delivery-stream-name> -region=<aws-region> [-access-key-id=<id>] [-secret-access-key=<key>] [-tempfile=<tempfile>]
```

## AWS IAM Policy
the credential provided manually or fetched automatically by IAM Role should have the policy that includes an action, 'cloudwatch:GetMetricStatistics'

## Installation
- `mkr plugin install mackerelio/mackerel-plugin-aws-kinesis-firehose`
- Or download binary in Github Releases

## Example of mackerel-agent.conf

```
[plugin.metrics.aws-kinesis-firehose]
command = "/path/to/mackerel-plugin-aws-kinesis-firehose -identifier=your-delivery-stream-name"
```
