# METbot-ccxt

METbot-ccxt is a private multi-exchange crypto spot trading bot powered by `ccxt`.

It is designed for traders who want a configurable automation tool with risk controls, Telegram monitoring, exchange-side protective stops when supported, diagnostics, reports, and private licensed delivery.

> METbot-ccxt is trading automation software. It is not financial advice and does not guarantee profit.

## What It Does

- Automates spot trading for a selected `BASE/QUOTE` market.
- Connects to exchanges through `ccxt`.
- Uses configurable timeframe and higher-timeframe trend filters.
- Applies entry filters for market quality, volatility, spread, volume, and orderbook conditions.
- Uses risk-based position sizing and max trade controls.
- Places exchange-side protective stops when the exchange supports them.
- Supports trailing stop, stop tightening, partial take profit, and re-entry logic.
- Provides Telegram commands for status, audit, reports, health checks, manual actions, and emergency control.
- Keeps decision logs and trade journals for later analysis.
- Includes shadow profiles for comparing alternative strategy modes without risking real funds.
- Includes watchdog and startup reconciliation logic for safer long-running operation.
- Uses a signed local `LICENSE_KEY` for private licensed delivery.

## Market Type

The current version is built for spot trading.

It does not:

- use leverage;
- open short positions;
- use futures margin modes;
- calculate liquidation price;
- use reduce-only orders;
- use funding-rate logic.

Futures or margin support would require separate development and exchange-specific testing.

## Delivery After Purchase

After purchase, the buyer receives:

- access to a private GitHub repository or private release;
- source code for the purchased version;
- setup documentation;
- `.env.example`;
- `LICENSE_KEY.example`;
- one signed `LICENSE_KEY` for the buyer.

The license is intended for:

- one buyer;
- one GitHub account;
- private use;
- no resale;
- no redistribution;
- no public upload.

## Safety Features

METbot-ccxt includes several protection layers:

- paper mode for testing before live trading;
- max trade size;
- risk-per-trade sizing;
- protective stop support;
- strict protective-stop mode;
- orderbook/slippage guard;
- spread guard;
- circuit breaker;
- loss guard;
- startup reconciliation;
- state synchronization after orders;
- external watchdog support.

These features reduce operational risk, but they do not remove trading risk.

## Telegram Monitoring

The bot includes Telegram-based monitoring and control commands such as:

- `/status`
- `/audit`
- `/health`
- `/watchdog`
- `/report`
- `/risk`
- `/missed`
- `/tuning`
- `/pause`
- `/resume`
- `/buy`
- `/sell`
- `/panic`
- `/sync`

Exact available commands may depend on the purchased version.

## Supported Exchanges

METbot-ccxt is based on `ccxt`, so the architecture is multi-exchange.

Each exchange must still be tested before live trading because exchanges differ in:

- API permissions;
- market symbols;
- min order amount;
- min order cost;
- precision;
- stop-order support;
- trigger-order parameters;
- order status APIs.

Before live use, the buyer should verify exchange behavior in paper mode and with a very small live trade.

## Important Risk Notice

Cryptocurrency trading is risky.

The buyer is responsible for:

- choosing the exchange;
- securing API keys;
- disabling withdrawal permissions;
- using paper mode first;
- testing with small position sizes;
- monitoring live operation;
- understanding market risk;
- accepting that losses can happen.

METbot-ccxt is automation software, not a guaranteed profitable strategy.

## What Is Not Included

Unless separately agreed, the purchase does not include:

- guaranteed profit;
- financial advice;
- exchange account setup;
- hosting or VPS;
- custom strategy development;
- futures/margin support;
- tax advice;
- recovery of trading losses.

## FAQ

### Is the source code public?

No. The source code is delivered through a private repository or private release after purchase.

### Can I resell it?

No. The standard license is for one buyer and one GitHub account. Resale and redistribution are not allowed.

### Can I modify it?

Yes, for your own private use, unless your individual agreement says otherwise.

### Does it guarantee profit?

No. No trading bot can guarantee profit.

### Does it support futures?

The current version is built for spot trading. Futures or margin support would require separate development and testing.

### Do I need API keys?

Yes, for live trading. API keys should never have withdrawal permissions.

### Can I test before live trading?

Yes. Start with `PAPER_MODE=true`, run diagnostics, and only then consider live mode with a very small max trade.

## Purchase and Contact

For access, pricing, or questions, contact:

- Telegram: `@artemius001`
- Email: `artem@president-kids.ru`
