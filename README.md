Bisa nyambung juga ke link ini https://drive.google.com/drive/folders/1AivMVl_m3uLFCOM0zTVTPgbjckxa339-

# TubesRobotika
Kelompok 4 URDF
1. M. Fahmi Ilmi Y - 1103210268
2. Tanto Indra WIcaksono - 1103210272
3. Raihan Aryanta putra - 1103210274
3. Muhammad Lugas Lumaksono - 1103210002
4. muhammad ma'ruf firmansyah – 1103210273
Prodi: Teknik Elektro
Matkul: Robotika – Tubes

Baca ini dulu!
Penjelasan:
Tubes ini adalah workspace ROS yang berisi dua package utama: dobot dan tubes_pkg. Bagian kami ini digunakan untuk mengontrol dan mengoperasikan robot Dobot menggunakan ROS. Adapun struktur direktori di file kami adalah sebagi berikut :
	build/: Direktori hasil build dari workspace.
	devel/: Direktori hasil develop dari workspace.
	src/: Direktori yang berisi source code dari proyek.
•	dobot/: Package untuk mengontrol robot Dobot.
o	launch/: Berisi file launch untuk menjalankan node ROS.
o	src/: Berisi kode sumber untuk package Dobot.
•	tubes_pkg/: Package utama dari proyek.
o	launch/: Berisi file launch untuk menjalankan node ROS.
o	src/: Berisi kode sumber untuk package tubes_pkg.
	.vscode/: Berisi konfigurasi untuk Visual Studio Code.
	CMakeLists.txt: File konfigurasi build untuk workspace.
Cara Kerja:
ROS (Robot Operating System) digunakan untuk mengelola komunikasi antar komponen perangkat lunak yang mengontrol robot Dobot. cara kerja sebagi berikut:
1.	Node: Program yang berjalan sebagai bagian dari ROS yang bisa saling berkomunikasi.
2.	Topic: Saluran komunikasi di mana node dapat mengirim dan menerima pesan.
3.	Launch Files: File XML yang mendefinisikan konfigurasi untuk menjalankan satu atau lebih node.
Di mana terdapat:
Package dobot: Berfungsi untuk mengendalikan robot Dobot. Ia memiliki node yang berinteraksi dengan hardware robot dan mengirimkan perintah melalui ROS.
Package tubes_pkg: Merupakan package utama yang berisi logika dan algoritma spesifik yang dibutuhkan untuk menjalankan tugas-tugas tertentu pada robot Dobot.
Cara penggunaan:
	ROS: Pastikan ROS sudah terpasang pada sistem Anda.
	Dobot SDK: Pastikan SDK Dobot sudah terpasang dan dapat diakses oleh ROS.
Langkah-Langkah:
1.	Kloning Repositori
git clone <repository-url> tubes_ws
cd tubes_ws
2.	Build Workspace
catkin_make
3.	Hubungkan dengan setup file
source devel/setup.bash
4.	Menjalankan node
roslaunch dobot <file_launch>.launch
roslaunch tubes_pkg <file_launch>.launch
5.	Perintah menjalankan
roslaunch dobot control.launch




