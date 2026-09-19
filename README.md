# zabbix_thermo_esp32-firmware

ESP32(Seeed XIAO ESP32C6)用ファームウェアの**配布専用**リポジトリです。ソースコードは含みません。

- ファームウェアの `.bin` と、公開済みの版の一覧 `manifest.json` は、このリポジトリの
  **Releases** に置かれます(Gitのファイルとしては置きません)
  - `xiao-esp32c6-latest` … 版の一覧 `manifest.json`(最新版の指し先を含む)
  - `xiao-v<版>` … 各版の `xiao_esp32c6_thermo.bin`
- 機器(ESP32)が、認証なしのHTTPSで `manifest.json` を取得し、自動または手動でファームウェアを更新します
- 公開は、配布元の公開スクリプトから行います。手作業でReleaseを編集しないでください
  (`manifest.json` と各 `.bin` のMD5が食い違うと、機器は更新を拒否します)

manifestのURL:
`https://github.com/kake359/zabbix_thermo_esp32-firmware/releases/download/xiao-esp32c6-latest/manifest.json`
