# Source provenance

- Original project: Binance Trade Bot, maintained upstream as `ccxt/binance-trade-bot`.
- Original author credited upstream: Eden Gaon.
- Upstream trading source revision: `55f8cbbe082bd083a722cba697f708a07f5add16`.
- Preparation date: 2026-10-29 (Europe/Moscow).
- Original GPL-3.0 LICENSE is retained unchanged.

## Package changes

- Preserved all Python files in `binance_trade_bot` and the dependency versions without changing trading logic.
- Included English and Russian README files describing archive downloads from release v1.1.0 and direct launch of the extracted executable.
- Included an account-independent release title, release description, and publishing instructions.
- Retained the blank API credentials and `testnet=true` in `.user.cfg.example`.
- Removed obsolete repository-link configuration tooling and the historical upstream README from this upload package. Original project attribution is preserved in the main README files and this provenance record.
- Removed inherited `logo` and `repository` URL fields from the optional deployment manifest. Other deployment fields are retained as legacy source configuration, without validation of the deployment platform.
- No executable, automatic uploader, or command-file launcher is included.

This is a source and documentation package. Windows compilation, executable behavior, dependency installation, and exchange connectivity were not tested. The archive download instructions describe the intended separately published binary package.
