# MP3 音樂剪輯工具｜免費線上裁切、剪接與合併音訊

Independent, ad-free browser tool by [Upliftorch](https://upliftorch.com/).

[線上使用 / Official demo](https://upliftorch.com/tools/mp3-cutter/) · [更多免費工具 / Free tools](https://upliftorch.com/tools)

## 功能與執行 / Usage

核心功能在瀏覽器執行；資料查詢、地圖、字型或第三方函式庫可能仍需網路。

The browser frontend may require network access for public data, map tiles, fonts or third-party libraries.

使用任何靜態 HTTP server 提供此資料夾，例如：

```sh
npx --yes http-server . -p 8080 -c-1
```

Open `http://localhost:8080/` or `/en/` for English. Files are not sample customer uploads. This repository contains only the selected tool frontend and required local assets.

### Optional video extraction

Audio editing uses Web Audio and the upstream lamejs library. Video extraction additionally expects `vendor/ffmpeg/ffmpeg.js`, `814.ffmpeg.js`, `ffmpeg-core.js` and `ffmpeg-core.wasm`. Those third-party binaries are not redistributed here. Obtain the compatible ffmpeg.wasm wrapper/core from the upstream project, comply with its licenses, and serve the required files locally. No native application binaries are included.

## Privacy / 隱私

- Removed advertising loaders, placements, ad account identifiers and tracking scripts.
- No personal identity, customer records, environment files, deployment credentials, account tokens or original Git history are included.
- Do not commit user-entered files, passwords, spreadsheet contents or credentials.
- External libraries, data providers and configured APIs can receive requests; local processing does not mean zero network activity.
- Public datasets are not bundled. Any existing public data-feed URLs remain dependencies, not a promise of continued availability or a license to redistribute the data.

## License

Upliftorch-authored source is MIT licensed; see [LICENSE](LICENSE). Third-party libraries, map tiles, data and optional media retain their upstream terms; see [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). The MIT license does not grant trademark rights or override third-party licenses.

## About Upliftorch

[Upliftorch 官網](https://upliftorch.com/) — tools and software development. The links above identify the original creator and official demo; they are not a search-ranking guarantee.
