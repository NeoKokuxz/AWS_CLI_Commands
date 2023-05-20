# AWS_CLI_Commands

## Switch Profile

1. Check Profile list
```
aws configure list-profiles
```
2. Make new profile 
```
$ code ~/.aws/config (Using VSCode)

[default]
region=us-east-1
output=json

[profile user1] // Include the prefix "profile" only when 
configuring a named profile in the config file
region=us-east-1
output=json


$ code ~/.aws/credentials

[default]
aws_access_key_id=xxxxx
aws_secret_access_key=xxxxxxx

[user1] // Do not use the prefix "profile" 
aws_access_key_id=YOUR_ACCESS_KEY
aws_secret_access_key=YOUR_SECRET_ACCESS_KEY
``` 
3. Export profile inside terminal
```
export AWS_PROFILE=profile_name (change name accordingly)
```
4. check activate profile
```
aws configure list
```
