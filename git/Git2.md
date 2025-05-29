# 📂 Git
 
<table >
  <tr>
    <th>Açıklama </th>
    <th>Git Kodu</th>
  </tr>
  <tr>
	<td>git yükleme yeri</th>
    <td><a href="https://git-scm.com/downloads/win target="_blank">git-scm.com</a><br> </td>
  </tr>
  <tr>
    <td>git yüklenmiş mi diye kontrol et</td>
    <td><pre><code>git --version </code></pre></td>
  </tr> 
  <tr>
    <td>eğer olmuyorsa: </td>
    <td>
		yukarıdaki yerden yükle <br>
		yüklendiği yolu kontrol et <br>
		konumunu path a kaydet
    </td>
  </tr>
  <tr>
    <td>eğer git varsa hesabını kaydet</td>
    <td>
    	<pre><code>git config --global user.name  ? </code></pre><br>
    	<pre><code>git config --global user.email ? </code></pre>
    </td>
  </tr>

<tr>
    <td>terminal kullanımı</td>
    <td>
    	<a href="https://youtu.be/aHOzKAe6bGE?list=PLeGbjrys0OZKPvB7z2JNT8Nxp4VfnFiN6 target="_blank">link1</a><br>
    	<a href="https://youtu.be/UWmIkn3f1UM?list=PLeGbjrys0OZKPvB7z2JNT8Nxp4VfnFiN6 target="_blank">link2</a>
    </td>
 </tr>

 <tr>
    <td>git komutları</td>
    <td><a href="https://git-scm.com/search/results?search=&language=en" target="_blank">git-scm.com/search</a></td> 
  </tr>
 
 <tr>
    <td>git deposu açar ve dosyaları izler.</td>
    <td><pre><code>git init</code></pre></td>
  </tr>

  <tr>
    <td>mevcut durum commitler, brachlar ,silinmiş dosyalar ,yeni dosyalar görüntüleme</td>
    <td><pre><code>git status</code></pre></td>
  </tr>
 
 <tr>
    <td>state bölgesine dosya gönderme </td>
    <td>
    	<pre><code>git add ? </code></pre><br>
    	<pre><code>git add . </code></pre>
    </td>
  </tr>
 
 <tr>
    <td>göndermeden önceki yorum yapma</td>
    <td><pre><code>git commit -m "yorum" </code></pre></td>
  </tr>

 <tr>
    <td>bütün dosyalar takip ediliyorsa ve stagede değilse</td>
    <td><pre><code>git commit -am "?" </code></pre></td>
  </tr>
 
 <tr>
    <td>stage bölgesinden geri alır </td>
    <td><pre><code>git restore --staged ? </code></pre><br>
    	<pre><code>git restore --staged . </code></pre></td>
  </tr>

 <tr>
    <td>commit geçmişi <br>--oneline tek satırda </td> 
    <td><pre><code>git log </code></pre><br>
    	<pre><code>git log --oneline </code></pre></td>
  </tr>
 
 <tr>
    <td>enson commit ettiğini düzenlemek</td>
    <td><pre><code>git add .</code></pre><br>
    	<pre><code>git commit --amend </code></pre></td>
  </tr>
  
 <tr>
    <td>gitignore dosyası</td>
    <td>commit edilmesini istemediğin dosyaları .gitignore içine teker teker veya <br>
	test/  gibi klasör adıyla veya *.js tüm js dosya gibi yazabilirisin.<br>
	git status yapınca görünmüyorlar</td>
  </tr>
  
<tr>
    <td><pre><code>git rm --cached ?</code></pre><br>
    	<pre><code>git rm --cached -r ? </code></pre><br> 
    	<pre><code>git rm --cached config.json </code></pre></td>
    <td>diyelimki config.json dosyasını gitignore ye koymadan commit edilmişse config.json dosyasında değişiklik yapınca bu değişiklik git statusta görünüyor. buna engel olmak için git rm --cached config.json yazqabilirsin bu sayede daha takip edilmez. klasörler için  git rm --cached -r </td>
</tr>
 
