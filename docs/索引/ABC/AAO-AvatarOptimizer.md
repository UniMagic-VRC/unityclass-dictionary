---
title: AAO:AvatarOptimizer
tags: [ゲームエンジン, 5回目]
---

アバター軽量化のためのツール群

## なに？

AAO:AvatarOptimizerは、anatawa12氏[^1] によって開発されている、[アバター軽量化](/docs/索引/あ行/アバターの軽量化)を手軽に実行するためのツール群です。

AAOの各ツールを活用することで、以下に示すVRChatのアバターパフォーマンスの各項目を向上できる可能性があります。

- ダウンロードサイズ/非圧縮サイズ(の削減): Trace And Optimize (※BlendShape削減による効果)
- [スキンドメッシュ](/docs/索引/STU/SkinnedMeshRenderer)の数/[基本メッシュ](/docs/索引/MNO/MeshRenderer)の数(の削減): Trace And Optimize / Merge Skinned Mesh
- [ボーン](/docs/索引/ABC/Bone)の数(の削減): Trace And Optimize
- 三角[ポリゴン](/docs/索引/PQR/Polygon)(の削減): Remove Mesh xxx

パフォーマンスランクを上げることは「より多くの人に本来の姿で自身のアバターを見せられる可能性を上げること」にも繋がりますので、可能な限り意識していきたい項目といえるでしょう。

[^1]: https://x.com/anatawa12_vrc
