# �ۑ�Q���|�[�g

�W���摜�ufreeza�v�����摜�Ƃ���D���̉摜�͏c450�摜�C��800��f�ɂ��f�B�W�^���J���[�摜�ł���D

ORG=imread('freeza.jpg'); % ���摜�̓���  
ORG = rgb2gray(ORG); colormap(gray); colorbar;  
imagesc(ORG); axis image; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W���ɂ������ʂ�}�P�Ɏ����D

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-1.png)  
�}1 �����Z�W�摜

���Ɍ��摜��2�K���ɂ��邽�߂Ɉȉ��̂悤�ɂ���.

IMG = ORG>128;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

2�K���̌��ʂ�}2�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-2.png)    
�}2 2�K���摜

���Ɍ��摜��4�K���ɂ��邽�߂Ɉȉ��̂悤�ɂ���.

IMG0 = ORG>64;  
IMG1 = ORG>128;  
IMG2 = ORG>192;  
IMG = IMG0 + IMG1 + IMG2;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

4�K���̌��ʂ�}3�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-3.png)    
�}3 4�K���摜

�Ō�Ɍ��摜��8�K���ɂ��邽�߂Ɉȉ��̂悤�ɂ���.

IMG3 = ORG>32;  
IMG4 = ORG>64;  
IMG5 = ORG>96;  
IMG6 = ORG>128;  
IMG7 = ORG>160;  
IMG8 = ORG>192;  
IMG9 = ORG>224;  
IMG = IMG3 + IMG4 + IMG5 + IMG6 + IMG7 + IMG8 + IMG9;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

8�K���̌��ʂ�}2�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/2-4.png)    
�}4 8�K���摜

�ȏ���A�K���𑽂����邱�ƂłȂ߂炩�ȃO���f�[�V�����ŕ\���ł���.