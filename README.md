# buck2-github-composite-action

This repo contains a [composite action] to download [Buck2] pre-built binaries
from the [official repository].

## Inputs

```yaml
inputs:
  release-tag:
    description: 'Release tag'
    required: true
    default: '2024-02-15'
  arch:
    description: 'Architecture'
    required: true
    default: 'x86_64'
  platform:
    description: 'Platform'
    required: true
    default: 'unknown-linux-gnu'
  sha384:
    description: 'SHA384'
    required: true
    default: '1442f2b6c1dfe0071a6c0cf3d3038e5b2b1488593555f60371c5fd1efa6d6fc4a4dc880203ddce699ba2100ce18092d7'
  output-path:
    description: 'Output path'
    required: true
    default: '/usr/bin/buck2'
```

[composite action]: https://docs.github.com/en/actions/creating-actions/about-custom-actions#composite-actions
[Buck2]: https://buck2.dev/
[official repository]: https://github.com/facebook/buck2/releases