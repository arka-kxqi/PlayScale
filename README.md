# PlayScale

PlayScale is a sample multiplayer game project leveraging **Amazon GameLift** and AWS managed services to build, scale, and deploy session-based online games. The project uses **Gomoku**, a classic board game, to demonstrate how to create a scalable multiplayer game with seamless matchmaking, game session management, and serverless infrastructure using AWS technologies.

## Overview

PlayScale provides a full-stack solution for game developers and system engineers to understand how to build a multiplayer game using **Amazon GameLift** and other AWS services. This project integrates AWS serverless components such as **Lambda**, **SQS**, **DynamoDB**, **S3**, **EC2**, and **ElastiCache** for creating an easily scalable, real-time multiplayer experience.

### Features
- **Serverless architecture** using AWS managed services.
- Integration with **Amazon GameLift** for matchmaking and game session hosting.
- **FleetIQ** to optimize fleet management and load balancing (currently in preview).
- Sample Python-based TCP game server for matchmaking and session handling.
- Real-time, multiplayer gameplay with auto-scaling capabilities.

## Architecture

The architecture of PlayScale includes several AWS services that work together to support a scalable multiplayer experience:
- **Amazon GameLift**: Manages game session hosting and multiplayer matchmaking.
- **FleetIQ**: A preview feature that helps with fleet management and efficient game instance balancing.
- **AWS Lambda**: Used for event-driven serverless processing.
- **DynamoDB**: Stores player and game session data.
- **SQS**: Handles communication between various AWS services.
- **S3**: Hosts game assets like images or other static content.
- **ElastiCache**: Caches frequently accessed data for performance optimization.

### CloudFormation Deployment
To make it easy to deploy, the infrastructure is defined using **CloudFormation**. You can set up the game infrastructure automatically by following the provided deployment guide.

## Getting Started

### Prerequisites:
1. **AWS Account**: Ensure you have an active AWS account.
2. **MS C++ Redistributable**: Make sure to include these packages for the Game Client & Game Server:
   - [Download MS C++ Redistributable](https://www.microsoft.com/en-us/download/details.aspx?id=48145)
3. **Game Client & Server Binaries**: Download the necessary binaries for game execution.

### Deployment Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/aws-samples/aws-gamelift-sample.git
   cd aws-gamelift-sample
   ```
2. Follow the detailed deployment guide found in the docs folder.

3. Deploy using CloudFormation to set up the game infrastructure automatically.

4. Run the Game Server and Client using the provided sample code.

### Future Work

1. Enhance and update FleetIQ demo to improve game instance management.
2. Develop multi-region game support for global scalability.
3. Continuous updates to adapt to new Amazon GameLift features.