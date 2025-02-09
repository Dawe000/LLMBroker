# LLMBroker

## Overview
LLMBroker is a decentralized platform that enables users to run large language model (LLM) inferences on idle computing hardware. By leveraging a distributed network of compute providers, LLMBroker connects those who need LLM services with those who have spare processing power, creating an efficient, cost-effective, and scalable solution. To ensure fair compensation for compute providers, LLMBroker utilizes the Flare Time Series Oracle (FTSO) to obtain real-time FLR-to-USD price data, stabilizing input token prices within its smart contracts.

## How It Works
LLMBroker consists of three core components:

### 1. LLMBroker Server
The LLMBroker Server allows users to earn money by running LLM inferences on their computers when they are idle. It acts as a RESTful API endpoint that processes inference requests and verifies them against smart contracts to ensure security and compliance.

### 2. Inference Agreement Smart Contracts
Smart contracts serve as a decentralized marketplace for LLM tokens. Users can purchase tokens to access compute resources, and providers receive tokens in exchange for fulfilling inference requests. This ensures a transparent and trustless transaction system.

### 3. LLMBroker NPM Package
The LLMBroker NPM package simplifies interaction with the smart contract marketplace. It abstracts token purchasing, server discovery, and request handling into an easy-to-use JavaScript library. This package is also integrated into the server code for seamless operation.

## Key Features
Key Features

- **Decentralized Compute Sharing** – Utilize idle GPUs and CPUs for LLM inference tasks.
- **Smart Contract Marketplace** – Secure and transparent token-based payment system.
- **Real-Time Price Stabilization** – Leverages the Flare Time Series Oracle (FTSO) to stabilize token prices for server owners.
- **Simple API Integration** – Easily connect to LLMBroker services using the NPM package.
- **Earn Passive Income** – Run LLM inferences and get rewarded for unused compute power.
- **Scalable & Cost-Effective** – Pay only for the compute you use, with no centralized overhead.

## Getting Started
### Setting Up Your Compute Server
Follow these steps to configure your machine as an LLMBroker compute server:

1. **Clone the Endpoint Repository**  
   - Download the Endpoint directory and set up your preferred LLM. By default, DeepseekR1 is pre-configured.

2. **Install LLMBroker API Library**  
   - In your project, install the LLMBroker API library:
     ```sh
     npm install llmbrokerapilib
     ```

3. **Create a Thirdweb Client & Wallet**  
   - Set up a Thirdweb client and generate a new wallet. 

4. **Deploy Your Server Contract**  
   - Use the `CreateServer` and `SetupModel` functions from the LLMBroker API library to configure your server with pricing and endpoint details. An example implementation is available in the NPM package repository.

5. **Configure Environment Variables**  
   - Update the `.env` file in the Endpoint server directory with the following details:
     - **Wallet Private Key**
     - **Deployed Server Contract Address**
     - **Thirdweb Client Details**

6. **Start Earning**  
   - Once set up, your server is publicly listed, allowing users to request inferences. You can now start earning by providing compute power!

## Contributing
We welcome contributions! Please submit pull requests and open issues to help improve LLMBroker.

## License
This project is licensed under the MIT License.

## Contact
For more details, visit our [GitHub repository](https://github.com/your-repo).

