# EC2

Elastic Compute Cloud (EC2) is AWS service for renting compute.

## Key Concepts

1. **EC2 Instance**
- a rentable virtual server.

2. **Amazon Machine Images**
- The operating system(s) that ec2 instances can run.

3. **User Data**
- Scripts that you can run on the first launch of your ec2 instance.
    - aka bootstrapping
    - runs with root user

4. ** Security Groups**
- A "firewall" around your ec2 instance that defines inbound/outbound access.
    - Only ALLOW rules, all inbound traffic is denied and all outbound traffic is allowed.
    - Reference by ip and other security groups.
    - Locked down to region + vpc
    - A security group can be attached to multiple instance, and an instance can have multiple security groups attached.
    - Controls access to ports:
        - 22 (SSH/SFTP)
        - 21 (FTP)
        - 80 (HTTP)
        - 443 (HTTPS)
        - 3389 (RDP)

## EC2 Instance Types

1. **General Purpose** - A balance between compute, memory and storage

2. **Compute Optimized** - High performance processors.

3. **Memory Optimized** - Good for large data sets in memory.

4. **Storage Optimized** - Good for high read and write to local storage.


