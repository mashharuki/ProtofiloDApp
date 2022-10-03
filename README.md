# ProtofiloDApp
ICP上で動作するDApp開発用のリポジトリです。

### DFXとは何か？
DFX とは DFINITY が提供する、開発したプロジェクトを IC にデプロイ、管理するための主要なツールです。

### dfxのインストールコマンド
 `sh -ci "$(curl -fsSL https://smartcontracts.org/install.sh)"`  
 `dfx --version`

### Svelteとは何か？
 Svelteとは、React や Vue などの JavaScript フレームワークに変わるツールです。  
 Svelteの特徴としては、アプリケーションの実行時にコードを解釈するのではなく、ビルド時に行います。また、他のフレームワークと比較しコードの記述量が少ないことも特徴です。

### Viteとは何か？
 2020年発表の新しいフロントエンドの高速ビルドツール

### TailWindcss のセットアップ
 `npx tailwindcss init  -p`

### ウォレットキャニスターを作成するためのコマンド
 `dfx canister --network=ic call fg7gi-vyaaa-aaaal-qadca-cai redeem '("655D7-BDB94-5F4A9")'`

 レスポンスの一例
 ```cmd
 (principal "pwult-uqaaa-aaaag-aau7a-cai")
 ```

### ウォレットキャニスターの状態を確認するコマンド
 `dfx canister --network=ic status "pwult-uqaaa-aaaag-aau7a-cai"`

 レスポンスの一例
 ```cmd
 Canister status call result for pwult-uqaaa-aaaag-aau7a-cai.
Status: Running
Controllers: wro4r-gzno2-ul3gr-lrqmq-rcww4-ye7v5-7fwxp-jlndv-pvwhh-zoveg-nae
Memory allocation: 0
Compute allocation: 0
Freezing threshold: 2_592_000
Memory Size: Nat(3786242)
Balance: 20_098_596_892_990 Cycles
Module hash: 0xb944b1e5533064d12e951621d5045d5291bcfd8cf9d60c28fef02c8fdb68e783
 ```

 `dfx identity --network=ic set-wallet "pwult-uqaaa-aaaag-aau7a-cai"`

 レスポンスの一例
 ```cmd
 Checking availability of the canister on the network...
Setting wallet for identity 'default' on network 'ic' to id 'pwult-uqaaa-aaaag-aau7a-cai'
Wallet set successfully.
 ```

### IC上のウォレットの残高を確認するコマンド

`dfx wallet --network=ic balance`

### ウェブサイトをデプロイする方法

`dfx deploy --network ic --with-cycles 1000000000000`

レスポンスの一例
```cmd
Deploying all canisters.
Creating canisters...
Creating canister website...
website canister created on network ic with canister id: vlb3k-cqaaa-aaaag-aawla-cai
Building canisters...
Building frontend...
Installing canisters...
Installing code for canister website, with canister ID vlb3k-cqaaa-aaaag-aawla-cai
Uploading assets to asset canister...
Starting batch.
Staging contents of new and changed assets:
  /index.html 1/1 (449 bytes)
  /assets/index.dfaeff84.css 1/1 (6370 bytes)
  /assets/index.22d017a0.js (gzip) 1/1 (3531 bytes)
  /index.html (gzip) 1/1 (298 bytes)
  /assets/index.dfaeff84.css (gzip) 1/1 (2008 bytes)
  /assets/unchain_logo.3151f11b.png 1/1 (31463 bytes)
  /assets/index.22d017a0.js 1/1 (8886 bytes)
Committing batch.
Deployed canisters.
```

デプロイしたサイトは<a href="https://vlb3k-cqaaa-aaaag-aawla-cai.ic0.app/">こちら</a>からアクセスできます。

### 参考文献
1. [Cycle Faucet](https://anv4y-qiaaa-aaaal-qaqxq-cai.ic0.app/coupon)
2. [Svelte](https://svelte.dev/)
3. [ICP Developer Docs](https://internetcomputer.org/docs/current/developer-docs/build/install-upgrade-remove/)
4. [Vite](https://ja.vitejs.dev/)