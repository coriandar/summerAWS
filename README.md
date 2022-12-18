# SummerAWS Project Stuff

## TODO
https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/setting-up-node-on-ec2-instance.html
https://www.reddit.com/r/aws/comments/twdk16/writing_to_dynamodb_why_is_this_so_hard/ cc

## Domain Names
baneung.xyz

## CLI Configure
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

## EC2 Webhosting commands
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
