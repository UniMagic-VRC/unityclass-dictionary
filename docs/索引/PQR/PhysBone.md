---
tags: [ゲームエンジン, 4回目]
---

主にVRC向けに作られた、揺れものを表現するための機能

## なに？

PhysBone(PBと略されることもある)とは、VRChat社が開発・提供している、揺れものを表現するための[コンポーネント](/docs/索引/ABC/Component)です。

揺れものとは、「髪の毛」や「スカートなどの布」など、アバターの動きに合わせてリアルタイム演算によってひらひらと動くもの自身を指します。

歴史的経緯としては、従来のVRChatにおいては揺れものの表現としては専らDynamicBone(DBと略されることもある)という有料Unityアセットツール[^1] が使われていました。当時の事情については筆者は分かりませんが、おそらくアバターや衣装にDynamicBoneが使われていて、改変ユーザが揺れものを表現したい場合はアバターや衣装の購入費用**とは別にDynamicBoneアセットも買わないといけない**、という状況だったと思われます。

2022年3月頃、VRChat社からリリースされたPhysBoneによりこの状況は劇的に改善されたようです。揺れものを使いたいユーザは別途DynamicBoneアセットを買う必要はなくなり、よりVRCに最適化された揺れものの表現が可能になりました。

なお、PhysBoneには名前こそ「Bone(ボーン)」が含まれてますが、いわゆる3DCGにおける[ボーン](/docs/索引/ABC/Bone)の概念とは異なります。
Boneは「[スキニング](/docs/索引/STU/Skinning)された[メッシュ](/docs/索引/MNO/Mesh)を動かすためのもの」ですが、PhysBoneはBone(および**あらゆる**GameObject)に揺れものやバネなどの物理演算を表現するための機能です。

PhysBoneにはボーンのようなリグやスキニングに関する設定情報は一切持っておらず、**あくまでも特定のGameObjectの集まりを揺れもののように動きをシミュレートさせるためのものに過ぎない**のです。

[^1]: https://assetstore.unity.com/packages/tools/animation/dynamic-bone-16743
