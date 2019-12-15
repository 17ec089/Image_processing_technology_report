# 課題３　レポート

標準画像「freeza」を原画像とする．この画像は縦450画像，横800画素によるディジタルカラー画像である．

ORG=imread('freeza.jpg'); % 原画像の入力  
ORG= rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示  
によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-1.png)  
図1 白黒濃淡画像

次に閾値を64とするために以下のようにする。

IMG = ORG > 64; % 輝度値が64以上の画素を1，その他を0に変換  
imagesc(IMG); colormap(gray); colorbar;

閾値64の結果を図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-2.png)    
図2 閾値64

次に閾値を96とするために以下のようにする。

IMG = ORG > 96;  
imagesc(IMG); colormap(gray); colorbar;

閾値96の結果を図3に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-3.png)    
図3 閾値96

次に閾値を128とするために以下のようにする。

IMG = ORG > 128;  
imagesc(IMG); colormap(gray); colorbar;

閾値128の結果を図4に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-4.png)    
図4 閾値128

最後に閾値を192とするために以下のようにする。

IMG = ORG > 192;  
imagesc(IMG); colormap(gray); colorbar;

閾値192の結果を図5に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-5.png)    
図5 閾値192

閾値が高いと画像が濃くなることが確認できた。