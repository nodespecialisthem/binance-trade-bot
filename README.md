# Binance Trade Bot for Windows

An independently maintained Windows distribution of the open-source Binance Trade Bot project.

## Download — v1.1.0

**Open Releases → select v1.1.0 → expand Assets → download `BinanceTradeBot.zip` or `BinanceTradeBot.rar`.**

Choose one archive format: ZIP or RAR. Both download options are named `BinanceTradeBot`; you only need one. The executable inside is named **`BinanceTradeBot-Windows-x64.exe`**.

The **Code → Download ZIP** option and the automatically generated **Source code** archives contain source files rather than the Windows application package.

## Extract and launch

1. Download **`BinanceTradeBot.zip`** or **`BinanceTradeBot.rar`** from **Releases → v1.1.0 → Assets**.
2. Extract the complete archive to a dedicated folder you can write to. Do not run the application from inside the archive viewer.
3. Keep the included configuration files and other resources in their original locations.
4. Configure the application as described below before enabling trading.
5. Open the extracted folder and double-click **`BinanceTradeBot-Windows-x64.exe`** to launch the application directly.

## Configuration

For a build using the published source configuration format:

- Copy the supplied `user.cfg.example` to **`user.cfg`**. If the archive does not include the template, obtain `.user.cfg.example` from the repository and save a copy as `user.cfg` beside the executable.
- Enter your credentials and settings locally. The source template contains blank API credentials and uses **`testnet=true`**.
- Keep **`supported_coin_list`** beside the application and review its symbols for the selected exchange environment. If it is missing from the package, obtain it from the matching source revision.
- Set `current_coin` deliberately. In the upstream implementation, leaving it empty can cause the bot to choose and buy a coin from the configured list.
- Keep the **`data`**, **`logs`**, and **`config`** folders with the application. Create them if they are required by your build and are not supplied or created automatically.

Keep your personal `user.cfg` and API credentials private. Test the setup in a test environment before considering live trading.

The exact settings and companion files depend on how the executable was built. Check the release notes for build-specific requirements.

## What the source project does

The Python implementation monitors relative cryptocurrency prices and can trade between configured coins through a bridge currency such as USDT. The repository includes strategy code, configuration examples, and historical-data backtesting code.

## Troubleshooting

| Problem | What to check |
| --- | --- |
| The executable cannot be found | Extract the complete `BinanceTradeBot` archive and open the extracted folder |
| Configuration is not found | Check that the file is named `user.cfg`, not `user.cfg.txt`, and is in the location expected by the build |
| Coin list is missing or empty | Check `supported_coin_list` and symbol availability in the selected environment |
| Log or database path errors | Check the `logs` and `data` folders and write permissions |
| The application closes or displays an error | Record the exact error and review any available logs; include the release version and Windows version in an issue |

Never attach API secrets or your full personal configuration to a public issue.

## Release information

The download instructions target **v1.1.0**. Supported Windows versions, the source revision used for the executable, build instructions, and test results should be documented by the maintainer in the release notes. The existence of an archive alone does not establish verified compatibility.

## Attribution and license

Based on **Binance Trade Bot**, originally created by **Eden Gaon**. This distribution is independently maintained. The original source license is **GPL-3.0**; see `LICENSE`.

Automated cryptocurrency trading can cause losses. No profit or performance is guaranteed.
