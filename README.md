# �e��
�o�ggithub�A�Ω�����ڦb�x�W�H�u���z�ǮէU�а��V���A��2�B3�P�����D�ءA�䤤���D����B�J�쪺���D�B�ѨM��k�C<br>
�D�ج��GWhere_am_i �Ϥ���ƶ��۰ʤ���<br>
train��ƶ��A�`�@������15�����O��Ƨ��C��test��ƶ��A�s�b�@�_�A�ؼ�:����test��ơC<br>

kaggle�Ghttps://www.kaggle.com/c/aia-tc-image-cla-where-am-i/leaderboard
<br>
# ���D�B�J
1.load_data<br>
2.�[�]model<br>
3.�ΦU����k����model���\�v
## load_data
�b�̪�J�쪺�Ĥ@�Ӱ��D�N�O���Jtrain��ƶ��A�H���J�쪺�D�ءAtrain�Btest��ƶ����O�i�H�����q�M��Wload.data�N�i�H�F�A���o�����D��train�����b�U��Ƨ����C<br>
�g�L�ܪ��@�q�ɶ����İ��A�̲ױNload data�o�Ӱ��D���Ѧ��X�ӨB�J�C<br>
1.���z�Lmapping.txt���o�Ҧ���Ƨ��W�١C<br>
2.��os�M��y�Xmapping���Ҧ���Ƨ��A�åͦ��Ҧ���Ƨ����Ϥ����|�C<br>
3.��cv2�M��A�y�X�Ҧ��Ϥ��A�ñN����match��train dataset<br>
## �[�]model
�b�ѨM�Fload_data���D��A�J�쪺�ĤG�Ӱ��D�Omodel����ܡA�]���ڬO��Ǫ̡A�ҥH�u���DMLP network�A�b�@�}�l��MLP training����A�դF�U�ذѼơA
predict�����G�̵M�u��20%���k�C�N��ۧڤw�g�I��FMLP�b�o�Ӱ��D�W�������F�A����google�F�\�[�A�o�{�Ϥ������A����Ӥ�V�C<br>
1.�E�����ǲ� trainfer Learning<br>
2.���n������ CNN<br>
�̫��ܤFCNN�����s���ҲաA�]��trainfer Learning���O�ޥΧO�H�g�n���M��A�A�հѼơA����Ǫ̪��ڨӻ��A�ڷQ���O����@�ۤv��model����O���٤����A
�ҥH���CNN���ڧ�z�����ǲߨ䤤����z(���ާڪ��Dtrainfer Learning�w���@�w����n)<br>
�b��CNN�ҲդW�A�ڨ̵M���tensorflow�@���ج[�A��]�����:<br>
1.�ڦb��MLP�ɴN�Υ��F�A�򥦤����<br>
2.kares�b�غc�ҲդW�A�ٲ��F�ܦh�y�k�A���ڻ{�����Ǫ̨ӻ��Atensorflow���ŧi���M�ܪ��A������n�ݥX�[�c�C<br>
�b�ڪ��Ĥ@��CNN�Ҳիذ_�ӮɡA�ڱĥΪ��[�c�O��h���n�h�B��h���Ƽh�B���U���ۤ@�hhidden�h(1024���g��)�A��train���G�ä��z�Q�C�ǤJ���Ϥ��j�p�O32*32�A
overfitting�����p�D�`�Y���A�]���Ϥ����j�A��T���h�A�ҥH�Ҳճz�L400epcho���k�A�N�৹���Q�_��train set�F�C���F�ѨM�o�Ӱ��D�A�����ڥ[�j�F�Ϥ��j�p��128*128�A
�H�۹Ϥ��W�j�A�ڤ]�[�`�FCNN���h�ơA�ت��O��CNN����X�Ӫ��S�x�����Ahidden�h�ڤ]��Ψ�h���O��512�B216�A�o�˥X�Ӫ����G�j�j���ɤF�ǽT�v�A���ǽT�v�Ө�45%���k�C
���ۧڽվA�Ѽ�(epcho�Bbatch_size�Blr)�A��ǽT�v�����ɦ�50%���k�C���]�t���h��CNN���o�Ӱ��D�������F�C���۫��򬰤F���ɷǽT�v�A�ڿ�ܱqtrain dataset�U��C