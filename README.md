# ポートフォリオ

現在、42Tokyoに所属し、C/python/goを用いて低レイヤーおよびソフトウェアエンジニアリングを学びながら、建設・BIM、機械学習、データ基盤、Physical AIの領域で開発と事業検証に取り組んでいます。

課題発見から、顧客ヒアリング、仮説構築、要件定義、実装、評価までを一貫して進めることに関心があります。単にスキルを学び、技術を実装するだけでなく、「誰の、どの判断を、どう改善するのか」を考えながらビジネスにつながるプロダクトをつくることを重視しています。

## Recent Work

### Software Engineering Internship — Private Company Work

2025年12月から2026年2月中旬まで、Digital GridでCTO直下のソフトウェアエンジニアインターンを経験しました。

気象庁が提供するGRIB2形式の気象データを扱う処理に関わり、Python / FastAPI / PostgreSQL / Dockerを中心に、データ取得・解析、API、データベース、ジョブ実行環境、テストに取り組みました。

企業で開発した成果物のため、ソースコードおよび内部構成は非公開です。

### Machine Learning — GCI Final Project

東京大学松尾・岩澤研究室が提供するGCIを受講し、

従業員の離職データを題材に、EDA、特徴量設計、クラス不均衡を考慮したモデル評価、交差検証、時系列を意識した検証を行いました。予測精度だけで完結させず、モデルの出力をどのような人事施策や意思決定につなげるかまで検討しました。

### Physical AI / Autonomous 4WD Car

松尾・岩澤研究室のPhysical AIプログラムを受講しphysical AI領域を体系的に学んでいます。

並行してRaspberry Pi 5と4WD車体を用いた自律走行ミニカーの開発を進めています。　（一時中断）

Raspberry Pi CameraとOpenCVを用いた小規模な制御ループで画像認識・経路判断ロジックを実装し、そしてAckermann Steering向けの出力を左右輪の差動駆動へ変換する構成を検討しています。安全性を重視し、モーター制御の抽象化、Mock実装、明示的な走行許可、通信途絶時のWatchdog停止、例外・シグナル受信時の安全停止を含む設計で進めています。


## Public Code / 42 Tokyo Foundations

以下は、42 Tokyoの制約下で実装した公開コードの一部です。

### [Codexion](https://github.com/pito-42/codexion)

CとPOSIX Threadsを用いた並行処理シミュレーションです。

FIFO / EDFの2種類のスケジューリング、カスタム二分ヒープ、条件変数による待機、2資源の同時割当によるデッドロック回避、部分初期化失敗時のリソース解放、ログ出力の競合防止を実装しました。

### [A-Maze-ing](https://github.com/pito-42/a-maze-ing)

Python製の設定駆動型迷路生成・可視化アプリケーションです。

2人チームで開発し、私は迷路生成ロジックと描画を担当しました。DFS / Primによる迷路生成、BFSによる最短経路探索、乱数シードによる再現、生成処理とUIの責務分離を実装しています。

### [Push Swap](https://github.com/pito-42/push_swap)

制約されたスタック操作だけを用いて整数列を整列するCプログラムです。

小規模入力には専用処理を使い、大規模入力ではLongest Increasing Subsequenceと、各要素を戻すための操作コスト計算を組み合わせました。正しさだけでなく、出力する操作数の削減も評価対象として実装しました。

## Technologies

C / Python / Go / FastAPI / PostgreSQL / Docker / OpenCV / PyTorch / ONNX Runtime / GitHub Actions / Raspberry Pi / Next.js / React / Typescript


## Interests

full stack engineering / Business Architecture / Backend Engineering / Data Pipelines / Machine Learning Systems / Physical AI / 
