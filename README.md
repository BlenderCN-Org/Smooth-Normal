# Smooth-Normal
This is the Blender addon that edit normal.  
これは法線を編集する Blender のアドオンです．

Location is Normal in tool shelf in Edit mode. "set face normal" is in face select mode only.   
ボタンはツールシェルフの Normal にあります．
表示されるのはエディットモードの時のみです．
set face normal はフェース選択モードのときのみ表示されます．

If you use A key or circle select or border select, you can not edit the normals. In that situation deselect one element and select the element again. By that operation, you can edit all the normals of the elements. Since BMesh's select_history is not able to get by multi select tool, that operation needed.  
A キーや円選択・矩形選択で選択すると法線を編集できません。その時は Shift を押しながら要素（頂点や面）をひとつ選択解除してから、その要素を再選択すると選択したすべての要素の法線を編集できます。このような動作になっているのは複数の要素を同時に選択すると BMesh の select_history が取得できないからです。

When smooth result is ugly, run revert with all selected vertices. It may run correctly.  
スムースがうまくいかない時は，すべての頂点を選択して revert を実行するとうまくいくことがあります．

Mask Color can change in Blender User Preferences > System > Custom Weight Paint Range.  
頂点色が見づらいときは Blender ユーザー設定 > システム > ウェイトペイントの色の設定で色を変更できます．
