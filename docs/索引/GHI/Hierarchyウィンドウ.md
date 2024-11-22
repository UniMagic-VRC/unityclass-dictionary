---
tags: [ゲームエンジン, 2回目, 3回目, 4回目, 5回目]
---

シーンで扱うすべてのGameObject、およびその親子関係がわかる場所

## なに？

ヒエラルキー(Hierarchy: 階層)ウィンドウとは[Unity](/docs/索引/STU/Unity)の画面の一部であり、[Sceneファイル](/docs/索引/STU/Scene-File)で扱うすべての[GameObject](/docs/索引/GHI/GameObject)およびその[親子関係](/docs/索引/あ行/親子関係)がわかる場所です。

![Hierarchyウィンドウ](/img_dictionary/Hierarchyウィンドウ_1.png)

たとえば上図のHierarchyウィンドウでは、「B03」という名前のSceneファイルの中身として「Main Camera」、「Directional Light」、「Gesture Manager」、「Phys_Haolan」といったGameObjectが同じ階層に並んでいることが分かり、「Phys_Haolan」にはさらに「Armature」、「Body」、「Body2」といったGameObjectが子のオブジェクトとして持っていることが分かります。

「階層構造」自体はUnity独自の考え方とは限らず、PhotoshopやIllustratorのようなデザインツール等でも度々見かけられます。たとえばPSD形式の[テクスチャ](/docs/索引/STU/Texture)ファイルをPhotoshop等で開いた場合、塗り方がパーツごとに分かれており、それらは親子関係や上下関係をもつ「レイヤー情報」としてまとめられています。

ただし注意点として、デザインツールの階層構造においては「上に置かれたレイヤーは必ず下のレイヤーを上書きするように、前面に描画される」という法則がありますがUnityの階層構造においては上下関係は描画には関係せず、描画順を決定する要素が別途用意されています(ZWrite、レンダーキューなど。興味がある方は調べてみてください！)。
