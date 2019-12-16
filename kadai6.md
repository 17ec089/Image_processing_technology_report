# 課題６　レポート

標準画像「freeza」を原画像とする．この画像は縦450画像，横800画素によるディジタルカラー画像である．

ORG=imread('freeza.jpg'); % 原画像の入力
ORG = rgb2gray(ORG);
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/6-1.png)  
図1 白黒濃淡画像

次に閾値を128として二値化するために以下のようにする。

IMG = ORG>128; % 128による二値化  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示  

閾値によって二値化した結果を図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/6-2.png)    
図2 二値化画像(閾値)

最後に、ディザ法によって二値化するために以下のようにする。

IMG = dither(ORG); % ディザ法による二値化  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示  

ディザ法によって二値化した結果を図３に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/6-3.png)    
図3 二値化画像(ディザ法)

図２、図３より、ディザ法はざらざらした感じになるが、対象物と背景が区別しやすくなることがわかる。