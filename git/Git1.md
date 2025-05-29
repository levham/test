# ✨ <ins> Git Snippet</ins>

###klasörde git yoksa ekle
```
git init
```

###commit ekle 
```
git add .
git commit -m "v1"
```

###son mesaj düzenleneme 
```
git commit --amend -m "Yeni commit mesajı"
git push origin main --force
```
###klasörü projeye bağla
```
cd "proje_konumu"   
git init   
git add .   
git commit -m "İlk yükleme"   
git branch -M main   
git remote add origin https://github.com/kullaniciadi/projeadi.git  
git push -u origin main   
```

###repoya gönder
```
git add .
git commit -m "v1"
git push -u origin main
```

###repoyu indir
```
git clone https://github.com/levham/notes
cd proje_adi
git pull origin main
```

###uzak depodaki değişiklikleri kendi versiyonunun üzerine çekebilirsin:
```
git rebase --abort
git pull origin main
```

###kendi değişikliklerini kaldırıp uzak depo içeriğini almak istersen
```
git reset --hard origin/main
```
