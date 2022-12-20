# SummerAWS Project Stuff

## TODO
https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/setting-up-node-on-ec2-instance.html
https://www.reddit.com/r/aws/comments/twdk16/writing_to_dynamodb_why_is_this_so_hard/
https://www.youtube.com/watch?v=O7cF8-bz2jE&list=PL55RiY5tL51rudermnWTq1LlGC1BL1g3l&index=4
https://docs.amazonaws.cn/en_us/sdk-for-javascript/v3/developer-guide/cross-service-example-submitting-data.html
https://docs.aws.amazon.com/sdk-for-javascript/v3/developer-guide/cross-service-example-submitting-data.html
https://medium.com/@kjthorpe18/how-to-build-a-serverless-web-app-with-react-api-gateway-lambda-dynamodb-f53c5dc1a53e

## Domain Names
baneung.xyz

## CLI Configure
```
aws configure
AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
Default region name [None]: us-west-2
Default output format [None]: json

aws sts get-caller-identity
OUTPUT: 
//change up values
{
    "UserId": "AIDATF7JJIROG64BLSD2E",
    "Account": "218995704924",
    "Arn": "arn:aws:iam::218995704924:user/hfdev"
}
```

## EC2 Webhosting commands
```
sudo su -
yum update -y
// Apache HTTP Server & git
yum install -y git httpd

git clone https://github.com/coriandar/honestFeedbackApp.git
cd honestFeedbackApp/
mv * /var/www/html


systemctl status httpd
systemctl enable httpd
systemctl start httpd

did not use EBS snapshot as it requires same region and not efficient
```
