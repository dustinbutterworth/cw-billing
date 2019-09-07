# cw-billing

Create a cloudwatch alarm that uses an encrypted SNS topic to let me know when monthly spending
has reached a certain value (Default 10 USD).

**Required Parameters**
* SubscriptionEmail
* TopicName
* AlarmName
* MetricName
* Namespace
* Statistic
* Period
* EvaluationPeriods
* Threshold
* ComparisonOperator
* AliasName
* KmsMasterKeyId

# Using CloudFormation Launcher (CLI)

1.  Clone the repo
2.  Modify the parameters in cw-billing-params.json
3.  Set stack name and review/modify cw-billing-cfnl.yml
4.  Run CFNL script to create stack
    ./cfnl.sh -f cw-billing-cfnl.yml

**Advanced CFNL Usage**
*  Create Stack - ./cfnl.sh -f cw-billing-cfnl.yml
*  Update Stack - ./cfnl.sh -u -f cw-billing-cfnl.yml
*  Delete Stack - ./cfnl.sh -d -f cw-billing-cfnl.yml
*  Create with Debug - ./cfnl.sh -b -f cw-billing-cfnl.yml
*  Delete with Debug - ./cfnl.sh -d -b -f cw-billing-cfnl.yml

**Primary Contact** 
* Dustin Butterworth - dustinbutterworth@protonmail.com

**Credits**
* Levon Becker for providing the cloudformation launcher that I'm using - https://github.com/bonusbits/cfn_launcher

