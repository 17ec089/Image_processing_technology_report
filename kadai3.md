# �ۑ�R�@���|�[�g

�W���摜�ufreeza�v�����摜�Ƃ���D���̉摜�͏c450�摜�C��800��f�ɂ��f�B�W�^���J���[�摜�ł���D

ORG=imread('freeza.jpg'); % ���摜�̓���  
ORG= rgb2gray(ORG); % �J���[�摜�𔒍��Z�W�摜�֕ϊ�  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��  
�ɂ���āC���摜��ǂݍ��݁C�����Z�W���ɂ������ʂ�}�P�Ɏ����D

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-1.png)  
�}1 �����Z�W�摜

����臒l��64�Ƃ��邽�߂Ɉȉ��̂悤�ɂ���B

IMG = ORG > 64; % �P�x�l��64�ȏ�̉�f��1�C���̑���0�ɕϊ�  
imagesc(IMG); colormap(gray); colorbar;

臒l64�̌��ʂ�}2�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-2.png)    
�}2 臒l64

����臒l��96�Ƃ��邽�߂Ɉȉ��̂悤�ɂ���B

IMG = ORG > 96;  
imagesc(IMG); colormap(gray); colorbar;

臒l96�̌��ʂ�}3�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-3.png)    
�}3 臒l96

����臒l��128�Ƃ��邽�߂Ɉȉ��̂悤�ɂ���B

IMG = ORG > 128;  
imagesc(IMG); colormap(gray); colorbar;

臒l128�̌��ʂ�}4�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-4.png)    
�}4 臒l128

�Ō��臒l��192�Ƃ��邽�߂Ɉȉ��̂悤�ɂ���B

IMG = ORG > 192;  
imagesc(IMG); colormap(gray); colorbar;

臒l192�̌��ʂ�}5�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/3-5.png)    
�}5 臒l192

臒l�������Ɖ摜���Z���Ȃ邱�Ƃ��m�F�ł����B