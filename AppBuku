impor  jawa . io . Konsol ;
impor  jawa . menggunakan . ArrayList ;
impor  jawa . menggunakan . Array ;
impor  jawa . menggunakan . HashMap ;

 BookApp kelas  publik {
  public  static  void  main ( String [] args ){
    Konsol  konsol = Sistem . konsol ();
    ArrayList < Buku > buku = new  ArrayList < Buku >();

    sementara ( benar ) {
      Sistem . keluar . println ( "\nMasukan Buku" );

      Sistem . keluar . print ( "Judul: " );
       Judul string = konsol . readLine ();

      Sistem . keluar . print ( "Penulis: " );
       Penulis string = konsol . readLine ();

      Sistem . keluar . print ( "Penerbit: " );
       Penerbit string = konsol . readLine ();

      Sistem . keluar . print ( "Tahun rilis: " );
      int  tahun = Bilangan Bulat . parseInt ( console .readLine ( ));

      Sistem . keluar . println ( "\npilih kategori buku:" );
      int  no = 1 ;
      untuk ( Kategori string  : Buku . CATEGORIES ){
        Sistem . keluar . println ( no + "." + kategori );
        tidak ada ++;
      }
      Sistem . keluar . print ( "pilih (1-" + Buku .KATEGORI .panjang + " ): " ) ;
       Kategori string = Buku . KATEGORI [ Bilangan bulat . parseInt ( console .readLine ()) - 1 ] ;

      buku . tambah ( Buku baru  ( judul , kategori , pengarang , penerbit , tahun ));

      Sistem . keluar . println ( "\n=========================BUKU=============== ==========================" );
      Sistem . keluar . println ( "No\tJudul\t\t\tPengarang\t\tKategori\t\tPenerbit\t\tTahun rilis" );
      Sistem . keluar . println ( "============================================ ============================" );
      tidak = 1 ;
      untuk ( Buku buku  : buku ) {
        Sistem . keluar . println ( no + "\t" + book .title + "\t\t\t" + book . author + "\t\t" + book . category + " \t\t\t" + book . publisher + "\t\t\t" + buku .tahun ) ;
        tidak ada ++;
      }
      Sistem . keluar . println ( "============================================ ============================" );

      Sistem . keluar . print ( "\nmasukkan lagi (ya/tidak)?: " );
      if (! console .readLine (). sama dengan ( "ya" )) {
        istirahat ;
      }
    }

    // buku yang dikelompokkan berdasarkan kategori
    HashMap < String , ArrayList < Buku >> groupedBooks = HashMap baru  <>();
    untuk ( Buku buku  : buku ) {
      ArrayList < Buku > groupedBook = groupedBooks . dapatkan ( buku .kategori ) ;
      if ( groupedBook == null ){
        groupedBooks . put ( book . category , new  ArrayList <>( Arrays .asList ( new Book [] { book }) ) ); 
      } lain {
        groupedBook . tambahkan ( buku );
      }
    }

    int  totalBukuLama = 0 ;
    int  totalBukuBaru = 0 ;
    untuk ( Buku buku  : buku ) {
      if ( buku . tahun < 2010 ){
        totalOldBooks ++;
      } lain {
        totalNewBooks ++;
      }
    }

    Sistem . keluar . println ( "Jumlah buku : " + buku.ukuran ( ));

    untuk ( Kategori string  : Buku . CATEGORIES ){
      ArrayList < Buku > groupedBook = groupedBooks . dapatkan ( kategori );
      if ( groupedBook == null ){
        lanjutkan ;
      }
      Sistem . keluar . println ( kategori + ": " + groupedBooks . get ( "Teknik" ). size ());
    }
    Sistem . keluar . println ( "Buku lama (<2010): " + totalOldBooks );
    Sistem . keluar . println ( "Buku baru: " + totalBukuBaru );
  }
}
