# Traffic-Signs-Detection-Tensorflow-YOLOv3-YOLOv4
Tugas Akhir Penerapan Machine Learning pada Sistem Mekatronika.


## Tentang ##
Sistem pengenalan, deteksi (menemukan letak dan ukuran objek pada citra masukan), dan klasifikasi (mengklasifikasikan objek yang terdeteksi ke dalam subkelas). Kedua tugas tersebut biasanya dilakukan dengan model deteksi/klasifikasi tunggal seperti YOLO atau SSD, di mana gambar masukan diberi label dengan kotak pembatas dan kelas masing-masing. Namun, memberi label dan melatih kumpulan data tersebut memerlukan banyak waktu dan upaya. Oleh karena itu, tujuan utama proyek ini adalah untuk mendeteksi hanya satu kelas utama (rambu), dan mengintegrasikan Jaringan Neural Konvolusional yang dibuat khusus untuk mengklasifikasikan objek yang terdeteksi (subkelas seperti batas kecepatan, rambu berhenti, dll). Dengan cara ini, kita hanya perlu melatih model deteksi satu kali, untuk mendeteksi satu kelas utama, sementara beberapa model klasifikasi dapat dilatih untuk mengklasifikasikan objek yang terdeteksi sesuai kebutuhan tugas.

![alt text](https://github.com/Alzaib/Traffic-Signs-Detection-Tensorflow-YOLOv3-YOLOv4/blob/main/images/flow.png)

## Output  ##
### Detection in Real Time ###

![gif](https://github.com/Alzaib/Traffic-Signs-Detection-Tensorflow-YOLOv3-YOLOv4/blob/main/images/demo.gif)

### Detection on Saved Images ###
![alt text](https://github.com/Alzaib/Traffic-Signs-Detection-Tensorflow-YOLOv3-YOLOv4/blob/main/images/output_images/1.jpg)
![alt text](https://github.com/Alzaib/Traffic-Signs-Detection-Tensorflow-YOLOv3-YOLOv4/blob/main/images/output_images/2.jpg)
![alt text](https://github.com/Alzaib/Traffic-Signs-Detection-Tensorflow-YOLOv3-YOLOv4/blob/main/images/output_images/6.jpg)


## Setup and Requirement ## 
OpenCV (version 4)

Python 

Numpy

TensorFlow 

Keras

## YOLO Implementation ##

Untuk proyek ini, karena keterbatasan waktu, saya memutuskan untuk menggunakan kumpulan data yang tersedia untuk umum (rambu lalu lintas Jerman) untuk melatih YOLO pada kumpulan data khusus saya yang dapat ditemukan di sini [1]. Rambu-rambu dalam dataset ini dibagi menjadi 4 kelas utama (larangan, bahaya, wajib dan lainnya). Karena memberi label ulang gambar menjadi 1 kelas adalah proses yang memakan waktu, jadi kami memutuskan untuk menggunakan kumpulan data dengan 4 kelas. YOLOv3 dan YOLOv4-Tiny khusus dilatih di Google Colab.

## Classification Model ##

Bagian ini melibatkan pembangunan jaringan saraf konvolusional khusus untuk mengklasifikasikan antara 43 kelas rambu lalu lintas. Kumpulan data yang digunakan untuk bagian ini dapat ditemukan di sini [2]. Metode tambahan untuk menyeimbangkan dan memperluas kumpulan data digunakan untuk prediksi keluaran yang lebih baik. Model ini juga dilatih di Google Colab.

## Weight ##
Weight: https://drive.google.com/drive/folders/1cJl0CUJXfGHbd7LQWa1pcOIzKLrf2jdf?usp=sharing

## References ## 

[1] Dataset (YOLO Format): https://www.kaggle.com/valentynsichkar/traffic-signs-dataset-in-yolo-format

[2] Dataset (Classification): https://drive.google.com/drive/folders/15ZFDX9nNrkwMIas9FUO0V1AaiXquztCl?usp=sharing 

[3] YOLO GoogleColab Tutorial: https://www.youtube.com/watch?v=_FNfRtXEbr4&t=703s 
