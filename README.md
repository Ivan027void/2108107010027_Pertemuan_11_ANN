## Pertemuan 11 ANN
<p>Nama: Ivan Chiari</p>
<p>NPM : 2108107010027</p>


Materi bacaan: 
- https://www.megabagus.id/deep-learning-artificial-neural-networks/ (halaman 1 - 7)
- ⁠⁠https://www.megabagus.id/deep-learning-artificial-neural-networks-aplikasi (halaman 1 - 4)

Pahami isi dari kedua artikel tersebut dan kerjakan:
- Contoh pada artikel kedua menggunakan tensorflow pada python environment
- ⁠Tugas 2 sebelumnya menggunakan SVM, kerjakan dengan menggunakan ANN pada python environment yang sama

Kumpulkan kedua tugas tersebut menggunakan repository pada github dengan nama repository: NPM_Pertemuan_11_ANN. Repository tersebut berisi:
- Dataset sebelum dipreprocessing (format csv)
- ⁠Kode python yang memuat process preprocessing, training, testing dan perhitungan akurasi
- ⁠File requirements.txt yang berisi library yang digunakan
- ⁠File README.md yang berisi penjelasan tentang kedua tugas yang dikerjakan beserta perbandingan akurasi SVM dan ANN


## How to Use

### Setting Up the Environment

1. Create a new conda environment named "tugas-11-ANN" with Python 3.10:

    ```bash
    conda create --name tugas-11-ANN python=3.10
    ```

2. Activate the newly created environment:

    ```bash
    conda activate tugas-11-ANN
    ```

### Installing Required Modules

3. Install the required modules listed in the `requirements.txt` file:

    ```bash
    pip install -r requirements.txt
    ```

### Running the Code

4. Once the environment is set up and the required modules are installed, you can run your code or scripts that depend on these modules within the "tugas-11-ANN" environment.

5. Remember to activate the environment before running your code:

    ```bash
    conda activate tugas-11-ANN
    ```

6. Execute your Python scripts or Jupyter notebooks as usual.

### Deactivating the Environment

7. When you're done working with your project, deactivate the conda environment:

    ```bash
    conda deactivate
    ```

---

**Dataset yang dipakai**
### Support Vector Clasifier (SVC)
Dataset dari kaggle https://www.kaggle.com/datasets/pushprajnamdev/diabetes-dataset

<p> in particular, all patients here are females at least 21 years old of Pima Indian heritage.</p>

* Pregnancies: Number of times pregnant
* Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
* BloodPressure: Diastolic blood pressure (mm Hg)
* SkinThickness: Triceps skin fold thickness (mm)
* Insulin: 2-Hour serum insulin (mu U/ml)
* BMI: Body mass index (weight in kg/(height in m)^2)
* DiabetesPedigreeFunction: Diabetes pedigree function
* Age: Age (years)
* Outcome: Class variable (0 or 1)

### Support Vector Regresion (SVR)
<p>Konteks:</p>
<p>Untuk mempelajari lebih lanjut tentang Algoritma SVM dan khususnya Regresi, saya telah mengunduh kumpulan data Penilaian Real Estat dari Repositori Pembelajaran Mesin UCI.</p>
<p>Ini adalah Kumpulan Data yang diunduh dari Repositori Pembelajaran Mesin UCI.<p>
<p>Deskripsi sesuai situs UCI : Kumpulan data historis pasar penilaian real estat dikumpulkan dari Sindian Dist., New Taipei City, Taiwan.<p>

<br>Informasi Atribut:
The inputs are as follows
* X1 the transaction date (for example, 2013.250=2013 March, 2013.500=2013 June, etc.)
* X2 the house age (unit: year)
* X3 the distance to the nearest MRT station (unit: meter)
* X4 the number of convenience stores in the living circle on foot (integer)
* X5 the geographic coordinate, latitude. (unit: degree)
* X6 the geographic coordinate, longitude. (unit: degree)

The output is as follow
* Y house price of unit area (10000 New Taiwan Dollar/Ping, where Ping is a local unit, 1 Ping = 3.3 meter squared)

# Perbandingan hasil SVM dan ANN
tugas SVM dapat dilihat pada repository <a href ="https://github.com/Ivan027void/Tugas-2-ML">ini</a>

## klasifikasi
 1. SVM
 model dengan kernel RBF berhasil memprediksi dengan akurasi 77%
 2. ANN
 model dengan 4 layer (input, 2 hidden, output) mendapatkan akurasi 81% setelah menghilangkan outlier

## regresi
 1. SVM
 model dengan polynomial derajat 3 memperoleh nilai mse MSE:0.24545393642224678
 2. ANN
 model dengan 4 layer (input, 2 hidden, output) menggunakan loss mse mendapat nilai 0.25035950541496277