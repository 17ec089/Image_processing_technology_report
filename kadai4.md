# 課題４　レポート

標準画像「freeza」を原画像とする．この画像は縦450画像，横800画素によるディジタルカラー画像である．

ORG=imread('freeza.jpg'); % 原画像の入力  
ORG= rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換  
imagesc(ORG); colormap(gray); colorbar;

によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/4-1.png)  
図1 白黒濃淡画像

次にヒストグラムを表示するために以下のようにする。

imhist(ORG); % ヒストグラムの表示  

ヒストグラムを図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/4-2.png)    
図2 ヒストグラム

図2より、濃度レベルが210および240付近の画素が多いことがわかる。