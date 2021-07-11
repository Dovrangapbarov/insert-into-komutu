# insert-into-komutu
tablolara insert into komutu ile 5'er tane kayıt girme


insert into public."SAKLAMA"("ID","Saklama_turu") Values (3,'Dondurucu'),(4,'Kitaplık'),(5,'Depo');
select * from public."SAKLAMA";
insert into public."TUR"("ID","Tur") Values (1,'Gıda'),(2,'Temizlik'),(3,'Kırtasiye'),(4,'Manav'),(5,'Temel ihtiyac');
select * from public."TUR";
insert into public."BİRİM"("ID","Birim") Values (1,'Adet'),(2,'Deste'),(3,'Düzine'),(4,'Metre'),(5,'Metreküp');
select * from public."BİRİM";

insert into public."URUN"("İD","Tur_id","Saklama_id","Birim_İD","Cins","Alis_fiyati","KDV") values (DEFAULT,1,2,3,'ŞEFTALİ',5,3);
insert into public."URUN"("İD","Tur_id","Saklama_id","Birim_İD","Cins","Alis_fiyati","KDV") values (DEFAULT,1,2,3,'Salatalık',6,3);
insert into public."URUN"("İD","Tur_id","Saklama_id","Birim_İD","Cins","Alis_fiyati","KDV") values (DEFAULT,1,2,3,'Elma',7,3);
insert into public."URUN"("İD","Tur_id","Saklama_id","Birim_İD","Cins","Alis_fiyati","KDV") values (DEFAULT,1,2,3,'Karpuz',1,0.5);
insert into public."URUN"("İD","Tur_id","Saklama_id","Birim_İD","Cins","Alis_fiyati","KDV") values (DEFAULT,1,2,3,'Kavun',4,2);
select * from public."URUN";

insert into public."STOK"("İD","Urun_id","Adet") Values (DEFAULT,2,500);
insert into public."STOK"("İD","Urun_id","Adet") Values (DEFAULT,1,1500);
insert into public."STOK"("İD","Urun_id","Adet") Values (DEFAULT,3,550);
insert into public."STOK"("İD","Urun_id","Adet") Values (DEFAULT,4,800);
insert into public."STOK"("İD","Urun_id","Adet") Values (DEFAULT,5,1200);
select * from public."STOK";

insert into public."SATİS"("ID","Urun_id","Adet","Satis_fiyati") Values (DEFAULT,2,300,9);
insert into public."SATİS"("ID","Urun_id","Adet","Satis_fiyati") Values (DEFAULT,1,40,9);
insert into public."SATİS"("ID","Urun_id","Adet","Satis_fiyati") Values (DEFAULT,3,150,9);
insert into public."SATİS"("ID","Urun_id","Adet","Satis_fiyati") Values (DEFAULT,4,1000,9);
insert into public."SATİS"("ID","Urun_id","Adet","Satis_fiyati") Values (DEFAULT,5,333,9);
select * from public."SATİS";
