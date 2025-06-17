# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- XSS in HTML comment (some Markdown renderers will parse comments into the DOM) -->
<!-- <img src=x onerror=alert('XSS-comment')> -->

## Unreleased

<script>alert('XSS-unreleased-section')</script>

## 2025-01-07 - 1.0.1

### Fixed

- Fixed issue with incorrect cursor `<img src=x onerror=alert('XSS-fixed')>`

## 2024-09-20 - 1.0.0

### Changed

- Changed lookback period for the "cold start" from 30 days to 1 hour `<svg/onload=alert('XSS-changed')>`
