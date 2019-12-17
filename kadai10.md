# 課題１０　レポート

標準画像「freeza」を原画像とする．この画像は縦450画像，横800画素によるディジタルカラー画像である．

ORG = imread('freeza.jpg'); % 原画像の入力  
ORG = rgb2gray(ORG); %カラーからグレイへの変換  
imagesc(ORG); colormap('gray'); colorbar;% 画像表示  

によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-1.png)  
図1 白黒濃淡画像

次にプレウィット法によるエッジ抽出をするために以下のようにする。

IMG = edge(ORG,'prewitt'); % エッジ抽出（プレウィット法）  
imagesc(IMG); colormap('gray'); colorbar;% 画像表示  

結果を図２に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-2.png)    
図2 プレウィット法

次にソベル法によるエッジ抽出をするために以下のようにする。

IMG = edge(ORG,'sobel'); % エッジ抽出（ソベル法）  
imagesc(IMG); colormap('gray'); colorbar;% 画像表示  

結果を図３に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-3.png)    
図3 ソベル法

最後にキャニー法によるエッジ抽出をするために以下のようにする。

IMG = edge(ORG,'canny'); % エッジ抽出（キャニー法）  
imagesc(IMG); colormap('gray'); colorbar;% 画像表示  

結果を図４に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-4.png)    
図4 キャニー法

図２、図３、図４より、キャニー法はプレウィット法とソベル法に比べ、多くのエッジを抽出していることが確認できた。