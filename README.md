# Open Source Computer Use by E2B

A secure cloud Linux computer powered by [E2B Desktop Sandbox](https://github.com/e2b-dev/desktop/) and controlled by open-source LLMs.

https://github.com/user-attachments/assets/3837c4f6-45cb-43f2-9d51-a45f742424d4

## Get Started

### Prerequisites

- Python 3.10 or later
- [git](https://git-scm.com/)
- [E2B API key](https://e2b.dev/dashboard?tab=keys)
- [OpenRouter API key](https://openrouter.ai/settings/keys)
- [Fireworks API key](https://fireworks.ai/account/api-keys)

### 1. Install the Prerequisites

#### macOS

In your terminal:

```sh
brew install poetry ffmpeg
```

#### Windows

1. Install [Chocolatey](https://chocolatey.org/install).
2. Run the following command in PowerShell:

```sh
choco install poetry ffmpeg
```

Alternatively, use [Scoop](https://scoop.sh/):

1. Install Scoop by following the instructions [here](https://scoop.sh/).
2. Run the following command in PowerShell:

```sh
scoop install poetry ffmpeg
```

#### Linux

Use your package manager to install the prerequisites. For example, on Ubuntu/Debian:

```sh
sudo apt update && sudo apt install poetry ffmpeg
```

### 2. Clone the Repository

In your terminal:

```sh
git clone https://github.com/e2b-dev/secure-computer-use/
```

### 3. Set the Environment Variables

Enter the project directory:

```sh
cd secure-computer-use
```

Create a `.env` file in `secure-computer-use` and set the following:

```sh
# Get your API key here - https://e2b.dev/
E2B_API_KEY="your-e2b-api-key"
OPENROUTER_API_KEY="your-openrouter-api-key"
FIREWORKS_API_KEY="your-fireworks-api-key"
```

### 4. Start the Web Interface

Run the following commands to start the agent:

```sh
poetry install
poetry run start
```

The agent will start and prompt you for its first instruction.
