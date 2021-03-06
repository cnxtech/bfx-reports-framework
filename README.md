# Bfx Reports Framework

## Description

Bfx Reports Framework is a Reactjs and Nodejs open source framework with License Apache 2.0 for Bitfinex and Ethfinex users that can be used to build financial Reports. </br>
When running the software the result is similar to what is hosted on https://www.bitfinex.com/reports </br>
Including main structures and libraries gives the possibility for developers to create their personalized reports. </br>

Bfx Reports Framework can be run by its own, without need of adding code, it already includes some exiting features not included on what is hosted on website.

### Included Features
- All reports and tools from https://www.bitfinex.com/reports
- Possibility to work without a connection to internet.
- All ledgers and wallet values expressed in USD or other Forex currency

### Composition
- https://github.com/bitfinexcom/bfx-report-ui UI components
- https://github.com/bitfinexcom/bfx-report-express Express server
- https://github.com/bitfinexcom/bfx-report Base from where back-end service extends from

## Setup

### Install

- Clone Github repository and install projects dependencies :

```console
git clone https://github.com/bitfinexcom/bfx-reports-framework.git
cd bfx-facs-reports-framework
npm run init
```

### Configure service

When running `node init.sh` configuration is done automatically. </br>
As to check instructions of how to configure each component, visit the git repositories of the components listed above.

## Other Requirements

### Grenache network

- Install `Grenache Grape`: <https://github.com/bitfinexcom/grenache-grape>:

```console
npm i -g grenache-grape
```

## Run

As to run the software, is needed to run the network and each component separately.

### Run grenache network

- Run two Grapes

```console
grape --dp 20001 --aph 30001 --bn '127.0.0.1:20002'
grape --dp 20002 --aph 40001 --bn '127.0.0.1:20001'
```

### Run back-end service

- From `bfx-reports-framework` folder, run:

```console
npm run start
```

### Run express service

- From `bfx-reports-framework/bfx-report-ui/bfx-report-express` folder, run:

```console
npm run start
```

### Run UI

- From `bfx-reports-framework/bfx-report-ui` folder, run:

```console
npm run start
```


## Testing

### Run tests

```console
npm test
```
