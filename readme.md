[![Build](https://github.com/haampie-spack/ci-example-2/actions/workflows/ci.yaml/badge.svg)](https://github.com/haampie-spack/ci-example-2/actions/workflows/ci.yaml)

Edit: you may want to use the Github Action instead: https://github.com/haampie-spack/setup-spack

# CI for C / C++ / Fortran / Python projects using Spack

- Set up Spack through https://github.com/haampie/spack-batteries-included;
- Use (a matrix of) compilers from github actions (see https://github.com/actions/virtual-environments);
- Reuse binaries, sources and ccache to speed up your n'th build.

All you need is a [workflow](.github/workflows/ci.yaml), an [environment file](ci/spack.yaml) and a [spack package](ci/repo/packages/mypkg/package.py).
