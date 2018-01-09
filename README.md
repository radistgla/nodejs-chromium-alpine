# nodejs-chromium-alpine

Image providing `headless chrome`

## Overview

The main purpose of this image is to use it in CI pipelines for executing unit tests

For example, for [Gitlab CI](https://about.gitlab.com/features/gitlab-ci-cd/):

```yaml
...

ng-test:
  image: radistgla/nodejs-chromium-alpine:latest
  stage: test
  script:
    - $(npm bin)/ng test --single-run --progress false

...
```

## License

[MIT](https://github.com/radistgla/nodejs-chromium-alpine/blob/master/LICENSE).
