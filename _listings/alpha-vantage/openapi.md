---
swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 1
info:
  title: Alpha Vantage
  description: alpha-vantage-apis-are-grouped-into-four-categories-1-stock-time-series-data-2-physical-and-digitalcrypto-currencies-e-g--bitcoin-3-stock-technical-indicators-and-4-sector-performances--all-apis-are-realtime-the-latest-data-points-are-derived-from-the-current-trading-day--
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=DIGITAL_CURRENCY_INTRADAY:
    get:
      summary: Digital Currencies Intraday
      description: This API returns the realtime intraday time series (in 5-minute
        intervals) for any digital currency (e.g., BTC) traded on a specific market
        (e.g., CNY/Chinese Yuan). Prices and volumes are quoted in both the market-specific
        currency and USD.
      operationId: getDigitalCurrenciesIntraday
      x-api-path-slug: queryfunctiondigital-currency-intraday-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Intraday
      - Time Series
  /query?function=DIGITAL_CURRENCY_DAILY:
    get:
      summary: Digital Currencies Daily
      description: This API returns the daily historical time series for a digital
        currency (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan),
        refreshed daily at midnight (UTC). Prices and volumes are quoted in both the
        market-specific currency and USD.
      operationId: getDigitalCurrenciesDaily
      x-api-path-slug: queryfunctiondigital-currency-daily-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Daily
      - Time Series
  /query?function=DIGITAL_CURRENCY_WEEKLY:
    get:
      summary: Digital Currencies Weekly
      description: This API returns the weekly historical time series for a digital
        currency (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan),
        refreshed daily at midnight (UTC). Prices and volumes are quoted in both the
        market-specific currency and USD.
      operationId: getDigitalCurrenciesWeekly
      x-api-path-slug: queryfunctiondigital-currency-weekly-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Weekly
      - Time Series
  /query?function=DIGITAL_CURRENCY_MONTHLY:
    get:
      summary: Digital Currencies Monthly
      description: This API returns the monthly historical time series for a digital
        currency (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan),
        refreshed daily at midnight (UTC). Prices and volumes are quoted in both the
        market-specific currency and USD.
      operationId: getDigitalCurrenciesMonthly
      x-api-path-slug: queryfunctiondigital-currency-monthly-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Monthly
      - Time Series
---