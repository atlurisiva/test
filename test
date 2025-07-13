graph TB
    subgraph "Management Account"
        MA[Management Account<br/>Hub]
        S3[(S3 Data Lake)]
        Lambda[Lambda Functions]
        CW[CloudWatch Dashboard]
    end
    
    subgraph "Account A"
        EC2A[EC2 Instances]
        CWA[CloudWatch Agent]
    end
    
    subgraph "Account B"
        EC2B[EC2 Instances]
        CWB[CloudWatch Agent]
    end
    
    subgraph "Account C"
        EC2C[EC2 Instances]
        CWC[CloudWatch Agent]
    end
    
    EC2A --> CWA
    EC2B --> CWB
    EC2C --> CWC
    
    CWA --> Lambda
    CWB --> Lambda
    CWC --> Lambda
    
    Lambda --> S3
    Lambda --> CW
