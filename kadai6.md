# �ۑ�U�@���|�[�g

�W���摜�ufreeza�v�����摜�Ƃ���D���̉摜�͏c450�摜�C��800��f�ɂ��f�B�W�^���J���[�摜�ł���D

ORG=imread('freeza.jpg'); % ���摜�̓���
ORG = rgb2gray(ORG);
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W���ɂ������ʂ�}�P�Ɏ����D

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/6-1.png)  
�}1 �����Z�W�摜

����臒l��128�Ƃ��ē�l�����邽�߂Ɉȉ��̂悤�ɂ���B

IMG = ORG>128; % 128�ɂ���l��  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��  

臒l�ɂ���ē�l���������ʂ�}2�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/6-2.png)    
�}2 ��l���摜(臒l)

�Ō�ɁA�f�B�U�@�ɂ���ē�l�����邽�߂Ɉȉ��̂悤�ɂ���B

IMG = dither(ORG); % �f�B�U�@�ɂ���l��  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��  

�f�B�U�@�ɂ���ē�l���������ʂ�}�R�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/6-3.png)    
�}3 ��l���摜(�f�B�U�@)

�}�Q�A�}�R���A�f�B�U�@�͂��炴�炵�������ɂȂ邪�A�Ώە��Ɣw�i����ʂ��₷���Ȃ邱�Ƃ��킩��B