<tr>
    <td>visual studio code'da git</td>
    <td>visual studio code da dosya listesinde gitignore varsa onun içindeki dosya o listede soluk renkte görülür. ayrıca takip edilen ve edilmeyen dosyalarda görülür. değişiklik bir dosyada yapılmışsa turuncu renkte yazı rengi değişir ve yanında M sembolu olur .eğer yanında U yazarsa takip edilmeyen anlamında </td>
</tr>
<tr>
	<td><pre><code>git branch</code></pre> </td>
	<td>branch listeler ve mevcut branch başında * görünür </td>
</tr>

<tr>
    <td><pre><code>git switch -C ? </code></pre> </td>
	<td>yeni brancg oluşturur ve geçiş yapar </td>
</tr>
<tr>
	<td><pre><code>git branch -m </code></pre></code> </td>
	<td>şuanki branch adı değiştirir </code></td>
</tr>
<tr>
	<td><pre><code>git branch -d test</code></pre> <br>
 	<pre><code>git branch -D </code></pre> </td>
 	<td>test branchını siler ama bulunduğu yeri silemezsin diğer brancha geçiş yapmalısın </td>
<tr>
<tr>
    <td> <pre><code>git switch ? </code></pre></td>
    <td>branchlara geçiş yapar.ve geçiş yaptığı branch a göre dizinde o dosyalar görünür.</td>
</tr> 
<tr>
    <td> <pre><code>git checkout</code></pre></td>
    <td>git switch in alternatifi eskisii</td>
</tr>
<tr>
    <td> <pre><code>git switch -f master </code></pre></td>
    <td>branchlar arası geçişte değişikliği kaydedilmeyen dosyalar için uyarı alınabilir  - f parametresiyle geçiş yapabilrisiniz ama veri kaybı oluyor </td>
</tr>
<tr> 
    <td> <pre><code>git remote add origin ?repourl? </code></pre> <br>
         <pre><code>git remote -v </code></pre> <br>
         <pre><code>git remote remove ?name? </code></pre></td> 
    <td> Remote Repository Ekleme ve Yönetme <br><br>
         Uzaktaki bir repo ekler. <br><br>
         Mevcut uzak repo bağlantılarını listeler. <br><br>
         Uzak repo bağlantısını kaldırır.</td>
</tr>
<tr>
    <td> <pre><code>git merge ?branch-name? </code></pre><br>
         <pre><code>git rebase ?branch-name?</code></pre></td> 
    <td> Branchleri Birleştirme (Merge & Rebase)<br>
         Belirtilen branch'ı mevcut branch'e birleştirir.<br>
         Mevcut branch'i belirlenen branch'e yeniden düzenler. </td>
</tr>
<tr>
    <td> <pre><code>git checkout -- ?file? </code></pre><br>
         <pre><code>git reset --soft HEAD~1 </code></pre><br>
         <pre><code>git reset --hard HEAD~1 </code></pre></td> 
    <td> Değişiklikleri Geri Alma (Undo & Reset)<br>
         Belirtilen dosyayı son commit durumuna döndürür.<br>
         Son commit'i geri alır ama değişiklikleri korur.<br>
         Son commit'i ve tüm değişiklikleri tamamen siler</td>
</tr>
<tr>
    <td> <pre><code>git stash </code></pre><br> 
         <pre><code>git stash list </code></pre><br>
         <pre><code>git stash apply </code></pre><br>
         <pre><code>git stash drop </code></pre></td>
    <td> Git Stash (Geçici Olarak Değişiklikleri Kaydetme)<br>
         Çalışma alanındaki değişiklikleri geçici olarak saklar.<br>
         Saklanan değişiklikleri listeler.<br>
         Son saklanan değişiklikleri tekrar uygular.<br>
         Saklanan değişiklikleri siler.</td>
</tr>
<tr>
    <td> <pre><code>git tag -a v1.0 -m "Version 1.0" </code></pre><br>
         <pre><code>git tag </code></pre><br>
         <pre><code>git push origin --tags </code></pre></td>
    <td> Tag Kullanımı (Sürüm Etiketleme)<br>
         Belirtilen sürümde bir etiket oluşturur.<br>
         Tüm etiketleri listeler.<br>
         Tüm etiketleri uzak repoya gönderir.</td>
<tr>
</table>