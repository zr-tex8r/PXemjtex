PXemjtex パッケージバンドル
===========================

LaTeX： アレ

  - `j-ﾅﾝﾄｶ` クラスの代わりに `pxj-ﾅﾝﾄｶ` クラスを使う。
  - `platex`（既定）、`uplatex` のオプションでエンジンを選ぶ。
      - `jlatex` にすると本物の `j-ﾅﾝﾄｶ` に処理を移譲するらしい。
      - `autodetect-engine` もあるらしい（うわぁ）
  - レイアウト設定は（というかクラスファイルのコード全部が）`j-ﾅﾝﾄｶ` クラス
    そのままである。
      - ただし一部を LaTeX 標準クラスに合わせて修正している。
  - カーネルのエミュレーションは一切行っていないので、命令の体系は pLaTeX
    標準と変わらず、JLaTeX の命令は使えない。
  - 和文フォント設定：
      - jis 系の JFM を使う。
      - 和文スケールを JLaTeX の標準と一致させた。
      - シェープ変更に対する明示の代替設定を行った。
      - その他は pLaTeX の標準のままである。
          - 明朝体（`mc`）を太字にするとゴシックになる。
          - 欧文ファミリの変更に和文ファミリは連動しない。
          - JLaTeX 標準では和文ファミリは 1 つしかない。従って pLaTeX で
            和文ファミリを明朝に固定すうと JLaTeX の挙動と一致する。

### 前提環境

  * フォーマット： LaTeX
  * エンジン： pTeX／upTeX
  * DVI ウェア： pTeX 対応のもの

### インストール

  - `*.cls`, `*.clo`, `*.def` → $TEXMF/tex/platex/PXemjtex/

### ライセンス

LPPL 1.3c 以降。

The work is distributed under the LPPL 1.3c or later.
The Work has the status ‘maintained’ and the Current Maintainer is
Takayuki YATO (八登崇之, aka. “ZR”).

更新履歴
--------

  * Version 0.2  〈2016/10/23〉
      - 最初の公開版

--------------------
Takayuki YATO (aka. "ZR")  
http://zrbabbler.sp.land.to/
