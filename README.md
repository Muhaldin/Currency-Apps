Cureency Apps
Aplikasi ini mencakup fungsi perhitungan nilai tukar satu dollar di anggap Rp 15.000

Scope & Functionalities
user dapat memasukkan angka
user dapat menyentuh tombol hitung
user mendapat info "INVALID" jika di masukkan berupa text
How Does It Works?
di awali dari method mainwindow pada class MainWindow.xaml.cs, kita mendeklarasikan

''' public MainWindow()

    {
        InitializeComponent();
        currency = new CurrencyController();
    }
'''

logika perhitungan terdapat pada class CurrencyControll.cs sebagai berikut:

'''

public string usdToIdr(string nominal)

    {
        var nominalDouble = Convert.ToDouble(nominal);
        var result = nominalDouble * 15000;
        return Convert.ToString(result);
    } 
