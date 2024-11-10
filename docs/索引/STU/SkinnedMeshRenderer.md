---
tags: [ゲームエンジン, 3回目, 4回目, 5回目]
---

主に変形するメッシュを扱うためのRendererコンポーネント

## なに？

SkinnedMeshRenderer(Skinned: [スキニング](/docs/索引/STU/Skinning)された)とは[Renderer](/docs/索引/PQR/Renderer) [コンポーネント](/docs/索引/ABC/Component)の1つであり、主に変形情報を持つ[メッシュ](/docs/索引/MNO/Mesh)を取り扱うためのものです。

変形情報とは、主に[ブレンドシェイプ](/docs/索引/ABC/BlendShape)やウェイト情報([ボーン](/docs/索引/ABC/Bone)の移動に伴うメッシュの変形情報のこと)のことを指します。

特に複数のボーンに対するウェイト情報を持つ衣装の場合、衣装自体が「[Armature](/docs/索引/ABC/Armature)」オブジェクトを持ちます。このため、[衣装改変](/docs/索引/あ行/衣装改変)においてはアバター側のボーンへ[追従させる](/docs/索引/た行/追従する)ために少し複雑な手順を取る必要が出てきます。
