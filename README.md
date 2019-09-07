# encrypted-s3-sns-sqs

Create an s3 bucket sending notifications to SQS through SNS. This template also has the following features:
1. KMS Key Creation 
2. Logging enabled for s3 bucket
3. Encrypted s3 bucket
4. Encrypted SNS Topic
5. Encrypted SQS Queue

**Required Parameters**
* BucketName
* DestinationBucketName
* LogFilePrefix
* VersioningConfiguration
* AccessControl
* InstallerTag
* MaximumMessageSize
* MessageRetentionPeriod
* ReceiveMessageWaitTimeSeconds
* UsedeadletterQueue
* VisibilityTimeout
* ContentBasedDeduplication
* QueueName
* TopicName
* FifoQueue
* QueuePolicySid
* KmsMasterKeyId
* QueuePolicyId
* AliasName

# Using CloudFormation Launcher (CLI)

1.  Clone the repo
2.  Modify the parameters in encrypted-s3-sns-sqs-params.json
3.  Set stack name and review/modify encrypted-s3-sns-sqs-cfnl.yml
4.  Run CFNL script to create stack
    ./cfnl.sh -f encrypted-s3-sns-sqs-cfnl.yml

**Advanced CFNL Usage**
*  Create Stack - ./cfnl.sh -f encrypted-s3-sns-sqs-cfnl.yml
*  Update Stack - ./cfnl.sh -u -f encrypted-s3-sns-sqs-cfnl.yml
*  Delete Stack - ./cfnl.sh -d -f encrypted-s3-sns-sqs-cfnl.yml
*  Create with Debug - ./cfnl.sh -b -f encrypted-s3-sns-sqs-cfnl.yml
*  Delete with Debug - ./cfnl.sh -d -b -f encrypted-s3-sns-sqs-cfnl.yml

**Primary Contact** 
* Dustin Butterworth - dustinbutterworth@protonmail.com

**Credits**
* Chris Goodson for teaching me important Cloudformation bits - https://www.linkedin.com/in/chris-goodson-93917553/
* David Drake for continuing to work with me on making this even more secure - https://www.linkedin.com/in/ddrake11
* Levon Becker for providing the cloudformation launcher that I'm using - https://github.com/bonusbits/cfn_launcher

