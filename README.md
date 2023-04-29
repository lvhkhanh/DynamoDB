# DynamoDB
## Certificates
- [x] Amazon DynamoDB: Building NoSQL DatabaseDriven Applications https://www.coursera.org/account/accomplishments/certificate/TGUL6PC2D6GP [Coursera TGUL6PC2D6GP.pdf](https://github.com/lvhkhanh/DynamoDB/files/11358173/Coursera.TGUL6PC2D6GP.pdf)

## Courses
- [x] https://learning.edx.org/course/course-v1:AWS+OTP-AWS-D6+3T2021/
## Concepts
- Capacity unit
  - RCU
  - WCU
- CAP
  - Consistent (Strong read, low, more CPU)
  - Available (weak consistent, fast)
  - Partition (always)   
- Adaptive Capacity
  - Total share on all partitions 
- Security
 - HIPPA
 - PCI DSS
 - token
- TTL: 48hours to auto deletion
- Global table
- Stream
- Optimistic locking: read and write on the same version attribute, otherwise fail
- Secondry indexes
  - LSI: new table difference partition key, sort key depend on base table
  - GSI: same partition key, other sort key
- Single table: SQL multi tables -> NoSQL single
- DAX
## Steps
### Create table
- table-name
- primary key
  - partition-key
  - sort-key(optional)
### Put item
- table-name
- primary key
- attributes
### Query(fast)
- table-name
- primary-key
  - --key-condition-expression="PK = :v1 AND SK = :v2"
- --expression-attribute-values="{':v1':'value1', ':v2':'value2'}"
### Scan(low)
- table-name
- filter-expression
### UpdateItem
- --update-expression="SET a= '100'"
- --condition-expression='b > 10'
## Tools
- Console
- Cloud9
- Shell
- SDK
## Use cases
- key-value store: Which type of database should be used to store user session data with the highest scalability and effective way?
