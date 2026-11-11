# Nix Workshop v0.0.4 beta smoke test

Use a disposable Git project and a free/local Ollama model. Do not share private code, credentials, or full logs in public issues. This is a **manual** validation checklist, not a claim that any steps have passed.

## Environment

- Date and tester (alias is fine):
- Windows version:
- VS Code version:
- Ollama version:
- Local model name and tag:
- Nix Workshop VSIX: v0.0.4-beta

For **each numbered step**, record **PASS / FAIL / BLOCKED / NOT AVAILABLE**. Provide observed behavior and exact reproduction steps for FAIL or BLOCKED; do not convert those outcomes to PASS. If a capability is absent from this beta, record NOT AVAILABLE rather than assuming support.

## Ten-step smoke test

1. Install the v0.0.4-beta VSIX on Windows in VS Code; record installation and activation behavior.
2. Start Ollama with a locally available coding model.
3. Connect Nix Workshop to that local model.
4. Ask a question and check that chat responds.
5. Open a test file and ask a code-context question.
6. Request a small edit and inspect the native VS Code diff **before** applying.
7. Reject an edit and verify that the test file remains unchanged (compare Git diff or file hash).
8. Approve a different edit and verify the actual file change.
9. Stop or hide the model and check that the extension reports a recoverable error. **Then restore Ollama and the same model; confirm it responds before proceeding.** Record the restoration outcome separately in step 9. If recovery fails, mark step 10 BLOCKED rather than treating its downstream failure as a successful lifecycle test.
10. Restart VS Code and repeat a chat **and** proposed edit after model availability has been restored. Record activation, chat, diff, and approval behavior.

## Result record

| Step | PASS / FAIL / BLOCKED / NOT AVAILABLE | Observed result / reproduction (redacted) |
| --- | --- | --- |
| 1. Install / activate | | |
| 2. Start Ollama | | |
| 3. Local connection | | |
| 4. Chat | | |
| 5. Code context | | |
| 6. Diff review | | |
| 7. Reject unchanged | | |
| 8. Approve edit | | |
| 9. Model error and restore | | |
| 10. Restart, chat and edit | | |

Additional observations: sidebar clipping, unexpected network or paid-API requests, reproducibility, and sanitized screenshots/errors. If attempting rollback, **label it separately as exploratory** and report the exact behavior. Do not claim rollback is a v0.0.4 feature or verified unless you can demonstrate it.

Report results on [tester issue #3](https://github.com/BillyMixNix/nix-workshop-releases/issues/3) or as a separate bug issue. Redact tokens, usernames, personal paths, private source, and sensitive logs.
