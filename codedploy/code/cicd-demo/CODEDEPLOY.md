
# Installing the CodeDeploy agent on EC2
```
sudo yum update -y
sudo yum install -y ruby wget
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
chmod +x ./install
sudo ./install auto
sudo service codedeploy-agent status
```
```

# deploy the files into S3
```
aws deploy push --application-name Codedeploy --s3-location s3://pranayec2codedeploy/codedeploy_zip/ --ignore-hidden-files --region ap-south-1 --profile aws-devops
```
