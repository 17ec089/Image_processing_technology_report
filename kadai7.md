# �ۑ�V�@���|�[�g

�W���摜�upoke�v�����摜�Ƃ���D���̉摜�͏c445�摜�C��600��f�ɂ��f�B�W�^���J���[�摜�ł���D

ORG = imread('poke.jpg'); % �摜�̓ǂݍ���
ORG = rgb2gray(ORG); % �����Z�W�摜�ɕϊ�
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\�� 

�ɂ���āC���摜��ǂݍ��݁C�����Z�W���ɂ������ʂ�}�P�Ɏ����D

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-1.png)  
�}1 �����Z�W�摜

�}�P�̃q�X�g�O������\������B

imhist(ORG); % �q�X�g�O�����̕\��  

�q�X�g�O������}2�Ɏ���.

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-2.png)    
�}2 �q�X�g�O����

���ɁA�_�C�i�~�b�N�����W���O����Q�T�T�ɂ��邽�߂Ɉȉ��̂悤�ɂ����B

ORG = double(ORG);  
mn = min(ORG(:)); % �Z�x�l�̍ŏ��l���Z�o  
mx = max(ORG(:)); % �Z�x�l�̍ő�l���Z�o  
ORG = (ORG-mn)/(mx-mn)*255;  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��  

�_�C�i�~�b�N�����W�g���̉摜��}�R�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-3.png)    
�}3 �_�C�i�~�b�N�����W�g���̉摜

�܂��A�摜���W�r�b�g�����Ȃ������Ƃ����Ƃ��̃q�X�g�O������\�����邽�߂Ɉȉ��̂悤�ɂ����B

ORG = uint8(ORG); % ���̍s�ɂ��čl�@����  
imhist(ORG); % �Z�x�q�X�g�O�����𐶐��A�\��  

����͔Z�x�͈̔͂��L�����鑀��ł���B�}�S�Ƀq�X�g�O�����������B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/7-4.png)    
�}4 �W�r�b�g�����Ȃ������̃q�X�g�O����

�}�Q�A�}�S���A�_�C�i�~�b�N�����W�g���̕����Z�x�͈̔͂��L���Ȃ��Ă��邱�Ƃ��킩��B