# ITC - Terraform Module - Template

[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
![CI workflow](https://github.com/indigo-tangerine/itc-tfm-project-template/actions/workflows/ci-pr.yml/badge.svg)
![CD workflow](https://github.com/indigo-tangerine/itc-tfm-project-template/actions/workflows/cd.yml/badge.svg)

## Change this line

![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/indigo-tangerine/terraform-aws-itc-CHANGEME)

## Maintainer

* indigo-tangerine

## Description

Describe what your module does here.

## Sub-Modules

## Examples

See examples folder (if present)

## Usage

To auto generate terraform-docs for sub-modules add the paths to the working-dir in the ci.yaml workflow:

```(yaml)
- name: Render terraform docs inside the USAGE.md and push changes back to PR branch
        uses: terraform-docs/gh-actions@v0.10.0
        with:
          working-dir: .,modules/sub-module1-dir,modules/sub-module2-dir
          output-file: README.md
          output-method: inject
          git-push: "true"

```

## IMPORTANT - CHANGE REQUIRED TO MAKE SEMVER WORK

Remove the following line from cd.yml - this is required to make this repo work but will cause a failure if using this template repo in ohpensource repositories.

```(yaml)
token: ${{ secrets.CICD_GITHUB_REPOSITORY_TOKEN }}
```

<!--- BEGIN_TF_DOCS --->
<!--- END_TF_DOCS --->
