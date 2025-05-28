# 📂 Git
 
<table >
  <tr>
    <th>Açıklama </th>
    <th>Git Kodu</th>
  </tr>
  <tr>
	<td>git yükleme yeri</th>
    <td>[**_git-scm.com_**](https://git-scm.com/downloads/win)</th>
  </tr>
  <tr>
    <td>git yüklenmiş mi diye kontrol et</td>
    <td><pre><code>git --version </code></pre></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
</table>



- [ ] eğer olmuyorsa
	+ yüklendiği yolu kontrol et 
	+ konumunu path a kaydet

- [ ] eğer git varsa hesabını kaydet 
	+ <pre><code>git config --global user.name  ??</code></pre>
	+ <pre><code>git config --global user.email ??</code></pre>


- [ ] terminal kullanımı 
	[^1]:https://youtu.be/aHOzKAe6bGE?list=PLeGbjrys0OZKPvB7z2JNT8Nxp4VfnFiN6)
	[^2]:https://youtu.be/UWmIkn3f1UM?list=PLeGbjrys0OZKPvB7z2JNT8Nxp4VfnFiN6)

- [ ] git komutları-> [**_git-scm.com/search_**](https://git-scm.com/search/results?search=&language=en)
	

- [ ] git init ->  git deposu açar ve dosyaları izler.
		
- [ ] git status -> mevcut durum commitler, brachlar ,silinmiş dosyalar ,yeni dosyalar görüntüler

- [ ] git add ->  state bölgesine dosya gönderir 
	<pre><code>git add asdf.txt </code></pre>
	<pre><code>git add . herşeyi gönder</code></pre>

git commit -> 
	göndermeden önceki yorum
	git commit -m "yorum"
	bütün dosyalar takip ediliyorsa ve stagede değilse ->
	git commit -am "yorum"

git restore --staged 
	stage bölgesinden geri alır 
	git restore --staged . hepsini geri alır 

git log 
	commit geçmişi
	git log --oneline tek satırdaki loglar

git commit --amend
git add ile 2 dosyadadn birini stageye gönderdikten ve git commit -m "" ettikten sonra stagede olmayan dosyayı deklemek istersen git add ile ekle sonra git commit --amend yaz çıkan sayfada commit ediceğin metni yaz bu sayede en son mmit ettiğin şey düzenlenmiş olucak

gitignore ->
	commit edilmesini istemeidğin dosyaları .gitignore içine teker teker veya test/  gibi klasör adıyla yazabilrisin veya *.js tüm js dosya gibi yazabilirisin.
git status yapınca görünmüyor bu sayede gitignore ile 

git rm --cached
	diyelimki config.json dosyasını gitignore ye koymadan commit ettin sonra config.json dosyasında değişiklik yapınca bu değişiklik git statusta görünüyor. buna engel olmak için git rm --cached config.json yazqabilirsin bu sayede daha takip edilmez. klasörler için  git rm --cached -r 

visual studio code da dosya listesinde gitignore varsa onun içindeki dosya o listede soluk renkte görülür. ayrıca takip edilen ve edilmeyen dosyalarda görülür. değişiklik bir dosyada yapılmışsa turuncu renkte yazı rengi değişir ve yanında M sembolu olur .eğer yanında U yazarsa takip edilmeyen anlamında 

git branch -> 
	branch listeler master gibi 
	mevcut branch başında * görünür
	git branch test komtu testisminde branch oluşturur 
	git switch -C test3 yeni brancg oluşturur ve geçiş yapar
	git branch -m yeniisim komutuyla şuanki branch adı değişti 
	git branch -d test komutu test branchını siler  ama bulunduğu yeri silemezsin diğer bracha geçiş yapıp öyle komuytu kullanabilrisin 
	git branch -D test


git switch ->
	git siwtch test test branchına greçiş yapar.ve geçiş yaptığı branch a göe dizinde o dosyalar görünür.

git checkout ->
	git sitch in alternatifi eskisii

git switch -f master 
branchlar arası geçişte değişikliği kaydedilmeyen dosyalar için uyarı alınabilir  - f parametresiyle geçiş yapabilrisiniz ama veri kaybı oluyor 
https://youtu.be/ntUaf2NHE00?list=PLeGbjrys0OZKPvB7z2JNT8Nxp4VfnFiN6
