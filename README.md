# Workflow (wfl)

<!-- Banner & Badges. Badges should have newlines -->
<!-- [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme) -->

👷🏻‍♂️ Workflow repository for CI/CD systems


## Table of Contents
<!-- - Must link to all Markdown sections in the file.
- Must start with the next section; do not include the title or Table of Contents headings.
- Must be at least one-depth: must capture all `##` headings. -->
- [Background](#background)
- [Usage](#usage)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [License](#license)

## Background

A reusable template / remote repository for workflows to integrate in CI/CD systems. Mainly (and possibly solely) steered towards usage in Github Actions via [reusable workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows#overview).

## Usage

Covered quite good in the [Github Actions documentation](https://docs.github.com/en/actions/using-workflows/reusing-workflows#overview).

```yaml
jobs:
  esphome:
    runs-on: ubuntu-latest
    steps:
      - uses: thibmaek/wfl/.github/workflows/compile_esphome.yaml@main
        with:
          esphome_dir: ./esphome
```

## Maintainer(s)

- [@thibmaek](https://github.com/thibmaek)

## Contributing

Not immediatly on my mind to accept contributions, but feel free to PR something if you find an improvement.

## License

Unlicense

For more info, see [license file](./LICENSE)
