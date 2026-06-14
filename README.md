# 龍山寺夢想火車

一座以台北龍山寺為核心，融合倫敦經典地標的明亮玩具鐵路世界。  
使用 Three.js 製作，可直接在瀏覽器中操作與欣賞。

## 網站首頁

### [開啟線上網站](https://YOUR-GITHUB-ACCOUNT.github.io/YOUR-REPOSITORY/)

> 發布前請將上方網址中的 `YOUR-GITHUB-ACCOUNT` 與 `YOUR-REPOSITORY`
> 替換成你的 GitHub 帳號及 repository 名稱。

[查看專案首頁檔案](./index.html)

## 靈感來源與致謝

本專案的玩具鐵路概念、視覺方向與互動設計，參考自
[Peter Gostev](https://github.com/petergpt) 創作的
[London Dream Railway](https://developers.openai.com/showcase/london-train)。

感謝 Peter Gostev 分享這個充滿創意的 Three.js 作品與製作過程，
讓本專案能以台北龍山寺為主題延伸出不同的城市鐵路版本。

- [原作線上展示](https://petergpt.github.io/london-train/)
- [原作 GitHub Repository](https://github.com/petergpt/london-train)

本專案並非原作的官方版本，也不代表 Peter Gostev 或 OpenAI。

## 畫面特色

- 以木製遊戲桌呈現色彩鮮明的立體玩具城市
- 台北龍山寺作為場景中心
- 收錄大笨鐘、國會大廈、倫敦塔橋、倫敦眼、聖保羅大教堂、碎片塔與巴特西發電站
- 紅色城市列車、Tube 風格列車及迷你 DLR 接駁車同時運行
- 高架軌道、橋墩、車站月台、河流、公園與可切換隧道
- 可操作的軌道轉轍器與列車跟隨視角
- 使用 InstancedMesh 呈現枕木、鐵軌、樹木、窗戶與重複物件
- 裝置像素比限制為 2，以兼顧畫質與效能

## 操作方式

| 控制項 | 功能 |
| --- | --- |
| 列車數量 | 調整同時運行的列車數量 |
| 列車速度 | 調整所有列車的運行速度 |
| 西側／東側轉轍器 | 將列車切換至不同路線 |
| 隧道剖面 | 隱藏隧道外殼，查看內部軌道 |
| 跟隨列車 | 讓攝影機跟隨行駛中的列車 |
| 攝影機預設 | 切換全桌、橋梁、車站及隧道視角 |
| 滑鼠拖曳 | 旋轉觀看角度 |
| 滑鼠滾輪 | 拉近或拉遠畫面 |

## 技術

- HTML5
- CSS3
- JavaScript ES Modules
- [Three.js](https://threejs.org/) `0.168.0`
- GitHub Pages

## 本機預覽

由於 Three.js 使用 ES Modules，建議透過本機伺服器開啟。

使用 Python：

```powershell
python -m http.server 4173
```

接著前往：

```text
http://127.0.0.1:4173
```

## 發布至 GitHub Pages

專案已包含 GitHub Actions 自動部署設定。

1. 在 GitHub 建立新的 repository。
2. 將本專案推送到 repository 的 `main` 分支。
3. 開啟 repository 的 `Settings`。
4. 選擇 `Pages`。
5. 在 `Build and deployment` 的 `Source` 選擇 `GitHub Actions`。
6. 等待 `Deploy static site to GitHub Pages` 工作完成。
7. 將本 README 上方的網站連結換成實際網址。

一般專案網站網址格式：

```text
https://你的帳號.github.io/repository名稱/
```

若 repository 名稱是 `你的帳號.github.io`，網址則為：

```text
https://你的帳號.github.io/
```

## 專案結構

```text
.
├── .github/
│   └── workflows/
│       └── deploy-pages.yml
├── .nojekyll
├── index.html
└── README.md
```

## 授權

本專案可作為個人展示與 Three.js 學習用途。若要公開散布或改作，
建議再依需求補上正式的開源授權條款。
