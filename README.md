# PRATIKUM7_RELASICLASS

nama :Bagas DWi Prasetyo
NIM : 312110053

![Screenshot1](https://user-images.githubusercontent.com/92739297/206585544-65d9def9-3d78-4b39-9bcd-5e715b239cc2.png)

DIATAS 
adalah gambar dari hasil relasi assosiasi java

dengan 
class mahasiswa

public class mahasiswa {
    private String NIM;
    private String Nama;
    protected String [] kodemaku1=new String[2];
    protected String [] namamaku1=new String[2];
    private int jmlmaku1=0;

    public mahasiswa (String kode,String Nm){
        this.NIM=kode;
        this.Nama=Nm;
    }
    public void setKodemaku1(String kdmaku1){
        kodemaku1[jmlmaku1]=kdmaku1;
        jmlmaku1++;
    }
    public void setNamamaku1 (String Nmmaku1){
        kodemaku1[jmlmaku1]=Nmmaku1;
        jmlmaku1++;
    }
    public int getJmlmaku1(){
        return  this.jmlmaku1;
    }
    public String getNIM(){
        return this.NIM;
    }
    public String getNama(){
        return this.Nama;
    }
    public void daftarMaku1(){
        System.out.println("NIM: "+NIM);
        System.out.println("Nama: "+Nama);
        System.out.println("mata kuliah yang diambil:");
        for (int i=0;i<jmlmaku1;i++){
            System.out.println(kodemaku1[i]);
        }
    }
}
 
class dosen

package mahasiswa.java;

public class dosen{
    private String NIM;
    private String Nama;
    private String Alamat;
    private String TglLahir;
    protected String [] kodemaku1=new String[2];
    protected String [] namamaku1=new String[2];
    protected String [] kodemaku2=new String[2];
    protected String [] namamaku2=new String[2];

    private int jmlmaku1=0;

    public dosen (String kode,String Nm, String AM, String TL){
        this.NIM=kode;
        this.Nama=Nm;
        this.Alamat=AM;
        this.TglLahir=TL;
    }
    public void setKodemaku1(String kdmaku1){
        kodemaku1[jmlmaku1]=kdmaku1;
        jmlmaku1++;
    }
    public void setNamamaku2 (String Nmmaku1){
        kodemaku1[jmlmaku1]=Nmmaku1;
        jmlmaku1++;
    }
    public void setKodemaku2(String kdmaku1){
        kodemaku1[jmlmaku1]=kdmaku1;
        jmlmaku1++;
    }
    public void setNamamaku1 (String Nmmaku1) {
        kodemaku1[jmlmaku1] = Nmmaku1;
        jmlmaku1++;
    }
    public int getJmlmaku1(){
        return  this.jmlmaku1;
    }
    public String getNIM(){
        return this.NIM;
    }
    public String getNama(){
        return this.Nama;
    }
    public String getAlamat(){
        return this.Alamat;
    }
    public String getTglLahir(){
        return this.TglLahir;
    }
    public void daftarMaku1(){
        System.out.println("NIM: "+NIM);
        System.out.println("Nama: "+Nama);
        System.out.println("Alamat: "+Alamat);
        System.out.println("Tanggal Lahir: "+TglLahir);
        System.out.println("mata kuliah yang diampu:");
        for (int i=0;i<jmlmaku1;i++){
            System.out.println(kodemaku1[i]);
        }
    }
}

class UKM

package mahasiswa.java;

public class UKM {
    private String Nomer;
    private String Nama;
    protected String [] kodemaku1=new String[2];
    protected String [] namamaku1=new String[2];
    private int jmlmaku1=0;

    public UKM (String NKG,String NM ){
        this.Nomer=NKG;
        this.Nama=NM;
    }
    public void setKodemaku1(String kdmaku1){
        kodemaku1[jmlmaku1]=kdmaku1;
        jmlmaku1++;
    }
    public void setNamamaku1 (String Nmmaku1){
        kodemaku1[jmlmaku1]=Nmmaku1;
        jmlmaku1++;
    }
    public int getJmlmaku1(){
        return  this.jmlmaku1;
    }
    public String getNomer(){
        return this.Nomer;
    }
    public String getNama(){
        return this.Nama;
    }
    public void daftarMaku1(){
        System.out.println("Jumlah UKM yang dipilih : "+Nomer);
        System.out.println("kategori UKM : "+Nama);
        System.out.println("UKM KAMPUS yang diambil:");
        for (int i=0;i<jmlmaku1;i++){
            System.out.println(kodemaku1[i]);
        }
    }
}

class matakuliah

public class Matakuliah {
    private String kdmaku1;
    private String Nmmatku1;
    public Matakuliah (String kdmaku1,String Nmmatku1){
        this.kdmaku1=Nmmatku1;
        this.kdmaku1=Nmmatku1;
    }
    public void setkdBuku (String kdmaku1){
        this.kdmaku1=kdmaku1;
    }
    public  void setNmmatku1(String Nmmatku1){
        this.Nmmatku1=Nmmatku1;
    }
    public String getKdmaku1(){
        return  this.kdmaku1;
    }
    public String getNmmatku1(){
        return this.Nmmatku1;
    }
}

class main

import com.sun.org.apache.bcel.internal.generic.NEW;
import mahasiswa.java.UKM;
import mahasiswa.java.dosen;
import mahasiswa.java.mahasiswa;

public class Main {
    public static void main(String[] args) {
        mahasiswa mahasiswa1 = new mahasiswa("9900099","ASEP");
        Matakuliah MAKUL1= new Matakuliah("kd001","1.pemograman java");
        Matakuliah MAKUL2= new Matakuliah("kd002","2.pemograman python");

        mahasiswa mahasiswa2 = new mahasiswa("92020202","dulloh");
        Matakuliah MAKUL11= new Matakuliah("kd0011","1.bahasa jerman");
        Matakuliah MAKUL12= new Matakuliah("kd0012","2. olahraga");

        dosen dosen1 = new dosen("200000920","agus","pedeslohor","28/11/98");
        Matakuliah MAKUL20 = new Matakuliah("kd00112","1.bahasa jepang");
        Matakuliah MAKUL21 = new Matakuliah("kd00112","1.program keteknikan");

        UKM ukm1 =new  UKM("2","internal Kampus");
        Matakuliah MAKUL30 = new Matakuliah("HT3389","1.PRAMUKA");
        Matakuliah MAKUL31 = new Matakuliah("HT3388","2.KEWIRAUSAHAAN");





        mahasiswa1.setKodemaku1((MAKUL1.getKdmaku1()));
        mahasiswa1.setKodemaku1(MAKUL2.getKdmaku1());
        mahasiswa1.daftarMaku1();
        System.out.println();


        mahasiswa2.setKodemaku1((MAKUL11.getKdmaku1()));
        mahasiswa2.setKodemaku1(MAKUL12.getKdmaku1());
        mahasiswa2.daftarMaku1();


        dosen1.setKodemaku1((MAKUL20.getKdmaku1()));
        dosen1.setKodemaku1(MAKUL21.getKdmaku1());
        dosen1.daftarMaku1();

        ukm1.setKodemaku1((MAKUL30.getKdmaku1()));
        ukm1.setKodemaku1(MAKUL31.getKdmaku1());
        ukm1.daftarMaku1();


    }
}

kelas UKM MENGGUNAKAN MATAKULIAH
kelas mahasiswa menggunakan matakuliah
kelas dosen menggunakan matakuliah
 dari hal tersebut Asosiasi didefinisikan sebagai
hubungan yang terstruktur, yang 
secara konsep memiliki arti 
bahwa dua komponen saling
terhubung satu sama lain.
semua terhubung dengan method yang ada di matakuliah

