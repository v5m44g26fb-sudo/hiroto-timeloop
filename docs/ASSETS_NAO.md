# 男装版なお 画像資産メモ（ASSETS_NAO.md）

調査日: 2026-11-09。主人公なお（男装練習生）の画像について、既存資産・流用可否・新規生成・不足分を整理する。

## 0. 同一性の基準（リファレンス）

- **現行の顔の基準＝ face2（2026-11-09 本人承認・正式決定）**: `assets/nao/2019/profile-face2-close.jpg`（名簿用アップ）／ `assets/nao/2019/profile-face2-full.jpg`（全身版）。制服＋青チェックの通常ネクタイ＋ガッツポーズは従来どおり
  - 特徴：鼻翼が狭く鼻筋が細い顔立ち（本人が提示した参照写真2枚に寄せたもの）。目の下のほくろ・白い肌は維持
  - 2021・2023のプロフィールと、ナオが写る場面カット類は全てこの face2 を同一性基準として生成し直す（旧フェイスとの混在禁止）
- **旧基準は使用禁止（2026-11-09 差し替え）**: 下記の旧基準ビジュアル（438CA…）から生成した旧フェイスの画像は全て表示から外す。対象：2019リボン版（`profile.jpg` / `profile-close.jpg`）、2019ネクタイ版（`profile-tie.jpg` / `profile-close2.jpg`）、および旧フェイスで生成された 2021・2023 プロフィールと全場面カット
- （旧）基準ビジュアル: `~/workspace/user/files/438CA2B6-C46E-4F5A-B3F6-16D1405B68DB-photo-82968D00-9B6A-4F0F-A184-C9ACBFE37FCC.jpg`（1122×1402、紺セーターで頭に手を添えた男版ビジュアル）
  - 本人の評価は「2026ビジュすぎる」。face2 の土台になった参照だが、顔の基準としては上記の face2 に置き換え済み

## 1. 既存の男版なお画像と流用可否

| ファイル | 内容 | 流用可否 |
|---|---|---|
| `~/workspace/lastart-manne/assets/av-nao.jpg` ＝ `nao-profile.jpg`（同一ファイル、1122×1402）／保管コピー: `~/workspace/profile-inbox/nao-profile-designated-20261103.jpg`、`nao-eldest-face-20261104.jpg`（同一ハッシュ） | マンネ編で本人指定の作中ビジュアル（男装設定） | **確定待ち（流用しない前提）**。`lastart-manne/IMAGE_SOURCES.md` に「本作（マンネ編）専用」と明記された指定画像のため、本作での流用には本人の再指定が必要。新規生成3点が確定すれば不要になる見込み |
| `~/workspace/lastart-manne/assets/nao-age7.jpg` / `nao-age10.jpg` / `nao-age12.jpg` / `nao-age15.jpg`（各912×1136） | マンネ編の年齢別ビジュアル（7/10/12/15歳） | **使用不可**。IMAGE_SOURCES.md に「マンネ編限定使用、他作品への流用不可」と明記。そもそも本作の年齢設定（17歳〜）とも合わない |
| `~/workspace/lastart-wish-game/assets/av-nao.jpg`（上記と別ハッシュ） | LASTART編側のなおアバター | **使用不可扱い**。別世界（LASTART編）の指定画像であり混用しない |
| 旧版（紺セーター系、`profile-inbox/*-superseded.jpg`） | マンネ編の差し替え前旧版 | **使用禁止**（マンネ編側で使用禁止が明記済み） |

## 2. 新規生成済み・確認待ち（2026-11-09 追加）

本人が確認中。**確定待ちリストから「生成済み・確認待ち」へ移行**した3点。いずれも1296×1616・webp。確定したら `assets/` へjpg変換して取り込む（変換は確定後）。

| 時代 | ファイル | 仕様 |
|---|---|---|
| 2019年版（日プ用）**現行の正＝ face2（2026-11-09 本人承認）** | `assets/nao/2019/profile-face2-full.jpg`（全身）／ `assets/nao/2019/profile-face2-close.jpg`（名簿用アップ） | 17歳・日プ制服（グレーブレザー＋白パイピング＋青チェックの**通常ネクタイ**＋名札）・立ちガッツポーズ・新フェイス（鼻翼が狭く鼻筋が細い）・ほくろと白い肌を維持。旧フェイスのリボン版・ネクタイ版は表示から撤去済み・使用禁止 |
| 2021年版（創造営用） | `~/workspace/imagine_media/media-generation-nao-male-2021-0-7a3d7c55-bd9c-41c9-a8de-b3df560bc841.webp` | 19歳・訓練生ジャケット正面プロフィール |
| 2023年版（ボイプラ用） | `~/workspace/imagine_media/media-generation-nao-male-2023-0-646fc911-55a8-45dd-a5d1-8e4b0f1fa204.webp` | 21歳・明るい茶髪レイヤー・韓国風練習生プロフィール |

