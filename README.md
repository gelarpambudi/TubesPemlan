# Tugas Besar Pemrograman Lanjut 
Oleh : <b>Gelar Pambudi A. /18117020</b> dan <b>M. Taufiq Rafiandi / 18117035</b>


Klasifikasi jenis sampah anorganik menggunakan deep learning. Klasifikasi dilakukan dengan menggunakan cara image classification.
Algoritma yang digunakan berupa CNN (Convolutional Neural Network).

Spesifikasi yang digunakan :
<ul>
  <li><b>Python 3.6.7</li>
  <li>Tensorflow-gpu 1.9</li>
  <li>Tensorflow-gpu 1.15 (untuk transfer learning)</li>
  <li>Keras</li>
  <li>Cuda Toolkit 9.0</li>
  <li>Cuda Toolkit 10.0 (untuk transfer learning)</li>
  <li>cuDNN 7.6.4</b></li>
</ul>


Dataset berupa gambar sampah. Dataset diperoleh dari link berikut : <a href=https://github.com/garythung/trashnet/tree/master/data>Dataset Sampah </a></br>

Kategori sampah yang akan diklasifikasikan : 
<ul>
  <li><b>Plastic</li>
  <li>Glass</li>
  <li>Paper</li>
  <li>Cardboard</li>
  <li>Metal</li>
  <li>Trash</b></li>
</ul>


Terdapat 3 jenis model yang diuji :
 
 <ul>
  <li>Model pertama yang dicoba di-train sebanyak 120 epoch. Hasil akhir model memiliki akurasi validasi sebesar 74,9%. </br>
       Model disimpan dalam file <b>modelConfig.h5</b>. Training history dari model tidak tersimpan</li>
  <li>Model kedua yang dicoba di-train sebanyak. Hasil akhir model memiliki akurasi validasi sebesar 78%.
      Model disimpan dalam file <b>modelConfig2.h5</b>. Training history dari model disimpan dalam file <b>historyModel2</b></li>
  <li>Model ketiga yang dicoba adalah hasil Transfer Learning dari model DenseNet121. Model tersebut di-train sebanyak 70 epoch.</br>
      Model disimpan dalam file <b>modelConfigTransferLearning.h5</b>. Training history dari model tidak tersimpan</li>
 </ul>
 
 File jupyter untuk training dan prediksi :
 <ul>
  <li><b>Model 1 : Tubes1.ipynb</li>
  <li>Model 2 : Tubes2.ipnyb</li>
  <li>Model 3: TubesTransferLearning.ipynb</li>
  <li>Prediksi : TubesPredict.ipynb</b></li>
 </ul>
 
 Dari ketiga model yang dicoba untuk melakukan prediksi, model hasil Transfer Learning memiliki performa paling bagus.
 
 
 ### Referensi
 <ul>
  <li><a href= https://arxiv.org/ftp/arxiv/papers/1908/1908.04393.pdf>Fine-Tuning Models Comparisons on Garbage Classification for Recyclability</a></li>
  <li><a href=https://github.com/frankplus/trash-cnn>https://github.com/frankplus/trash-cnn</a></li>
  <li><a href=https://www.kaggle.com/vasantvohra1/using-cnn-test-accuracy-77>https://www.kaggle.com/vasantvohra1/using-cnn-test-accuracy-77</a></li>
</ul>
