# Running FinRL-X inside GitHub

This repository mirrors `AI4Finance-Foundation/FinRL-Trading` and adds GitHub-native runtime helpers.

## Interactive dashboard with GitHub Codespaces

1. Open **Code → Codespaces → Create codespace on main**.
2. Dependencies are installed automatically using Python 3.11.
3. The Streamlit app starts automatically on port `8501`.
4. GitHub forwards port 8501 and opens the FinRL Trading Dashboard in the browser.

## GitHub Actions smoke test

A separate `.github/workflows/finrl-smoke.yml` workflow is managed through the GitHub connector and verifies installation plus the Streamlit health endpoint.

## Important

Live/paper trading requires broker/API credentials. No secrets are committed by this import. Configure credentials only through GitHub Secrets or Codespaces Secrets.
