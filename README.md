# Black Duck CoPilot Gradle/Travis CI Example



Shows a working setup for using the Synopsys CoPilot integration to analyze the risk of project dependencies

## Travis CI Setup

The `.travis.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
after_success:
  - bash <(curl -s https://copilot.blackducksoftware.com/ci/travis/scripts/upload)
```

