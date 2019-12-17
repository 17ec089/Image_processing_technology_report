# 課題７　レポート

標準画像「poke」を原画像とする．この画像は縦445画像，横600画素によるディジタルカラー画像である．

ORG = imread('poke.jpg'); % 画像の読み込み
ORG = rgb2gray(ORG); % 白黒濃淡画像に変換
imagesc(ORG); colormap(gray); colorbar; % 画像の表示 

によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-1.png)  
図1 白黒濃淡画像

図１のヒストグラムを表示する。

imhist(ORG); % ヒストグラムの表示  

ヒストグラムを図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-2.png)    
図2 ヒストグラム

次に、ダイナミックレンジを０から２５５にするために以下のようにした。

ORG = double(ORG);  
mn = min(ORG(:)); % 濃度値の最小値を算出  
mx = max(ORG(:)); % 濃度値の最大値を算出  
ORG = (ORG-mn)/(mx-mn)*255;  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示  

ダイナミックレンジ拡大後の画像を図３に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-3.png)    
図3 ダイナミックレンジ拡大後の画像

また、画像を８ビット符号なし整数としたときのヒストグラムを表示するために以下のようにした。

ORG = uint8(ORG); % この行について考察せよ  
imhist(ORG); % 濃度ヒストグラムを生成、表示  

これは濃度の範囲を広くする操作である。図４にヒストグラムを示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-4.png)    
図4 ８ビット符号なし整数のヒストグラム

図２、図４より、ダイナミックレンジ拡大後の方が濃度の範囲が広くなっていることがわかる。