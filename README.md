# tugas9

##SOAL

pada bagian ini saya diberikan tugas sebagai berikut :

![image](https://user-images.githubusercontent.com/92866211/144430913-3d558d60-e3e8-46a1-883b-48c72ed15ff4.png)


##JAWAB

Buatlah sebuah list sebanyak 5 elemen dengan nilai bebas

    a = [2, 4, 6, 8, 10] 

Dan kemudian akses list sebagai berikut :

>• tampilkan elemen ke 3
>• ambil nilai elemen ke 2 sampai elemen ke 4
>• ambil elemen terakhir

dari soal diatas saya mengerjakan dengan cara sebagai berikut :

    1. a[2]
    2. del a[1:4]
        print(a)
    3. del a[1] 
        print(a)

lalu ubah elemen list :

>• ubah elemen ke 4 dengan nilai lainnya
>• ubah elemen ke 4 sampai dengan elemen terakhir

dari soal diatas saya mengerjakan dengan cara sebagai berikut :

    a [3] = 9
    print (a)
    a [3:5] = 12, 14
    print(a)

dan pada soal terakhir tambah elemen list:
>• ambil 2 bagian dari list pertama (A) dan jadikan list ke 2 (B)
>• tambah list B dengan nilai string
>• tambah list B dengan 3 nilai
>• gabungkan list B dengan list A

dari soal diatas saya mengerjakan dengan cara sebagai berikut : 

    b = []
    b.extend (a[0:2])
    print(b)
    b.append ('enam')
    print(b)
    b.extend([8, 10, 12])
    print(b)
    c=a+b
    print(c)

Dibawah ini adalah syntax pada visual studio code :

![image](https://user-images.githubusercontent.com/92866211/144419801-1626dcfd-96b5-48a2-99a4-f7e22741a194.png)


##output

![image](https://user-images.githubusercontent.com/92866211/144419901-2fb194c2-5841-4a48-b413-9e8eb0beff3b.png)

#tugas
![img](gambar/sssoal2.PNG)

# Flowchart

dan contoh flowchart nya sebagai berikut :

![image](https://user-images.githubusercontent.com/92866211/144420415-57f9a6c8-b81f-4c85-8738-eb06ec058b3f.png)


## Jawab

pertama saya membuat inputan dan looping agar program terus berjalan

    while true:
        c = input("apakah ingin menambah data? y/t ")

kemudian saya membuat fungsi if apabila menginput 'y' contoh sebagai berikut :


    if (c.lower() == 'y'):                                               
            print('\nTambah Data Mahasiswa Baru')
            nama= input("Masukkan Nama\t\t: ")                                        
            nim= input("Masukkan NIM\t\t: ")                                         
            nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))                              
            nilaiUts= int(input("Masukkan Nilai UTS\t: "))                                   
            nilaiUas= int(input("Masukkan Nilai UAS\t: "))                                    
            nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)              
            data[nama]= nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir                         
            print("\nData Berhasil Ditambahkan!")

membuat percabangan if untuk apabila menginput 't' contoh sebagai berikut : 

    elif (c.lower() == 't'):                                                                    
            if data.items():                                                                     
                print("\n                      DAFTAR NILAI MAHASISWA                    ")
                print("==================================================================")
                print("| No |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
                print("==================================================================")
                i = 0
                for x in data.items():
                    i += 1
                    print("| {6:2} | {0:12s} | {1:9s} | {2:5} | {3:5} | {4:5} | {5:6} |".format(x[0], x[1][0], x[1][1], x[1][2], x[1][3], x[1][4], i))  
                print("==================================================================")
            else:
                print("\n                      DAFTAR NILAI MAHASISWA                    ")
                print("==================================================================")
                print("| No |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
                print("==================================================================")
                print("|                          TIDAK ADA DATA!                       |")
                print("==================================================================")

lalu menambahan else untuk menyetop loopingan tadi :

    else:
        break

Dibawah ini adalah syntax pada visual studio code  :

![image](https://user-images.githubusercontent.com/92866211/144430770-b48ece7a-d1ac-42f0-9486-66d227788b75.png)


## Output

![image](https://user-images.githubusercontent.com/92866211/144430820-01c55348-b78a-4341-89dd-579c8faa0a57.png)



