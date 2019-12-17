# 課題８　レポート

標準画像「freeza」を原画像とする．この画像は縦450画像，横800画素によるディジタルカラー画像である．

ORG = imread('freeza.jpg'); % 画像の読み込み  
ORG = rgb2gray(ORG); % 白黒濃淡画像に変換  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示  

によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/8-1.png)  
図1 白黒濃淡画像

次に閾値を128として二値化するために以下のようにする。

IMG = ORG > 128; % 閾値128で二値化
imagesc(IMG); colormap(gray); colorbar; % 画像の表示  

閾値によって二値化した結果を図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/8-2.png)    
図2 二値化画像(閾値)

最後に、二値化された画像の連結成分にラベルを付けるために以下のようにする。

IMG = bwlabeln(IMG);  
imagesc(IMG); colormap(jet); colorbar; % 画像の表示  

ラベリングした結果を図３に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/8-3.png)    
図3 ラベリング

図３より、顔や背景に着目するとラベリングされているのがわかりやすい。