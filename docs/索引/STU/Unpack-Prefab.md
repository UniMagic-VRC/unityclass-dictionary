---
title: Unpack Prefab
tags: [ゲームエンジン, 設計思想, 5回目]
---

Prefabを壊して元となるGameObjectの集まりに展開すること

## なに？

Unpack Prefab(Unpack: 取り出す)とは、[Prefab](/docs/索引/PQR/Prefab)を壊して元となる[GameObject](/docs/索引/GHI/GameObject)の集まりとして展開することを指します。

Unpackという行為は一方的なものであり、一度展開されたデータは元のPrefabに戻すことは二度とできません。

Prefabには様々なメリットがあるため、可能な限りはUnpack Prefabをしないことが望ましいです。従来の[衣装改変](/docs/索引/あ行/衣装改変)においてはUnpack Prefabをすることがある種の通過儀礼でしたが、現在ではPrefabのまま扱える方法として[Modular Avatar](/docs/索引/MNO/ModularAvatar)などの[非破壊ツール](/docs/索引/は行/破壊的-非破壊的)が普及しています。可能な限りそちらを使うのが良いでしょう。
