# GTA5 Police Bodyguard

GTA V Steam版のシングルプレイ用 ScriptHookVDotNet v3 MODです。

`F5`を押すと、既存の巡査風NPCを主人公の近くにボディガードとして召喚します。ボディガードは主人公についていき、主人公やボディガードが攻撃された時にピストルで応戦します。

## 必要なもの

- GTA V Steam版
- Script Hook V
- ScriptHookVDotNet v3
- .NET Framework 4.8 Developer Pack
- Visual Studio または Visual Studio Build Tools

## 導入方法

1. Script Hook Vを導入します。
   - `dinput8.dll`
   - `ScriptHookV.dll`
2. ScriptHookVDotNet v3を導入します。
   - `ScriptHookVDotNet.asi`
   - `ScriptHookVDotNet3.dll`
3. GTA Vのインストールフォルダーに`scripts`フォルダーを作成します。
4. `Gta5PoliceBodyguard.dll`を`scripts`フォルダーへコピーします。
5. GTA Vをシングルプレイで起動します。
6. `F5`を押すと警察官ボディガードが出現します。

## ビルド方法

ソースコードからビルドする場合は、GTA Vのインストールフォルダー直下に`ScriptHookVDotNet3.dll`がある状態で、次を実行します。

```powershell
.\build.ps1
```

または:

```powershell
MSBuild.exe Gta5PoliceBodyguard.csproj /p:Configuration=Release
```

出力:

```text
bin\Release\Gta5PoliceBodyguard.dll
```

## 操作

- `F5`: 警察官ボディガードを1人召喚します。

もう一度`F5`を押すと、古いボディガードを削除して新しいボディガードを召喚します。

## 注意

オンラインでは使用しないでください。このMODはシングルプレイ専用です。
