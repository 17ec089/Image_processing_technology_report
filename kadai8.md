# �ۑ�W�@���|�[�g

�W���摜�ufreeza�v�����摜�Ƃ���D���̉摜�͏c450�摜�C��800��f�ɂ��f�B�W�^���J���[�摜�ł���D

ORG = imread('freeza.jpg'); % �摜�̓ǂݍ���  
ORG = rgb2gray(ORG); % �����Z�W�摜�ɕϊ�  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��  

�ɂ���āC���摜��ǂݍ��݁C�����Z�W���ɂ������ʂ�}�P�Ɏ����D

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/8-1.png)  
�}1 �����Z�W�摜

����臒l��128�Ƃ��ē�l�����邽�߂Ɉȉ��̂悤�ɂ���B

IMG = ORG > 128; % 臒l128�œ�l��
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��  

臒l�ɂ���ē�l���������ʂ�}2�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/8-2.png)    
�}2 ��l���摜(臒l)

�Ō�ɁA��l�����ꂽ�摜�̘A�������Ƀ��x����t���邽�߂Ɉȉ��̂悤�ɂ���B

IMG = bwlabeln(IMG);  
imagesc(IMG); colormap(jet); colorbar; % �摜�̕\��  

���x�����O�������ʂ�}�R�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/8-3.png)    
�}3 ���x�����O

�}�R���A���w�i�ɒ��ڂ���ƃ��x�����O����Ă���̂��킩��₷���B