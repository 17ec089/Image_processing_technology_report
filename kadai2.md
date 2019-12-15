# 課題２レポート

標準画像「freeza」を原画像とする．この画像は縦450画像，横800画素によるディジタルカラー画像である．

ORG=imread('freeza.jpg'); % 原画像の入力  
ORG = rgb2gray(ORG); colormap(gray); colorbar;  
imagesc(ORG); axis image; % 画像の表示

によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-1.png)  
図1 白黒濃淡画像

次に原画像を2階調にするために以下のようにする.

IMG = ORG>128;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

2階調の結果を図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-2.png)    
図2 2階調画像

次に原画像を4階調にするために以下のようにする.

IMG0 = ORG>64;  
IMG1 = ORG>128;  
IMG2 = ORG>192;  
IMG = IMG0 + IMG1 + IMG2;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

4階調の結果を図3に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-3.png)    
図3 4階調画像

最後に原画像を8階調にするために以下のようにする.

IMG3 = ORG>32;  
IMG4 = ORG>64;  
IMG5 = ORG>96;  
IMG6 = ORG>128;  
IMG7 = ORG>160;  
IMG8 = ORG>192;  
IMG9 = ORG>224;  
IMG = IMG3 + IMG4 + IMG5 + IMG6 + IMG7 + IMG8 + IMG9;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

8階調の結果を図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-4.png)    
図4 8階調画像

以上より、階調を多くすることでなめらかなグラデーションで表現できる.