## STRAPI on AWS Fargate Spot
🚀 Project Overview

This project deploys a Strapi application on AWS using:

Amazon ECS

AWS Fargate Spot (cost-optimized)

Application Load Balancer (ALB)

Amazon ECR

Amazon RDS (PostgreSQL)

Default AWS VPC

Infrastructure managed with Terraform

## Architecture

User → ALB → ECS (Fargate Spot) → RDS
Docker image stored in → ECR
Infrastructure managed via → Terraform

## Services Used
| Service        | Purpose                 |
| -------------- | ----------------------- |
| ECS            | Container orchestration |
| Fargate Spot   | Cost-optimized compute  |
| ALB            | Public traffic routing  |
| ECR            | Docker image storage    |
| RDS (Postgres) | Database backend        |
| Default VPC    | Networking              |
| Terraform      | Infrastructure as Code  |


## GitHub Secrets Required

Add these in repository → Settings → Secrets:

AWS_ACCESS_KEY

AWS_SECRET_KEY

## Accessing Strapi

http://<alb_dns_name>/admin
