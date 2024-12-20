---
tags: [ゲームエンジン, 2回目, 5回目]
---

VRChatで遊ぶ人がアバター改変・ワールド作成をするときに使う基本キット、もしくはUnity上でアバターをアップロードするための画面

## なに？

VRCSDKには2種類の意味があり、一つはいわゆるSDKとして、もう一つは[Unity](/docs/索引/STU/Unity)上でアバターを[アップロード](/docs/索引/あ行/アップロード)するための画面です。

前者の意味だと、VRCSDKとはVRChat向けのSDK(Software Development Kit: ソフトウェア開発キット)のことです。SDKというのは、一般には[ソフトウェア](/docs/索引/さ行/ソフトウェア)の開発に必要な基本コードやサンプルコードなどを**ひとまとまりにしたもの**、とされています。
身近な例では、iPhoneのアプリ開発にはiOS SDKが必要になりますし、同じゲーム開発エンジンであるUnreal EngineからはUnreal Development Kit(UDK)というものがあります。

VCCからUnity[プロジェクト](/docs/索引/PQR/Project)にVRCSDKをインストールすることで、皆さんは改変したアバターのアップロードに必要な前準備や、アップロード自体の実行ができるようになります。

後者の意味だと、下図のようなVRCSDKとはUnity上でアバターをアップロードするための画面のことです。

![VRCSDK](/img_dictionary/VRCSDK_1.png)

この画面は、UnityプロジェクトにVRCSDKをインストールした後であれば画面上部のメニューから「VRChat SDK→Show Control Panel」を押せば表示されます。この画面では、アバターのアップロードや削除といった、VRChatサーバと通信するための機能が備わっています。

## なぜ？

SDKがゲームやアプリケーション本体には付属せず、別途にインストールしないといけない理由はあくまでもSDKが「開発用途において**のみ**必要」だからと言えるでしょう。

たとえばiPhone向けに作られたアプリを使う人たちはみなiOS SDKを準備する必要はありません。Unreal Engineで作られたPCゲームを遊ぶ人たちも同様に、UDKをわざわざインストールする必要はないのです。

SDKはあくまでも開発に必要な基本コードやツールなどをまとめたものに過ぎない、ということです。

VRCSDKも同様に、VRChat社の想定としては「オリジナルアバターの作成(BOOTHから買った商品の改変を含む)」や「オリジナルワールドの作成」は**あくまでも限られた一部のユーザによって**、ある種の追加コンテンツのようなものとして作ってもらっていることに過ぎない、と考えているのかも…しれません。
