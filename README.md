
# Action Repository

This repository is used to trigger GitHub actions (push, pull request, merge) and send webhook events to the webhook-repo.

## Table of Contents

- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/action-repo.git
   cd action-repo
   ```

2. **Create a new branch for your changes:**

   ```bash
   git checkout -b feature-branch
   ```

3. **Make your changes and commit them:**

   ```bash
   git add .
   git commit -m "Describe your changes"
   ```

4. **Push your changes to GitHub:**

   ```bash
   git push origin feature-branch
   ```

5. **Create a pull request** from your feature branch to the main branch.

## Usage

1. **Trigger Actions:**
   - Push: Make changes to the repository and push them to GitHub.
   - Pull Request: Create a pull request from one branch to another.
   - Merge: Merge a pull request.

2. **Webhooks:**
   - Ensure the webhook is configured to point to the webhook-repo endpoint (e.g., `http://your-public-server/webhook/receiver`).

## Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the License - see the [LICENSE](LICENSE) file for details.
