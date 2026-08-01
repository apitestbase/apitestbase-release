# API Test Base

[![Latest release](https://img.shields.io/github/v/release/apitestbase/apitestbase-release?label=latest%20release)](https://github.com/apitestbase/apitestbase-release/releases/latest)

API Test Base tests your API **and everything it does behind the scenes**: the database records it writes, the messages it puts on queues, the downstream services it calls. A single `POST /orders` call is verified end to end, in one automated test case:

    ✓ HTTP response = 200
    ✓ Order record created in database
    ✓ Message sent to queue
    ✓ Downstream API called successfully

It is free, with no account to create and no cloud behind it — you run it on your own machine or in your CI/CD pipeline, and build test cases in a no-code / low-code UI.

![API Test Base test case run result — three steps (set up database data, invoke the HTTP API, check the database) all passed, shown in green with per-step timings](https://apitestbase.io/screenshots/basic-use/test-case-run-result.png)

## Download

Get the [latest release](https://github.com/apitestbase/apitestbase-release/releases/latest) and follow the [Quick Start](https://apitestbase.io/docs/quick-start) to install API Test Base and create your first test case.

## Why API Test Base

Tools like Postman and Bruno make it easy to check an API's response, and for many APIs that is enough. Real APIs often do more, though — they write records to databases, publish messages to queues, and call downstream services. API Test Base verifies those side effects in the same test case, and it can trigger APIs that don't start with an HTTP request: a message arriving on a queue, a file dropped on an FTP or SFTP server, a SOAP call.

See [how API Test Base compares to Postman, Bruno and other API clients](https://apitestbase.io/comparison).

## Supported protocols and systems

* HTTP(S)
* SOAP
* Relational databases (Oracle, SQL Server, PostgreSQL, H2, etc.)
* IBM MQ
* JMS (ActiveMQ, Solace)
* AMQP
* MQTT
* FTP(S)
* SFTP
* Local files
* IBM ACE

## Website

[apitestbase.io](https://apitestbase.io) — documentation and guides.

---

This repository hosts API Test Base release binaries.