### **AWS CLI**  
- ` aws configure `
```
    output:
    PS C:\Users\1511 MXTI> aws configure
    AWS Access Key ID [None]: YOU_ACCESS_KEY
    AWS Secret Access Key [None]: YOUR_SECRET_KEY
    Default region name [None]: eu-central-1
    Default output format [None]:
```  
- `aws ec2 create-key-pair --key-name DevopsBook --query'KeyMaterial' --output text YOUR_PRIVATE_KEY`  
- `aws ec2 create-vpc --cidr-block
"192.168.0.0/24"`
- `aws ec2 create-subnet --cidr-block
"192.168.0.0/24" --vpc-id vpc-0825b5c6f6a2a2429`
- `aws ec2 create-security-group --group-name
devops-book --description "Example used in the book" --vpc-id vpc-
0825b5c6f6a2a2429`  
- `aws ec2 authorize-security-group-ingress --
group-id sg-0da7b308d99365dc3 --protocol tcp --port 22 --cidr
0.0.0.0/0`  
- `aws ec2 run-instances --count 1 --instancetype
t3.micro --key-name DevopsBook --security-group-ids sg-
0da7b308d99365dc3 --subnet-id subnet-0c7889e706674e64f --image-id
ami-0b418580298265d5c`  
- `aws ec2 describe-instances --query`  
- ``
