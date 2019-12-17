# 課題９　レポート

標準画像「freeza」を原画像とする．この画像は縦450画像，横800画素によるディジタルカラー画像である．

ORG = imread('freeza.jpg'); % 画像の読み込み  
ORG = rgb2gray(ORG); % 白黒濃淡画像に変換  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示  

によって，原画像を読み込み，白黒濃淡化にした結果を図１に示す．

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-1.png)  
図1 白黒濃淡画像

次にノイズを添付するために以下のようにする。

ORG = imnoise(ORG,'salt & pepper',0.02); % ノイズ添付  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示  

ノイズ添付した結果を図2に示す.

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-2.png)    
図2 ノイズ添付

図２を平滑化フィルタで雑音除去するために以下のようにする。

IMG = filter2(fspecial('average',3),ORG); % 平滑化フィルタで雑音除去  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示  

平滑化フィルタの結果を図３に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-3.png)    
図3 平滑化フィルタ

図２をメディアンフィルタで雑音除去するために以下のようにする。

IMG = medfilt2(ORG,[3 3]); % メディアンフィルタで雑音除去  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示  

メディアンフィルタの結果を図４に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-4.png)    
図4 メディアンフィルタ

また、以下のようなフィルタを設計した。

f=[0,-1,0;-1,5,-1;0,-1,0]; % フィルタの設計  
IMG = filter2(f,IMG,'same'); % フィルタの適用  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示  

結果を図５に示す。

![原画像](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-5.png)    
図5 フィルタ設計

図３、図４より、平滑化フィルタはノイズが残っているうえにぼやけてしまったが、メディアンフィルタではノイズが取り除かれ、ぼやけも小さいことが確認できた。
