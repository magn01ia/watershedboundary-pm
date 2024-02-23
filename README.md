# watershedboundary-pm
流域・非集水域のベクトルタイル(PMTiles)  
unvt/nanban(国連ベクトルタイルツールキット)でTippecanoeを使用して作成。  

## デモ    

## 元データ  
国土数値情報(国土交通省)にて公開されている各データを加工して作成。  
### 流域界・非集水域  
- 全国版(S52)  
  https://nlftp.mlit.go.jp/ksj/gmlold/datalist/gmlold_KsjTmplt-W12.html  
  GDALでgeojsonに変換  
### 河川ラインデータ  
- 47都道府県分(第3.1版)    
  https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-A29-v2_1.html  
  都道府県別のデータになっているので結合してgeojsonに変換。  

## 変換  
- tippecanoe -pf -pk -Z7 -z10
