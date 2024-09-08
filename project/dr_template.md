# Infrastructure

## AWS Zones
Zone 1

## Servers and Clusters

### Table 1.1 Summary
| Asset             | Purpose                        | Size                | Qty | DR                                                                  |
|-------------------|--------------------------------|---------------------|-----|---------------------------------------------------------------------|
| EC2 instance      | Hosts python web backend       | 1 t3.micro instance | 1   | Yes, another EC2 instance hosting the same web app can be deployed. |
| RDS mysql cluster | Databse for the python backend | 1 mysql writer      | 1   | Yeah, we can deploy another cluster in a different region f         |
| EKS cluster       | hosts the monitoring stack     | single node cluster | 1   | we can have multiple nodes, k8s control planes..                    |

### Descriptions


## DR Plan
### Pre-Steps:

## Steps:
