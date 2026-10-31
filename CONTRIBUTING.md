# Contribution guidelines

**Scope:** Public and private repositories owned by [matgir99](https://github.com/matgir99). These guidelines do not govern organization-owned repositories. Repository-specific instructions may supplement or replace the default rules with the owner's authorization.

## Branches and pull requests

1. **Never push directly to \`main\` or \`master\`.** Changes must enter through a pull request (PR), including changes made by the owner.
2. Ordinarily, work in a short-lived \`feature/*\`, \`fix/*\`, \`experiment/*\`, or similar task-specific branch and open a PR into \`develop\`.
3. Only the owner or explicitly authorized maintainers may push directly to \`develop\`. All other contributors use PRs.
4. The owner promotes release-ready changes through a PR from \`develop\` to \`main\` / \`master\`.
5. Where a repository has no \`develop\` branch, submit a feature-branch PR directly into \`main\` / \`master\`.
6. Emergency fixes may target the stable branch through a \`hotfix/*\` PR. Integrate the fix back into \`develop\` when applicable.
7. Do not force-push or delete shared branches without express permission. Never force-push or delete the stable branch.

## Quality and reviews

1. **Do not merge with failing or unfinished applicable CI checks.** A GitHub setting that allows a merge does not waive this requirement.
2. Explain the purpose and scope of each PR and summarize tests or manual validation performed.
3. Address failing checks and relevant review feedback before merging. If CI is unavailable, document appropriate manual checks.
4. Keep unrelated changes in separate PRs; request an independent review for substantial work when a qualified reviewer is available.
5. Do not disable or weaken tests, workflows, or protections to make a PR pass without authorization.

## Releases and automation

1. Treat \`main\` / \`master\` as stable and release-ready.
2. Where configured, a merge into the stable branch can trigger an automatic versioned release **only after successful final validation**.
3. Follow the repository-specific versioning and deployment procedure; do not publish or deploy independently without authorization.
4. Do not add paid services, expensive scheduled jobs, or other resource-intensive automation without the owner's approval.

## Security and confidentiality

1. **Never commit or disclose credentials**, including passwords, API tokens, private keys, or secrets in files, logs, issues, PRs, or artifacts.
2. Keep private repository contents confidential; do not transmit them to third-party services without authorization.
3. Use your own account with two-factor authentication. Never share accounts or credentials.
4. Do not change collaborator access, repository settings, CI/CD permissions, security controls, or integrations without authorization.
5. Report exposed credentials or suspected security incidents to the owner promptly and privately.

## AI-assisted contributions

The human operating an AI coding agent remains accountable for reviewing, testing, and securing its changes. Agents must follow the same PR, validation, security, and release rules, and must not independently alter credentials, permissions, billing, or security settings.

## Compliance

**Technical capability is not authorization.** GitHub Free cannot enforce all of these requirements, especially for private repositories; the rules still apply. Exceptions require the owner's explicit approval. Repeated or serious violations can lead to removal of collaborator access.
