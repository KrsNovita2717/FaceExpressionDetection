# Face Expression Detection

Repositori ini berisi notebook Colab untuk mendeteksi ekspresi wajah menggunakan gambar dan webcam. 

## File yang Tersedia

- **ExpressionRecognitionImage.ipynb**: Digunakan untuk mendeteksi ekspresi wajah pada gambar statis.
- **ExpressionRecognitionWebcam.ipynb**: Digunakan untuk mendeteksi ekspresi wajah secara real-time melalui webcam.
- **FaceExpressionDetection.ipynb**: Notebook ini berisi kode untuk melatih model deteksi ekspresi wajah.

## Cara Mengunduh Model

Anda dapat mengunduh model untuk deteksi ekspresi wajah dengan mengklik [FaceDetectionModel](https://drive.google.com/uc?id=1BuVp5Te1vKMV062dJANtgf2o1ob7exZ4).

## Dataset

Dataset yang digunakan untuk melatih model adalah [Face Expression Recognition Dataset](https://www.kaggle.com/jonathanoheix/face-expression-recognition-dataset) dari Kaggle. 

Anda dapat mengunduh dataset tersebut dari tautan tersebut dan memasukkan ke drive<br />
atau menggunakan perintah berikut (bersifat sementara):
1. Sebelum menggunakan API Kaggle, Anda perlu mengautentikasi menggunakan token API. Langkah-langkahnya adalah sebagai berikut:
   - Buka tab [Account](https://www.kaggle.com/settings/account) pada profil pengguna Kaggle Anda.
   - Pilih opsi 'Create New Token'.
   - Ini akan memicu pengunduhan file kaggle.json, yang berisi kredensial API Anda.
2. Unduh dataset

from google.colab import files <br />
*#Upload kunci API Kaggle*<br />
uploaded = files.upload()

*# Pindahkan file ke direktori Kaggle*<br />
!mkdir -p ~/.kaggle<br />
!cp kaggle.json ~/.kaggle/<br />
!chmod 600 ~/.kaggle/kaggle.json

*# Unduh dataset dari Kaggle*<br />
!kaggle datasets download -d jonathanoheix/face-expression-recognition-dataset

## Cara Penggunaan

1. Buka salah satu notebook yang diinginkan menggunakan Google Colab.
2. Ikuti instruksi dalam notebook untuk menjalankan program.
3. Anda dapat memuat gambar atau menggunakan webcam untuk mendeteksi ekspresi wajah.

## Dependensi

Pastikan Anda memiliki instalasi Python 3 dan pustaka berikut sebelum menjalankan notebook:

- TensorFlow
- OpenCV
- NumPy
- PIL
- gdown

## Lisensi

Tidak ada lisensi yang disertakan. Silakan gunakan dan modifikasi kode sesuai kebutuhan Anda.

## Penulis

Dibuat oleh [KrsNovita2717](https://github.com/KrsNovita2717)
