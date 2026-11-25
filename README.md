# Azri — update files / ملفات التحديث

This repository holds only the **signed update files** of Azri, the Premiere Pro panel. The code itself is private.

- Every release has three files: `azri-<version>.zip`, `latest.json` (version, what is new, the zip's SHA-256) and
  `latest.json.sig` (an Ed25519 signature by the publisher's key).
- Azri reads `releases/latest/download/latest.json`, believes it only when the signature matches the key built into the
  plugin, checks the zip's SHA-256, and installs only the engine and the panel. Nothing about the computer is sent.
- There is nothing to download here by hand: Azri shows «🆕 في نسخة جديدة» and installs it itself.

المستودع ده فيه ملفات التحديث الموقّعة بس. أزري بيقرا آخر نسخة من هنا، يتأكد من الإمضاء والبصمة، ويركّب التحديث لوحده.
