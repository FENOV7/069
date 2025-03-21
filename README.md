#include <iostream>
#include <string>

using namespace std;

int main() {
    string nik, nama, tempat_lahir, alamat, kelurahan, kecamatan, agama, pekerjaan, kewarganegaraan, status_perkawinan;
    string provinsi, kabupaten;
    char jenis_kelamin, gol_darah;
    int tanggal, bulan, tahun, rt, rw;

    // Input data dari user
    cout << "Masukkan NIK Anda: ";
    cin >> nik;
    cin.ignore();
    
    cout << "Provinsi: ";
    getline(cin, provinsi);

    cout << "Kabupaten/Kecamatan: ";
    getline(cin, kabupaten);

    cout << "Masukkan Nama Anda: ";
    getline(cin, nama);

    cout << "Masukkan Tempat/Tgl Lahir Anda: ";
    cin >> tempat_lahir >> tanggal >> bulan >> tahun;
    cin.ignore();

    cout << "Jenis Kelamin (L/P): ";
    cin >> jenis_kelamin;
    cin.ignore();

    cout << "Masukkan Golongan Darah Anda: ";
    cin >> gol_darah;
    cin.ignore();

    cout << "Masukkan Alamat Anda: ";
    getline(cin, alamat);

    cout << "Masukkan RT: ";
    cin >> rt;
    cout << "Masukkan RW: ";
    cin >> rw;
    cin.ignore();

    cout << "Masukkan Kelurahan/Desa Anda: ";
    getline(cin, kelurahan);

    cout << "Masukkan Kecamatan Anda: ";
    getline(cin, kecamatan);

    cout << "Agama: ";
    getline(cin, agama);

    cout << "Status Perkawinan: ";
    getline(cin, status_perkawinan);

    cout << "Masukkan Pekerjaan Anda: ";
    getline(cin, pekerjaan);

    cout << "Kewarganegaraan: ";
    getline(cin, kewarganegaraan);

    // Output 
    cout << "\t\t\t\t PROVINSI" << provinsi << endl;
    cout << "\t\t\t\t KABUPATEN \t\t\t\t" << kabupaten <<endl;
    cout << "NIK: " << nik << endl;
    cout << "Nama: " << nama << endl;
    cout << "Tempat/Tgl Lahir: " << tempat_lahir << " " << tanggal << " " << bulan << " " << tahun << endl;
    cout << "Jenis Kelamin: " << (jenis_kelamin == 'L' ? "Laki-Laki" : "Perempuan") << " | Gol. Darah: " << gol_darah << endl;
    cout << "Alamat: " << alamat << endl;
    cout << "RT/RW: " << rt << "/" << rw << endl;
    cout << "Kel/Desa: " << kelurahan << endl;
    cout << "Kecamatan: " << kecamatan << endl;
    cout << "Agama: " << agama << endl;
    cout << "Status Perkawinan: " << status_perkawinan << endl;
    cout << "Pekerjaan: " << pekerjaan << endl;
    cout << "Kewarganegaraan: " << kewarganegaraan << endl;
    cout << "Berlaku Hingga: SEUMUR HIDUP" << endl;
    return 0;
}
