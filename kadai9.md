# �ۑ�X�@���|�[�g

�W���摜�ufreeza�v�����摜�Ƃ���D���̉摜�͏c450�摜�C��800��f�ɂ��f�B�W�^���J���[�摜�ł���D

ORG = imread('freeza.jpg'); % �摜�̓ǂݍ���  
ORG = rgb2gray(ORG); % �����Z�W�摜�ɕϊ�  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��  

�ɂ���āC���摜��ǂݍ��݁C�����Z�W���ɂ������ʂ�}�P�Ɏ����D

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-1.png)  
�}1 �����Z�W�摜

���Ƀm�C�Y��Y�t���邽�߂Ɉȉ��̂悤�ɂ���B

ORG = imnoise(ORG,'salt & pepper',0.02); % �m�C�Y�Y�t  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��  

�m�C�Y�Y�t�������ʂ�}2�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-2.png)    
�}2 �m�C�Y�Y�t

�}�Q�𕽊����t�B���^�ŎG���������邽�߂Ɉȉ��̂悤�ɂ���B

IMG = filter2(fspecial('average',3),ORG); % �������t�B���^�ŎG������  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��  

�������t�B���^�̌��ʂ�}�R�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-3.png)    
�}3 �������t�B���^

�}�Q�����f�B�A���t�B���^�ŎG���������邽�߂Ɉȉ��̂悤�ɂ���B

IMG = medfilt2(ORG,[3 3]); % ���f�B�A���t�B���^�ŎG������  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��  

���f�B�A���t�B���^�̌��ʂ�}�S�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-4.png)    
�}4 ���f�B�A���t�B���^

�܂��A�ȉ��̂悤�ȃt�B���^��݌v�����B

f=[0,-1,0;-1,5,-1;0,-1,0]; % �t�B���^�̐݌v  
IMG = filter2(f,IMG,'same'); % �t�B���^�̓K�p  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��  

���ʂ�}�T�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/9-5.png)    
�}5 �t�B���^�݌v

�}�R�A�}�S���A�������t�B���^�̓m�C�Y���c���Ă��邤���ɂڂ₯�Ă��܂������A���f�B�A���t�B���^�ł̓m�C�Y����菜����A�ڂ₯�����������Ƃ��m�F�ł����B
