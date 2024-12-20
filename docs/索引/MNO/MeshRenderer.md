---
tags: [ゲームエンジン, 3回目, 4回目, 5回目]
---

主に変形しないメッシュを扱うためのRendererコンポーネント

## なに？

MeshRendererとは[Renderer](/docs/索引/PQR/Renderer) [コンポーネント](/docs/索引/ABC/Component)の1つであり、主に変形しない[メッシュ](/docs/索引/MNO/Mesh)を取り扱うためのものです。

「変形しない」というのは、主に[ブレンドシェイプ](/docs/索引/ABC/BlendShape)を持たない、ウェイト情報([ボーン](/docs/索引/ABC/Bone)の移動に伴うメッシュの変形情報のこと)を持たないことが条件となります。
これらの条件を満たせない場合は[SkinnedMeshRenderer](/docs/索引/STU/SkinnedMeshRenderer)コンポーネントを使う必要があります。

MeshRendererコンポーネントで描画されるオブジェクトの例として、シンプルなメガネや帽子などが挙げられます。

ですが昨今のBOOTH商品の傾向としては「どれだけシンプルなオブジェクトであったとしても、あらゆるアバターへの改変がしやすいように幾つかのシェイプキーを入れておく」ことが標準となっているように考えられます。そのため、BOOTHで販売されている商品のうちMeshRendererで作られているオブジェクトは極僅かと言えるでしょう。

SkinnedMeshRendererコンポーネントのほうがより多機能と言えますが、その分負荷も高いためGameObjectの描画は可能な限りMeshRendererコンポーネントを使うのが望ましいとされています。
