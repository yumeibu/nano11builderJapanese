# Nano11Builder

A script to make your OWN Nano11 image.

This is a script to automate the build of an Nano 11 iso.
The main goal of this is to use only Microsoft utilities like DISM, and nothing external. The only executable included is oscdimg.exe, which is provided in the Windows ADK and it is used to create bootable ISO images. Also included is an unattended answer file, which is used to bypass the MS account on OOBE.

To download the post-setup, you will need git If you don't want to install it, you can skip the step

Instructions:

1. Download an Windows 11 ISO.
2. Mount the downloaded ISO image using Windows Explorer.
3. Run the nano11builder.bat file.
4. Select the drive letter where the image is mounted (only the letter, no colon (:))
5. Select the SKU that you want the image to be based.
6. Sit back and relax :)
7. When the image is completed, you will see it in the folder where the script was extracted, with the name nano11.iso

What is removed:

Everything Nano11 Removes

Known issues:

1. Only ja-jp (Japanese) x64 is supported. Use this script only with a Japanese-language Windows 11 ISO. If you need another language, replace every instance of ja-jp with the language needed (like en-us, ro-RO and so on), and every x64 instance with arm64.

And that's pretty much it for now!

独自のNano11イメージを作成するためのスクリプトです。

これは、Nano 11のISO作成（ビルド）を自動化するスクリプトです。
主な目的は、外部ツールを一切使用せず、DISMなどのMicrosoft製ユーティリティのみを利用することです。唯一含まれている実行ファイルは`oscdimg.exe`（Windows ADKに付属し、ブート可能なISOイメージの作成に使用されるもの）のみです。また、OOBE（初期セットアップ）時にMicrosoftアカウントの入力を回避するための無人セットアップ用応答ファイルも含まれています。

Post-setup（セットアップ後の処理）ファイルをダウンロードするにはgitが必要です。インストールしたくない場合は、その手順をスキップできます。

手順:

1. Windows 11のISOをダウンロードします。
2. ダウンロードしたISOイメージをエクスプローラーでマウントします。
3. `nano11builder.bat`ファイルを実行します。
4. イメージがマウントされているドライブ文字を選択します（文字のみ入力し、コロン「:」は含めないでください）。
5. ベースとするイメージのSKU（エディション）を選択します。
6. あとは完了するのを待つだけです :)
7. イメージの作成が完了すると、スクリプトを展開したフォルダに`nano11.iso`という名前で保存されます。

削除されるもの:

Nano11で削除されるすべての要素

既知の問題:

1. ja-jp（日本語）のx64版のみサポートされています。日本語版のWindows 11 ISOでのみこのスクリプトを使用してください。他の言語が必要な場合は、`ja-jp`を必要な言語（`en-us`、`ro-RO`など）に、`x64`を`arm64`にすべて置き換えてください。

現時点では以上です！
