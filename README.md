### README.md for `action-repo`

# GitHub Action Trigger

This repository serves as a demonstration for triggering GitHub webhook events. By performing actions like pushing commits, creating pull requests, and merging branches, you can observe how GitHub events are captured and processed by your webhook receiver (`webhook-repo`).

---

## Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/action-repo.git
   cd action-repo
   ```

2. **Configure Webhook**
   - Go to `Settings` > `Webhooks` > `Add webhook` in your GitHub repository (`action-repo`).
   - Set the **Payload URL** to the endpoint provided by your Flask application (`webhook-repo`).
   - Select content type as `application/json`.
   - Choose to send events for "Push", "Pull Request", and "Merge".

---

## Usage

- Perform actions (push commits, create pull requests, merge branches) in this repository to trigger GitHub webhook events.
- Monitor the captured events in real-time using your `webhook-repo` frontend interface.

---

## Example Workflow

- **Push Event:**
  - Make changes to a file (`git add .`, `git commit -m "Update file"`, `git push origin main`).

- **Pull Request Event:**
  - Create a new branch (`git checkout -b feature-branch`), make changes, and push the branch (`git push origin feature-branch`).
  - Create a pull request from `feature-branch` to `main` in GitHub.

- **Merge Event:**
  - After the pull request is approved, merge it into the `main` branch on GitHub.

---

## Contributing

- Fork the repository, make your changes, and submit a pull request.
- Report issues or suggest improvements by opening an issue.

---

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

