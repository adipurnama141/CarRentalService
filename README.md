Copyright		:	(c) Kelompok CarRental PPLS
Service			:	CarRentalService
Provider		: 	CRS
Domain			: 	id.kcrsppls.crs
Brief			:	Car Rental Service
Endpoint		:	http://127.0.0.1/endpoint.php
Type Definitions:

string nama_idkota;
string merk_jenis_idmobil;
string infomobil;
string statusmobil;
string listpeminjaman;
string rangetanggal;
string infotransaksi;

string databooking;
string dataperpanjang;
string datamobil;

int idkota;
int idmobil;
int idtransaksi;
int success;


Function Prototypes:
# list available kota
nama_idkota LAK(void);

# list available mobil di kota
merk_jenis_idmobil LAMK(idkota);

# get mobil
infomobil GM(idmobil);

# add mobil
success AM(datamobil);

# edit mobil
success EM(idmobil, datamobil);

# get status mobil
statusmobil GSM(idmobil);

# edit status mobil
success ESM(idmobil,statusmobil);

# list peminjaman
listpeminjaman LP(rangetanggal);

# get peminjaman
infotransaksi GP(idtransaksi);

# add transaksi peminjaman
success AP(infotransaksi);

# edit transaksi peminjaman
success EP(idtransaksi, infotransaksi);

# booking car
idtransaksi BC(databooking);

# cancel booking
success CB(idtransaksi);

# kembalikan mobil
success KM(idtransaksi);

# perpanjang peminjaman
success PP(idtransaksi,dataperpanjang);




