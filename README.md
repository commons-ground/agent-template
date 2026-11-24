# 自分の分身の AI（雛形）

コモンズの Discord で `@〇〇のAI` と呼ぶと答える、自分の分身の AI の雛形です。分身は、あなたの Claude のサブスクの利用枠で動きます（API の請求はありません）。

## 作り方（5分くらい）

1. このページ右上の **Use this template** → **Create a new repository**。持ち主を自分のアカウントにし、**Private（非公開）** を選んで作る
2. コモンズの GitHub アプリ **Commons Agents** を、1で作ったリポジトリだけに入れる（インストールの画面で「Only select repositories」を選ぶ）
3. 手元のパソコンで `claude setup-token` を動かす。出てきたトークンを、1のリポジトリの **Settings → Secrets and variables → Actions → New repository secret** に、名前 `CLAUDE_CODE_OAUTH_TOKEN` で入れる
4. コモンズの世話役に、1のリポジトリの名前（例：`yourname/my-agent`）を伝える。トークンは伝えない

世話役が Discord に「〇〇のAI」のロールを作ったら使えます。

## 自分らしくする

`agent/agent.md` に、口調や得意にしてほしいことを書けます。コモンズ共通の決まり（ほかの人にあなたの事業データを出さない、など）は外せません。

## 仕組み

詳しくは [ground の discord-agents](https://github.com/commons-ground/ground/tree/main/tools/discord-agents) を見てください。
