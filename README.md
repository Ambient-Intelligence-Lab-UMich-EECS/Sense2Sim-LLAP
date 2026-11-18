# LLAP · Pilot study: offline package

在线版 / Online: https://ambient-intelligence-lab-umich-eecs.github.io/Sense2Sim-LLAP/

- LLAP · Pilot study, Version 20 (Great Lakes run 51, kit bb8886d7)
- Sensing Universe: the SenseWeaver knowledge base; the Model rating filter starts with A and B
- Sensing World: its spaces as of 2026-11-17, built from SenseWeaver main c1070103 (unified/all/spaces/sim)
- 3D asset gallery: the SenseWeaver asset pack, 230 models (pack of 2026-11-12); credits and licences in CREDITS.md
- Packed 2026-11-18 by tools/offline.mjs (SenseWeaver claude/project-thread-pvay98, 52d85c0)

## 打开方式

1. 解压后双击 `index.html`。推荐用 Chrome 或 Edge；不需要网络。
2. 页面链接到的页面（`pages/` 里：“SenseWeaver Knowledge Base Review”, “Sensing World”, “SenseWeaver 资产包”）都在包里。
3. 相机：在模拟器页面按 “Camera”，浏览器问是否允许使用相机时选允许。手和上半身的追踪（MediaPipe）在包里，不需要网络。
   如果浏览器不让从磁盘打开的页面用相机（例如 Safari），在这个文件夹里运行 `python3 -m http.server 8000`，再打开 http://localhost:8000/ 。

仍需联网的只有这些链接（点开时才需要）：
   - https://www.youtube.com/watch?v=gs8wMrOSY80&t=20s

## How to open

1. Unzip, then double-click `index.html`. Chrome or Edge recommended; no network needed.
2. The pages it links to (under `pages/`: “SenseWeaver Knowledge Base Review”, “Sensing World”, “SenseWeaver 资产包”) are in the package.
3. The camera: on a simulator page press “Camera” and allow the camera when the browser asks. Hand and upper-body tracking (MediaPipe) is in the package and needs no network.
   Where a browser does not give the camera to a page opened from the disk (Safari, for one), run `python3 -m http.server 8000` in this folder and open http://localhost:8000/ .

Only these links still need the network (when clicked): 
   - https://www.youtube.com/watch?v=gs8wMrOSY80&t=20s

## What is in it

- `index.html`: the page, as built, with its loads pointed at the package (offline.json lists every line rewritten)
- `pages/sensing-universe/`: a copy of the page “SenseWeaver Knowledge Base Review”
- `pages/sensing-world/`: a copy of the page “Sensing World”
- `pages/asset-gallery/`: a copy of the page “SenseWeaver 资产包”
- `CREDITS.md`
- three@0.170.0, from npm
- @mediapipe/tasks-vision@0.10.35, from npm
- hand_landmarker.task (7.5 MB, sha256 fbc2a30080c3…), the camera's model
- pose_landmarker_lite.task (5.5 MB, sha256 59929e1d1ee9…), the camera's model
- 98 font files from Google Fonts, inlined

Made by tools/offline.mjs (SenseWeaver, skill senseweaver6); `offline.json` gives each file's bytes and sha256 and where each came from.