- 用途（想定）: 各時代のアバター、練習生名簿のプロフィール、番組公式プロフィール画面
- 未確定事項: 本人のOKが出るまでゲームには組み込まない。差し替え生成が来たら本ファイルのパスを更新する
- **2026-11-09 face2 全面差し替え（進行中）**: 2019は face2 へ差し替え完了。2021・2023のプロフィール（`2021/profile.jpg`、`2023/profile.jpg`、`2023/profile-close.jpg`）と、ナオが写る場面カット類（2019: dorm / practice / ranking-close / selfie / stage / stage2、2021: daily / practice / stage / study、2023: daily / fancam-close / fancam2 / practice / stage）は face2 基準で再生成する。再生成前の旧フェイス版は `hidden_files/nao-oldface-backup/` に保管。顔の写らないカット（`common/room.jpg`、`common/livehouse.jpg`、後ろ姿の `common/audience-back.jpg`）は差し替え対象外

## 3. まだ不足している画像リスト

プロフィール正面は §2 で生成済みになったため、残りは場面別カット。

### 2019 日プ編（最優先）→ 生成済み（2026-11-09、目視確認で同一性・肌色とも合格、作り直し0回）
1. ~~練習着での全身／レベル分け評価カット~~ → `assets/nao/2019/practice.jpg`
2. ~~宿舎・日常カット~~ → `assets/nao/2019/dorm.jpg`
3. ~~ステージ衣装カット~~ → `assets/nao/2019/stage.jpg`
4. ~~順位発表・脱落の夜に使う近接カット~~ → `assets/nao/2019/ranking-close.jpg`
- 生成マスター（webp）は `hidden_files/nao-masters/2019/` に保管（リポジトリには jpg のみ）

### 2021 創造営編 → 生成済み（2026-11-09、目視確認合格）
5. ~~練習着／合宿日常カット~~ → `assets/nao/2021/practice.jpg` / `assets/nao/2021/daily.jpg`（＋プロフィール `assets/nao/2021/profile.jpg`）
6. ~~ステージ衣装カット~~ → `assets/nao/2021/stage.jpg`

### 2023 ボイプラ編 → 生成済み（2026-11-09、目視確認合格。ステージは親側でも目視し同一性・肌色を確認）
7. ~~練習着／日常カット~~ → `assets/nao/2023/practice.jpg` / `assets/nao/2023/daily.jpg`（＋プロフィール `assets/nao/2023/profile.jpg`）
8. ~~ステージ衣装カット~~ → `assets/nao/2023/stage.jpg` ＋ チッケム風近接 `assets/nao/2023/fancam-close.jpg`

### 現在編（2026）
9. 現在の彼女（女性）としての表示素材 — **未確定**。なお本人の写真は作品ごとに許可範囲が決まっている素材であり、本作での使用許可はまだない。前作までの原則（アバターは初期アイコン）に従い、許可が出るまで空欄で設計する

### 共通・演出用 → 生成済み（2026-11-09）
10. ~~0周目差分演出用カット（客席の後ろ姿）~~ → `assets/nao/common/audience-back.jpg`
   - 初回生成はステージ看板に無関係な英語タイトル（別番組の世界観）が写り込んだため**不採用**とし、看板なし・アイドルサバイバルの収録スタジオ風で再生成した第2版を採用（親側で目視確認済み）

## 4. 大翔・他キャストの時代別写真（既存資産あり、新規不要）

| 時代 | 置き場所 | 内容 |
|---|---|---|
| 2019 日プ | `~/workspace/produce-uragawa/assets/s1/`（184ファイル） | 大翔 `hiroto.jpg` / `hiroto-big.jpg` ほかS1キャスト |
| 2021 創造営 | `~/workspace/chuang-uragawa/assets/cast90/`（90名） | 大翔 `hiroto.jpg` ほか全キャスト（出典は各MANIFEST.md確認済み） |
| 2023 ボイプラ | `~/workspace/boysplanet-uragawa/assets/cast/`（93名分＋α） | 大翔 `hiroto.jpg` ほか。出典: Mnet公式プロフィール（MANIFEST.mdに照合記録あり） |

- Tinder版 assets にもある時代写真（`bp-profile.jpg`、`china2021.jpg`）は補助素材として使えるが、正は上記の各サバイバル編リポジトリ側とする

- 2019年版の初回生成（白T・座りポーズ）は本人が「別人すぎる、顔が茶色い」と却下したため**破棄**（ファイルは残置するが使用禁止）。2019の正は制服版のみ。
