# 31825

First, read the [Renovate minimal reproduction instructions](https://github.com/renovatebot/renovate/blob/main/docs/development/minimal-reproductions.md).

Then replace the current `h1` with the Renovate Issue/Discussion number.

## Current behavior

When renovate-bot checks against the checkmk image, it generates a new PR with version: checkmk/check-mk-cloud:2.3.0 .

## Expected behavior

When renovate-bot checks against the checkmk image, it generates a new PR with version: checkmk/check-mk-cloud:2.3.0p* .

## Explanation

CheckMK uses the following schema for versioning:
- 2 (first number) -> Major
- 3 (second number) -> Minor
- p* (number behind p) -> Patch

The 0 in 2.3.0 seems to be constant as in: every major checkmk version has the 0 as the third number and it never changes.

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/31825
