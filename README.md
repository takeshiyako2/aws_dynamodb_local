# aws_dynamodb_local

AWS DynamoDB Local Installer

```
git clone https://github.com/takeshiyako2/aws_dynamodb_local.git
cd aws_dynamodb_local/installer
/bin/bash ./install.sh

mkdir /root/.aws
cat << EOT > /root/.aws/config
[default]
aws_access_key_id =
aws_secret_access_key =
region=ap-northeast-1
EOT

/etc/init.d/aws_dynamodb_local start

aws dynamodb list-tables --endpoint-url http://localhost:8000
{
    "TableNames": []
}
```
