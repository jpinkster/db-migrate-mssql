# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.1] - 2019-04-14
### Fixed
- Invalid object name '[your-schema].migrations'. Was caused by checking the `recordset` property that is already removed by the `all` and `runSql` functions.

## [1.0.0] - 2019-04-13
I've built db-migrate-mssql today. I started from a fork of https://github.com/db-migrate/pg . Took me about half a day to build it, and it's working. Without transactions for now. I'm sure there's room for improvement though. If you want to try, run: yarn add @devotis/db-migrate-mssql

I've not adapted the tests from pg to mssql yet, so no guarantees, but I'm able to migrate up and down. I tried only runSql thus far.
