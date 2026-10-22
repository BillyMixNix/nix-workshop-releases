# Nix Workshop v0.0.4 beta smoke test

Use a disposable project. Do not share private code, credentials, or full logs in public issues.

1. Install the VSIX on Windows in VS Code.
2. Start Ollama with a locally available coding model.
3. Connect the extension to the local model.
4. Ask a question and check that chat responds.
5. Open a test file and ask a code-context question.
6. Request a small edit and inspect the native VS Code diff.
7. Reject an edit and confirm the file stays unchanged.
8. Approve a different edit and verify the result.
9. Stop or hide the model and check that the extension reports a recoverable error.
10. Restart VS Code and repeat a chat and edit.

Record: Windows version, VS Code version, Ollama version, model name, pass/fail for each step, and exact reproduction steps for any failure. Redact tokens, personal paths, and source code before opening a public issue.

This checklist is for human testing, not evidence that the checks have passed.
