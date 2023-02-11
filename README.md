# DynamoDB

## Courses
- [ ] https://learning.edx.org/course/course-v1:AWS+OTP-AWS-D6+3T2021/
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
### Scan(low)
- table-name
- filter-expression

## Tools
- Console
- Cloud9
- Shell
- SDK
## Use cases
- key-value store: Which type of database should be used to store user session data with the highest scalability and effective way?
