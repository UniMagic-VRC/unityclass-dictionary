---
tags: [ゲームエンジン, 2回目]
---

ゲームを、カメラ越しで見た際の見え方を確認するための画面

## なに？

Gameウィンドウとは一般に、開発中のゲームをカメラ越しで見た際の見え方を確認するための画面です。

普段我々が操作する[Sceneウィンドウ](/docs/索引/STU/Scene-Window)はカメラの位置を自由に変えることが出来ますが、一般に実際のゲームとは違う視点で見ていることが多いです。たとえば三人称視点のゲームなら「主人公の背中を映すような位置」にカメラがあって、そこから見える景色が画面に映っているはずです。VRChatのような一人称視点のゲームなら「主人公の目線に相当する位置」から見える景色が映っているはずです。

実際、[VRCSDK](/docs/索引/VWX/VRCSDK)のワールド制作用[Unity](/docs/索引/STU/Unity) [プロジェクト](/docs/索引/PQR/Project)であればこのGameウィンドウを通してワールド内を一人称視点で見たり移動したりすることが出来ます。しかしながら、[アバター改変](/docs/索引/あ行/アバター改変)においてはそのような機能も用意されておらず、Gameウィンドウを使う機会はほとんど無いと言っていいかもしれません。

ちなみに、[再生モード](/docs/索引/さ行/再生モード)に入るたびにSceneウィンドウが隠されてしまうこのGameウィンドウですが、再生モード実行時にGameウィンドウを前面に出さない設定もあります。Gameウィンドウを表示→上部のツールバーの「Play Focused」をクリック→出てきた一覧から一番下の「Play Unfocused」を選択で設定可能です(下図参照)。

![Focused設定](/img_dictionary/Gameウィンドウ_1.png)
