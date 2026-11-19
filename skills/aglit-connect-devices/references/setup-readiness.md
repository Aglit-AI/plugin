# Set up and verify computer control

Run these steps on the intended original computer, through an existing authorized connection. A cloud terminal is not the user's desktop. Keep the selected CLI environment, account server, account, employee/device registration, team and model settings. Use that environment's installed launcher; do not replace its profile or start an old executable.

## Inspect before changing setup

Check installed help and the running release:

```sh
aglit --help
aglit status --json
aglit update --check --json
aglit desktop status --json
aglit browser status --json
```

Inspect the actual response; CLI and native runtime versions are separate. A command or field missing from an older release means that check is unavailable. Update through the supported installer/updater when appropriate, preserving active work and any next-launch deferral. Do not substitute source files or another device's successful check.

For a new installation, follow the connection guide and run `aglit init` on that computer. For an enrolled installation, prefer `aglit init --repair` when its installed help advertises it; `--repair --json` is the unattended readiness report. Compatible repair mode keeps existing identity/settings and reports exact blockers. If unavailable, use the individual status checks and supported setup commands; do not assume rerunning ordinary init cannot change account, team or model choices.

## Check each layer

| Check | Evidence and next action |
|---|---|
| Original installation | Correct environment, device/employee and existing account. A stopped runtime needs its supported launcher; an offline or locked computer may need local attention. |
| Desktop control | On macOS, `aglit desktop status --json` must report `ready: true`. Follow `aglit desktop setup` for missing Screen Recording and Accessibility. `requiresUpdate` or an unavailable helper is a runtime/component issue, not permission success. The Mac permission check does not establish Windows input readiness. |
| Browser extension | `aglit browser status --json` must report `installed: true`, `enabled: true` and `connected: true`. Run `aglit browser setup` to prepare/connect the correct bundled or store extension in the existing Chrome profile. A production extension does not establish connection to a different environment's app. |
| Chrome profile access | On compatible macOS releases, `permissionRequired: "chrome-profile-access"` / `BROWSER_PROFILE_ACCESS_DENIED` identifies blocked profile inspection. Guided setup explains the scope, asks to open **Privacy & Security → Files & Folders**, and rechecks after approval. Allow **Google Chrome** only for the exact Aglit app/helper named by macOS. This can expose sensitive Chrome profile data; retain the normal user consent. Full Disk Access is not a substitute. |
| Remote access | If requested, verify Anywhere Access is both enabled and connected in the intended account/team. A visible roster entry, open port or successful registration is not a live connection. |
| Agent/model readiness | Preserve the selected provider, model and account connection. A detected login, catalog entry or deferred model choice does not prove inference. Report model readiness separately from desktop/browser transport. |

If the extension is visibly installed/enabled while status cannot detect it, inspect OS access and native-host diagnostics before repeatedly reinstalling. `detectionAvailable: false` is an unavailable check, not proof of absence. If installation succeeds but `connected` remains false, inspect the original native host and selected profile; preserve profile ambiguity checks, approvals and history. Use the supported browser setup/updater to repair registration rather than editing installed wrappers.

Computer Use can help navigate the existing Chrome profile and its setup screens after desktop control works. Discover the current `p1_computer_use` and `p1_browser_use` schemas, then follow the documentation returned by their initialization. Do not invent tools or use another employee's session. Permission changes and protected OS prompts keep their normal approval boundaries; do not silently toggle unrelated grants.

## Finish with actual control

Use the same original device to observe its live desktop and perform an authorized harmless input with visible readback. Then use its actual browser tool to read an existing permitted page or a temporary page owned by this setup, and verify a harmless browser action. Read-only discovery alone does not prove clicks or typing work. Preserve user tabs, login and other tasks.

Recheck status after the supported reconnect/restart when one was required. Report desktop viewing, desktop input, browser connection, browser actions, remote access and model inference separately. A successful init, permission toggle or plugin install is not enough to mark all layers ready. Keep precise blockers for unavailable checks, offline devices and required human actions; continue independent authorized repair.
