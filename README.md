# BuildPulse Example Project: Java + Gradle + JUnit

This is an example [JUnit](https://junit.org/junit5/) project demonstrating how to send test results to [BuildPulse](https://buildpulse.io) to help you detect, track, and eliminate flaky tests.

## Connect JUnit to BuildPulse

After starting a [free trial](https://github.com/marketplace/buildpulse/plan/MDIyOk1hcmtldHBsYWNlTGlzdGluZ1BsYW40NzM5#pricing-and-setup), you can add BuildPulse to your project in just a few quick steps:

1. Identify the directory where your build is writing JUnit's XML test reports. (If you're using Gradle, the reports are written to `<project-root>/build/test-results` by default.)

2. Then, configure your build to send the JUnit XML reports to BuildPulse. [[example][commit-for-buildpulse-integration]]

    The [configuration][commit-for-buildpulse-integration] relies on your BuildPulse account ID, repository ID, key, and secret. You'll see this information when viewing your repository on buildpulse.io.

    This example uses GitHub Actions CI, but you can integrate just as easily with other CI providers as described below.

## Works with the CI you already have

BuildPulse offers integrations for:

- **CircleCI** [[docs](https://circleci.com/developer/orbs/orb/workshop64/buildpulse)]
- **GitHub Actions** [[docs](https://github.com/marketplace/actions/buildpulse)]
- **Semaphore** [[docs](https://github.com/Workshop64/buildpulse-semaphore)]
- **Travis CI** [[docs](https://github.com/Workshop64/buildpulse-travis-ci)]
- Buildkite (available in early access)
- Jenkins (available in early access)

Don't see your CI provider? [Get in touch](mailto:hello@buildpulse.io?body=%3C%3C%20Please%20tell%20us%20what%20CI%20service%20you%27re%20using.%20We%27ll%20follow%20up%20with%20you%20soon%21%20%3E%3E&amp;subject=Please%20add%20support%20for%20this%20CI%20service%20next) and we may be able to quickly add support for it.

---

<p>
  <a href="https://buildpulse.io?utm_source=github.com&utm_campaign=example-repositories&utm_content=junit-button">
    <img width="325" title="Automatically detect flaky JUnit tests with BuildPulse" alt="Try BuildPulse for free" src="https://user-images.githubusercontent.com/2988/86935247-9f059b80-c10a-11ea-9579-575b357e70d6.png">
  </a>
</p>

Automatically **detect flaky tests.** Focus on the top offenders to **quickly improve your builds.** Save developer time and frustration. **Regain trust in your test suite.**

👉 [Get started at buildpulse.io](https://buildpulse.io?utm_source=github.com&utm_campaign=example-repositories&utm_content=junit-text-link)

[commit-for-buildpulse-integration]: https://github.com/buildpulse/buildpulse-example-junit/commit/main
