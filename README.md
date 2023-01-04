# Data Science Template

## File Structure

```text
├── src/
│   ├── common/                 <- 放不同階段會共用的程式碼，或無關階段會使用的程式碼
│   │   └── common.R            <- import packages
│   ├── s0_pre_process/         <- 各階段用 s0, s1, ... 開頭，後面接階段名稱
│   └── s1_first_process/
├── data/
│   ├── raw/                    <- 放原始資料
│   ├── interim/                <- 放處理過但未處理完成的資料
│   ├── processed/              <- 放處理完成的資料
│   ├── external/               <- 放外部資料
│   └── temp/                   <- 放暫存資料
├── results/                    <- 放輸出結果
├── references/                 <- 放參考文件
├── .devcontainer/              <- dev containers 相關設定
│   ├── python/
│   │   ├── .devcontainer.json
│   │   └── Dockerfile
│   └── R/
│       ├── .devcontainer.json
│       └── Dockerfile
├── .rstudio_config/            <- RStudio 相關設定
├── .vscode/                    <- VSCode 相關設定
│   ├── keybindings.json        <- 快捷鍵設定，需自行套用到 user 層級的 keybindings.json 才會有效
│   └── settings.json           <- workspace 層級的 settings
├── .dockerignore
├── .env                        <- 環境變數，SESSION 在此設定
├── .gitignore
├── .lintr                      <- linter for R
├── docker-compose.yml
├── README.md
└── requirements.txt
```
