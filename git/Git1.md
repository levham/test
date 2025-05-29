# ✨ <ins> Git Snippet</ins>

### Git klasörde git yoksa ekle
```
git init
```

### Commit ekle 
```
git add .
git commit -m "v1"
```

### Son mesaj düzenleneme 
```
git commit --amend -m "Yeni commit mesajı"
git push origin main --force
```
### Klasörü projeye bağla
```
cd "proje_konumu"   
git init   
git add .   
git commit -m "İlk yükleme"   
git branch -M main   
git remote add origin https://github.com/kullaniciadi/projeadi.git  
git push -u origin main   
```

### Repoya gönder
```
git add .
git commit -m "v1"
git push -u origin main
```

### Repoyu indir
```
git clone https://github.com/levham/notes
cd proje_adi
git pull origin main
```

### Uzak depodaki değişiklikleri kendi versiyonunun üzerine çekebilirsin:
```
git rebase --abort
git pull origin main
```

### Kendi değişikliklerini kaldırıp uzak depo içeriğini almak istersen
```
git reset --hard origin/main
```
 
