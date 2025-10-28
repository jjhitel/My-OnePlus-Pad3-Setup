## **Environment**
- Tested On ColorOS 16.0.0.206

I prefer open-source modules, but for Android 16, I had to use alternatives for those that aren't working properly yet.

---

## **Magisk/KernelSU Modules**
- [ReZygisk](https://github.com/PerformanC/ReZygisk)
  - Implements the Zygisk API with a focus on open-source transparency, security, and performance.
- [Tricky Store](https://github.com/5ec1cff/TrickyStore)
  - Modifies the Android Key Attestation certificate chain to pass integrity checks.
- [PlayIntegrityFork](https://github.com/osm0sis/PlayIntegrityFork/actions/runs/18437509161)
  - Fixes Play Integrity and SafetyNet verdicts to get a valid attestation.
- [Integrity-Box](https://github.com/MeowDump/Integrity-Box)
  - An open-source keybox updater and toolset with various spoofing features to help pass Play Integrity.
- [Treat Wheel](https://t.me/zygote64_32)
  - A Zygisk module to help hide root and pass integrity checks.
- [LSPosed](https://github.com/JingMatrix/LSPosed)
  - Allows for real-time modifications to system and app behavior without altering APKs through an ART framework.