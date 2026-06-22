# AWS IoT Vehicle Telemetry Pipeline

## Overview

This project demonstrates the implementation of an end-to-end IoT telemetry data pipeline using AWS cloud services. The objective was to simulate a vehicle or IoT device that continuously generates telemetry data and securely transmits it to AWS IoT Core using the MQTT protocol.

A Python-based device simulator was developed to publish dynamic telemetry data at regular intervals, mimicking real-world device behavior. AWS IoT Core was configured to authenticate the device using certificates and manage secure communication through MQTT topics and IoT policies.

Incoming telemetry messages were processed using AWS IoT Rules and routed to Amazon S3 for persistent storage. The stored data can be utilized for future analytics, monitoring, reporting, and machine learning applications.

This project was developed as a Proof of Concept (PoC) during my internship to gain hands-on experience with real-world IoT-to-Cloud communication workflows.

## Architecture

Device Simulator (Python)
        ↓
AWS IoT Core
        ↓
AWS IoT Rule
        ↓
Amazon S3

## Technologies Used

- Python
- AWS IoT Core
- MQTT
- Amazon S3
- IAM
- Device Certificates
- IoT Policies

## Implementation Steps

### Step 1: AWS IoT Core Setup

- Created an IoT Thing
- Generated device certificates
- Attached IoT policies
- Configured MQTT topics

### Step 2: Device Simulator

- Developed a Python-based simulator
- Established secure MQTT connection
- Published telemetry data periodically
- Simulated dynamic sensor values

### Step 3: IoT Rule Configuration

- Created AWS IoT Rules
- Routed incoming telemetry messages
- Configured S3 integration

### Step 4: Data Persistence

- Stored telemetry records in Amazon S3
- Verified successful message delivery

### Step 5: Monitoring and Validation

- Validated device connectivity
- Monitored message publishing
- Confirmed successful data persistence

## Key Learnings

- AWS IoT Core architecture
- MQTT communication
- Secure device authentication
- Cloud data ingestion pipelines
- AWS service integration

## Future Enhancements

- AWS Lambda integration
- DynamoDB storage
- CloudWatch monitoring
- Real-time dashboard
