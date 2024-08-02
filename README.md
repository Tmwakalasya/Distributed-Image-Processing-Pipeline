# Distributed Image Processing Pipeline

## Overview

This project implements a scalable, distributed system for processing large volumes of images. It leverages distributed computing to efficiently handle tasks such as image resizing, filtering, and feature extraction across a cluster of machines.

## Features

- Distributed file system for efficient storage and retrieval of raw and processed images
- Task queue system for managing and distributing processing jobs
- Worker nodes that perform various image processing tasks
- Results aggregation system for collecting and organizing processed data
- Dynamic load balancing to ensure even distribution of work across nodes
- Fault tolerance mechanisms to handle node failures gracefully
- Support for multiple image processing algorithms including resizing, filtering, and feature extraction
- RESTful API for job submission and result retrieval

## Architecture

The system consists of the following components:

1. **Distributed File System**: Stores raw and processed images (using HDFS)
2. **Task Queue**: Manages processing jobs (using Apache Kafka)
3. **Worker Nodes**: Perform image processing tasks
4. **Master Node**: Coordinates job distribution and monitors system health
5. **Results Aggregator**: Collects and organizes processed data
6. **API Server**: Provides RESTful interface for job submission and result retrieval

## Technologies Used

- Python 3.8+
- Apache Hadoop (HDFS)
- Apache Kafka
- Docker & Kubernetes
- OpenCV for image processing
- Flask for API server

## Setup and Installation

1. Clone the repository:
