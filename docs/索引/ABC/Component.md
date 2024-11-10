---
tags: [ゲームエンジン, 2回目, 3回目, 4回目, 5回目]
---

GameObjectの役割を決定させるためのもの

## なに？

コンポーネント(Component: 成分)は[Inspectorウィンドウ](/docs/索引/GHI/Inspectorウィンドウ)から一覧を確認できるもので、ある1つの[GameObject](/docs/索引/GHI/GameObject)に対してどのような機能や役割をもたせるかを決めるためのものです。

全てのGameObjectは必ず[Transform](/docs/索引/STU/Transform)コンポーネントを持ちますが、これは3D空間上における位置・回転・スケール(大きさ)の情報を持たせるための機能です。

Unity標準のコンポーネントとしては、物理演算をさせるためのRigidbody、当たり判定をさせるためのCollider、

[アバター改変](/docs/索引/あ行/アバター改変)においては、基本的にはアバターの[子](/docs/索引/か行/子-親子関係)となるGameObjectには[Armature](/docs/索引/ABC/Armature)を除けば[SkinnedMeshRenderer](/docs/索引/STU/SkinnedMeshRenderer)もしくは[MeshRenderer](/docs/索引/MNO/MeshRenderer)という、[メッシュ](/docs/索引/MNO/Mesh)データを描画するための機能を持たせていることがほとんどです。

![Componentの例](/img_dictionary/Component_1.png)

たとえば上図の場合、[Hierarchyウィンドウ](/docs/索引/GHI/Hierarchyウィンドウ)で選択中のhairというGameObjectに対しては「Transform」コンポーネントおよび「SkinnedMeshRenderer」コンポーネントの2つが付与されています。

ちなみに「HAOLAN_Hair (Material)」というのはあくまでもMaterialの[プロパティ](/docs/索引/PQR/Property)の一覧であって**これ自体はコンポーネントではなく**、便宜上つけられているものです。マテリアルは本来[Projectウィンドウ](/docs/索引/PQR/Projectウィンドウ)から直接マテリアルファイルを選択して編集する必要がありますが、[Renderer](/docs/索引/PQR/Renderer)コンポーネントで参照中のマテリアルを直接編集できると便利だよね、という意図で付けられているものです。
