# smile_work02
創造社デザイン専門学校　スマイル工房 2020 冬季

## JavaScript スライダー入門
### jQueryとは
### slickプラグイン
### JSON形式
### 設置の仕方

## HTMLフォーム研究(PHP)
### POSTとGET
### HTMLのフォームの作り方
### HTMLフォームの書き方
### PHPとの連携

## LIGHTBOX 入門
### jQueryとは
### LIGHTBOX プラグイン
https://lokeshdhakar.com/projects/lightbox2/
### CDN
```
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
```
### 設置方法
### JSON

## Google Map
### 基本
Googleで地図検索をし、共有>地図を埋め込むでHTMLコードを取得

### ルートを含むMapの共有
GoogleMap上でルートを検索
ハンバーガーメニューから「地図を共有又は埋め込む」を選択


### iframeとは？
iframe(アイフレーム)タグはHTMLの中に別のHTMLファイルを組み込むタグ。
HTMLが入れ子(ネスト)になっていると考える事も出来ます。
|  属性  |  意味  |
| ---- | ---- |
|  SRC属性  |  表示させるファイルを指定  |
|  WIDTH属性  |  iframeの幅を指定  |
|  height属性  |  iframeの高さを指定  |

### Google Mapのiframeタグ
```
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3280.6707299802883!2d135.49016731523187!3d34.6882588804377!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6000e6896ff95165%3A0xf53f3dc9231f03bf!2z5Ym16YCg56S-44OH44K244Kk44Oz5bCC6ZaA5a2m5qCh!5e0!3m2!1sja!2sjp!4v1610150629282!5m2!1sja!2sjp" width="600" 
height="450" 
frameborder="0" 
style="border:0;" 
allowfullscreen="" 
aria-hidden="false" 
tabindex="0">
</iframe>
```
### iframeタグに含まれるオプション
上記基本属性に加えて
|  属性  |  意味  |
| ---- | ---- |
|  frameborder属性  |  フレームの枠線の表示を設定するための属性　0で非表示、1で表示(非推奨)　現在の推奨は　CSS の border プロパティ  |
|  style属性  |  iframeの幅を指定  |
|  allowfullscreen属性  | trueで全画面モード対応(非推奨) 現在の推奨はallow="fullscreen" |
|  aria-hidden属性  |  非表示の属性  |
|  tabindex属性  |  TABキーで進む順番を指定  |

## Youtube
### 基本
Youtubeで埋め込みたい動画を探し、共有から埋め込むを選択、埋め込みタグが表示されるのでコピーをクリック。
HTMLにiframeタグを埋め込む

### Youtube画面で選べるオプション
|  属性  |  意味  |
| ---- | ---- |
|  開始位置  |  再生を始めるフレームを分秒単位で指定(0:00)  |
|  プライバシー強化モードを有効  |  ユーザーが動画を再生するまで、ユーザーの情報がYouTubeに保存されないようにするための設定  |

### Youtubeのiframeタグ
```
<iframe 
width="560" 
height="315" 
src="https://www.youtube.com/embed/tlGLlUBkczM" 
frameborder="0" 
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen>
</iframe>
```

### iframeタグに含まれるオプション
|  属性  |  意味  |
| ---- | ---- |
|  SRC属性  |  表示させるファイルを指定  |
|  WIDTH属性  |  iframeの幅を指定  |
|  height属性  |  iframeの高さを指定  |
|  src属性  |  動画ファイルのURL  |
|  frameborder属性  |  フレームの枠線の表示を設定するための属性　0で非表示、1で表示(非推奨)　現在の推奨は　CSS の border プロパティ  |
|  allow属性  |  埋め込まれた文書が利用することができるユーザーのデバイスやブラウザの機能、APIの有効化と無効化を指定する属性  |
|  allowfullscreen属性  |  trueで全画面モード対応(非推奨) 現在の推奨はallow="fullscreen"  |

### Youtubeのカスタマイズ
src属性にリクエストクエリでオプションを追記する

#### 自動再生
https://www.youtube.com/embed/<video_id>?autoplay=1&mute=1

#### ループ再生
https://www.youtube.com/embed/<video_id>?loop=1&playlist=<video_id>

#### 自動再生とループ
https://www.youtube.com/embed/<video_id>?autoplay=1&mute=1&playsinline=1&loop=1&playlist=<video_id>

### コントロールの非表示
https://www.youtube.com/embed/<video_id>?controls=0

### 背景として使用
https://www.youtube.com/embed/<video_id>?autoplay=1&mute=1&playsinline=1&loop=1&playlist=<video_id>&controls=0&disablekb=1
