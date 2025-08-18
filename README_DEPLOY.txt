RCCM 問題4-2（JSON固定パス版）デプロイ手順
======================================

公開URL: https://cat-hiro.github.io/rccm-problem2/

1) GitHub → rccm-problem2 リポの *公開フォルダ*（Pages の設定で "Branch: main / Folder: root" ならリポ直下、"docs" なら docs/）に、
   - index.html
   - rccm_data.json
   - .nojekyll
   の3つをそのまま置いて Commit（ドラッグ&ドロップでOK）

2) 数十秒後、 https://cat-hiro.github.io/rccm-problem2/ を開く。
   読み込みが止まるときは、 https://cat-hiro.github.io/rccm-problem2/rccm_data.json を直接開いて
   中身が表示されるか確認（404 なら配置パスの誤り or 未反映）。

メモ:
- この index.html は /rccm-problem2/rccm_data.json を **絶対パス**で取得します。
  そのため、公開されるフォルダ（root でも docs でも）に rccm_data.json を置けばOKです。
- うまくいかない場合は、Pages の "Build and deployment" を一度 None にして保存 → 再度 main/root（or docs）に戻すと再デプロイされます。