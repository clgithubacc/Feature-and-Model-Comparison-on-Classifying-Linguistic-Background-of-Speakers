# Python Audio Analysis library

install instruction:  
1:   
git clone https://github.com/tyiannak/pyAudioAnalysis.git  
2:  
cd pyAudioAnalysis  
3: Install dependencies:  
pip install -r ./requirements.txt  
4:  
pip install -e .  
  
  
The features can be extracted are listed below:  
1-Zero Crossing Rate：短时平均过零率，即每帧信号内，信号过零点的次数，体现的是频率特性  
2-Energy：短时能量，即每帧信号的平方和，体现的是信号能量的强弱  
3-Entropy of Energy：能量熵，跟频谱的谱熵（Spectral Entropy）有点类似，不过它描述的是信号的时域分布情况，体现的是连续性  
4-Spectral Centroid：频谱中心又称为频谱一阶距，频谱中心的值越小，表明越多的频谱能量集中在低频范围内，如：voice与music相比，通常spectral
centroid较低  
5-Spectral Spread：频谱延展度，又称为频谱二阶中心矩，它描述了信号在频谱中心周围的分布状况  
6-Spectral Entropy：谱熵，根据熵的特性可以知道，分布越均匀，熵越大，能量熵反应了每一帧信号的均匀程度，如说话人频谱由于共振峰存在显得不均匀，而白噪声的频谱就更加均匀，借此进行VAD便是应用之一  
7-Spectral Flux：频谱通量，描述的是相邻帧频谱的变化情况  
8-Spectral Rolloff：频谱滚降点，给出定义： 
