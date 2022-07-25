# LatexPresentationTemplate
[![Build](https://github.com/iwishiwasaneagle/LatexPresentationTemplate/actions/workflows/build.yml/badge.svg)](https://github.com/iwishiwasaneagle/LatexPresentationTemplate/actions/workflows/build.yml)
[![Publish](https://github.com/iwishiwasaneagle/LatexPresentationTemplate/actions/workflows/publish.yml/badge.svg)](https://github.com/iwishiwasaneagle/LatexPresentationTemplate/actions/workflows/publish.yml)

A simple beamerpresentation template for University of Glasgow students/staff/researchers/whoever

## Features

- Automatically builds the package on push to `master`
  - Prevents pushes from breaking the compilation
- Create a new release at midnight if there is new content
  - This includes a changelog, and a compiled PDF
- Some packages that I found useful
- A file structure that makes sense

## Installation

This template was designed to work with the [blang/latex-docker](https://github.com/blang/latex-docker) image, and [latex-workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) VSCode plugin. This is optional, do what you want!

Open VSCode in this container, and run the `Remote Container` extension. This will open a new
instance from within the docker container with all the extensions installed. Easy. 

## Automated Workflows

You will need to set a `personal access token` with the `repo` scope to enable scheduled releases. This then needs to be given the name `PAT` to enable the workflow to access it.

- https://github.com/settings/tokens
- https://docs.github.com/en/actions/security-guides/encrypted-secrets
- [Relevant CI configuration file](https://github.com/iwishiwasaneagle/LatexPresentationTemplate/blob/e2941bd404f4932ce1199f5704b849eaec57d688/.github/workflows/create-tag.yml#L44)
