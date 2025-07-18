📘 Tugas Besar PBE — Pemodelan Penyebaran Worm Berbasis Model SIRD
Repositori ini berisi implementasi tugas besar mata kuliah Pemodelan Berbasis Energi (PBE) dengan pendekatan matematis menggunakan model SIRD (Susceptible–Infected–Recovered–Dead) untuk memodelkan penyebaran worm dalam suatu sistem jaringan komputer.

🧮 Model Matematika
Model ini memanfaatkan beberapa parameter penting seperti:

$N$ : Total populasi (sistem yang diamati)

$\alpha$ : Tingkat deteksi oleh IDS/IPS

$\beta$ : Tingkat infeksi worm

$\gamma$ : Tingkat pemulihan

$\mu$ : Tingkat kematian sistem

$\delta$ : Tingkat kembali rentan

$p$ : Peluang sistem terkena infeksi

Model diferensial yang digunakan:

$\displaystyle \frac{dS}{dt} = -p \cdot \frac{\beta S I}{N} - (1-p) \cdot \alpha S + \delta R$

$\displaystyle \frac{dI}{dt} = p \cdot \frac{\beta S I}{N} - \gamma I - \mu I$

$\displaystyle \frac{dR}{dt} = (1-p) \cdot \alpha S + \gamma I - \delta R$

$\displaystyle \frac{dD}{dt} = \mu I$

⚙️ Tools dan Library
Notebook ini menggunakan:

Python (Jupyter Notebook)

numpy, scipy.integrate untuk penyelesaian numerik

matplotlib untuk visualisasi

📊 Hasil
Visualisasi dari masing-masing variabel (S, I, R, D) ditampilkan dalam bentuk grafik terhadap waktu, yang memberikan gambaran dinamika infeksi worm pada jaringan berdasarkan parameter yang ditentukan.

