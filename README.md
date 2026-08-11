# ポートフォリオ

42 TokyoでC・python・go等で定レイヤーおよびソフトウェアエンジニアリングを学びながら、建設・BIM、機械学習、データ基盤、Physical AIの領域で開発と事業検証に取り組んでいます。

課題発見から、顧客ヒアリング、仮説構築、要件定義、実装、評価までを一貫して進めることに関心があります。単に技術を実装するだけでなく、「誰の、どの判断を、どう改善するのか」を考えながらビジネスにつながるプロダクトをつくることを重視しています。

## Recent Work

### Construction Tech / BIM — Private

共同創業を前提とした建設領域の新規事業の立ち上げ準備・事業検証に、2人を中心とした体制で取り組みました。

業界調査、企業への架電、顧客ヒアリング、課題仮説・事業仮説の構築、要件定義、デモ設計・実装、顧客へのデモ、PoC提案、価格提示までを共同で進めました。一部企業からは、動作条件を満たした場合の利用検討と、実データを用いた検証の許可を得る段階まで進みました。会社設立・正式ローンチ前の事業検証として実施したものです。

現在はこの経験を基に、BIM × AI領域での事業化も視野に入れた検証を個人で進めています。顧客名、事業仮説の核心、具体的な開発内容、ソースコードは非公開です。

### VoltDelta — Private Technical MVP

電気設備平面図の旧版・新版PDFを比較し、設備記号の追加・削除・移動候補と、数量・直接費への影響候補を根拠付きで提示する変更影響分析システムです。

自動判定で業務判断を置き換えるのではなく、人間が根拠を確認し、修正・承認できるHuman-in-the-loop型の設計を採用しています。

合成・自作データを決定論的に生成し、元平面単位で学習・検証データを分割することでデータリークを防止しました。また、テンプレート照合と学習モデルを同じ評価データ・評価規則・下流処理で比較し、Locked Testを用いて採否を判断しています。

Python、FastAPI、OpenCV、PyTorch、ONNX Runtime、PostgreSQL、Docker、GitHub Actionsなどを使用しています。現時点では実図面に対する一般的な実用性は未検証であり、技術MVPとしての検証範囲を明示しています。こちらは事業化を見据えてはいませんでしたが、上記事業との関係からリポジトリは非公開です。

### Software Engineering Internship — Private Company Work

2025年12月から2026年2月中旬まで、Digital GridでCTO直下のソフトウェアエンジニアインターンを経験しました。

気象庁が提供するGRIB2形式の気象データを扱う処理に関わり、Python / FastAPI / PostgreSQL / Dockerを中心に、データ取得・解析、API、データベース、ジョブ実行環境、テストに取り組みました。

企業で開発した成果物のため、ソースコードおよび内部構成は非公開です。

### Machine Learning — GCI Final Project

東京大学松尾・岩澤研究室が提供するGCIを受講し、

従業員の離職データを題材に、EDA、特徴量設計、クラス不均衡を考慮したモデル評価、交差検証、時系列を意識した検証を行いました。予測精度だけで完結させず、モデルの出力をどのような人事施策や意思決定につなげるかまで検討しました。

### Physical AI / Autonomous 4WD Car — In Progress

松尾・岩澤研究室のPhysical AIプログラムを受講しphisical AI領域を体系的に学んでいます。

Raspberry Pi 5と4WD車体を用いた自律走行ミニカーの開発を進めています。

画像認識・経路判断ロジックを実装し、Raspberry Pi CameraとOpenCVを用いた小規模な制御ループ、そしてAckermann Steering向けの出力を左右輪の差動駆動へ変換する構成を検討しています。安全性を重視し、モーター制御の抽象化、Mock実装、明示的な走行許可、通信途絶時のWatchdog停止、例外・シグナル受信時の安全停止を含む設計で進めています。
現在は一時中断中。

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
