<p align="center">
  <h1 align="center">Iceberg data storage format</h1>
  <p align="center">
    <a href="README_ZH.md"><strong>简体中文</strong></a> | <strong>English</strong>
  </p>

## Table of Contents

- [Repository Introduction](#repository-introduction)  
- [Prerequisites](#prerequisites)  
- [Image Specifications](#image-specifications)
- [Getting Help](#getting-help)
- [How to Contribute](#how-to-contribute)

## Repository Introduction  
[Apache Iceberg](https://github.com/apache/iceberg) is a new open-source table format used for large-scale data analysis. It is designed to store large, slow-moving table data. It aims to improve the de facto standard table layout built into Hive, Trino (PrestoSQL), and Spark. Iceberg can mask differences in underlying data storage formats and provide a unified API for operations, allowing different engines to access through its provided API.

**Core Features:**
1. Schema evolution: Supports adding, dropping, updating, renaming, and reordering table format definitions.
2. Partition layout evolution: The layout of a table can be updated with changes in data volume or query patterns.
3. Hidden partitioning: The query no longer depends on the physical layout of the table. By separating physical and logical data, Iceberg tables can develop partitioning schemes as the amount of data changes and time passes. Tables with incorrect configurations can be fixed without the need for expensive migration.
4. Time travel: supports users to use identical snapshots for repeated queries, or allows users to easily check for changes.
5. Version rollback: allows users to quickly correct issues by resetting tables to a good state.

**Architecture Design:**

![](./images/img001.png)

This project offers pre-configured [**OpenMetadata metadata management platform**](https://marketplace.huaweicloud.com) images with OpenMetadata and its runtime environment pre-installed, along with deployment templates. Follow the guide to enjoy an "out-of-the-box" experience.

> **System Requirements:**
> - CPU: 2GHz or higher  
> - RAM: 4GB or more  
> - Disk: At least 40GB  

## Prerequisites  
[Register a Huawei account and activate Huawei Cloud](https://support.huaweicloud.com/usermanual-account/account_id_001.html)

## Image Specifications  

| Image Version                                                                                                      | Description                                              | Notes |  
|--------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------|-------|  
| [OpenMetadata2.1_HCE2.0](https://marketplace.huaweicloud.com) | Deployed on Kunpeng servers with Huawei Cloud EulerOS 2.0 64bit |  | 
| [OpenMetadata2.1_Ubuntu24.04](https://marketplace.huaweicloud.com) | Deployed on Kunpeng servers with Ubuntu24.04 64bit   |  |  

## Getting Help
- Submit an [issue](https://github.com/HuaweiCloudDeveloper/OpenMetadata-image/issues)
- Contact Huawei Cloud Marketplace product support

## How to Contribute
- Fork this repository and submit a merge request.
- Update README.md synchronously based on your open-source mirror information.
