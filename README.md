# Autheriq CLI

A command-line interface tool that combines blockchain functionality with AI capabilities for enhanced authentication and interaction.

## Features

- 🔗 Ethereum blockchain integration via Ethers.js and Viem
- 🤖 AI-powered assistance through OpenAI integration
- 💻 Interactive CLI experience
- 🔐 Secure environment variable management

## Prerequisites

- Node.js 16+ 
- npm or yarn
- An OpenAI API key
- Ethereum RPC endpoint (if using blockchain features)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd autheriq-cli
```
2. Install dependencies:
```bash
npm install
```
3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your configuration
```

## Environment Setup
Create a .env file in the root directory with the following variables:
```env
OPENAI_API_KEY=your_openai_api_key_here
ETHEREUM_RPC_URL=your_ethereum_rpc_url_here
PRIVATE_KEY=your_private_key_here (optional)
```

### Usage
## Development Mode
```bash
npm run start
```
## Build and run
```bash
npm run build
node dist/index.js
```

## Available Scripts

| Script | Description |
|--------|-------------|
| `npm run build` | Compile TypeScript to JavaScript |
| `npm run start` | Build and run the application |
| `npm test` | Run tests (not yet implemented) |

## Dependencies

### Core Dependencies
- **ethers** - Ethereum blockchain interaction library
- **viem** - TypeScript interface for Ethereum
- **openai** - OpenAI API client for AI functionality
- **node-fetch** - HTTP request library
- **readline** - Interactive CLI input handling

### Development Dependencies
- **typescript** - TypeScript compiler
- **ts-node** - TypeScript execution environment
- **@types/node** - Node.js type definitions
- **dotenv** - Environment variable management

## Project Structure
```text
autheriq-cli/
├── src/           # Source TypeScript files
├── dist/          # Compiled JavaScript files
├── .env           # Environment variables (create from .env.example)
├── package.json   # Project configuration
└── tsconfig.json  # TypeScript configuration
```

## Development

1. Make sure you have all prerequisites installed
2. Set up your environment variables
3. Run `npm run start` to build and execute
4. The CLI will start and guide you through available options

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the ISC License.

## Support

For questions or issues, please open an issue on the repository or contact the maintainers.

---

**Note:** This tool handles sensitive information like private keys and API keys. Always keep your `.env` file secure and never commit it to version control.