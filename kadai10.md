# �ۑ�P�O�@���|�[�g

�W���摜�ufreeza�v�����摜�Ƃ���D���̉摜�͏c450�摜�C��800��f�ɂ��f�B�W�^���J���[�摜�ł���D

ORG = imread('freeza.jpg'); % ���摜�̓���  
ORG = rgb2gray(ORG); %�J���[����O���C�ւ̕ϊ�  
imagesc(ORG); colormap('gray'); colorbar;% �摜�\��  

�ɂ���āC���摜��ǂݍ��݁C�����Z�W���ɂ������ʂ�}�P�Ɏ����D

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-1.png)  
�}1 �����Z�W�摜

���Ƀv���E�B�b�g�@�ɂ��G�b�W���o�����邽�߂Ɉȉ��̂悤�ɂ���B

IMG = edge(ORG,'prewitt'); % �G�b�W���o�i�v���E�B�b�g�@�j  
imagesc(IMG); colormap('gray'); colorbar;% �摜�\��  

���ʂ�}�Q�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-2.png)    
�}2 �v���E�B�b�g�@

���Ƀ\�x���@�ɂ��G�b�W���o�����邽�߂Ɉȉ��̂悤�ɂ���B

IMG = edge(ORG,'sobel'); % �G�b�W���o�i�\�x���@�j  
imagesc(IMG); colormap('gray'); colorbar;% �摜�\��  

���ʂ�}�R�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-3.png)    
�}3 �\�x���@

�Ō�ɃL���j�[�@�ɂ��G�b�W���o�����邽�߂Ɉȉ��̂悤�ɂ���B

IMG = edge(ORG,'canny'); % �G�b�W���o�i�L���j�[�@�j  
imagesc(IMG); colormap('gray'); colorbar;% �摜�\��  

���ʂ�}�S�Ɏ����B

![���摜](https://github.com/17ec089/Image_processing_technology_report/blob/master/image/10-4.png)    
�}4 �L���j�[�@

�}�Q�A�}�R�A�}�S���A�L���j�[�@�̓v���E�B�b�g�@�ƃ\�x���@�ɔ�ׁA�����̃G�b�W�𒊏o���Ă��邱�Ƃ��m�F�ł����B