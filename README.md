<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
</head>
<body>

  <h1>📊 K-Means Kümeleme Analizi</h1>

  <p>
    Bu proje, <strong>k-means kümeleme algoritması</strong> kullanılarak bir veri kümesinin nasıl gruplandığını
    ve ideal küme sayısının <em>Elbow Yöntemi</em> ve <em>Silhouette Score</em> ile nasıl belirlendiğini göstermektedir.
    Yapay bir veri kümesi oluşturulmuş ve analiz edilmiştir.
  </p>

  <h2>📌 Proje Akışı</h2>

  <ol>
    <li><strong>Veri Üretimi:</strong> <code>make_blobs</code> kullanılarak 4 farklı merkeze sahip 300 örnekten oluşan bir veri kümesi oluşturuldu.</li>
    <li><strong>K-Means Uygulaması:</strong> Veri kümesine k-means algoritması uygulandı. İlk olarak k=4 seçildi.</li>
    <li><strong>Silhouette Score:</strong> Kümeleme sonucunun kalitesi <em>Silhouette Score</em> ile ölçüldü. Bu skor, kümelerin ne kadar ayrıştığını gösterir.</li>
    <li><strong>Elbow Yöntemi:</strong> K değerleri 1 ile 10 arasında denenerek WCSS değerleri hesaplandı. 
    WCSS'nin (Within-Cluster Sum of Squares) grafiği çizildi ve dirsek (elbow) noktası incelendi.</li>
  </ol>

  <h2>📈 Öne Çıkan Bulgular</h2>
  <ul>
    <li><strong>Silhouette Score:</strong> k=4 için yüksek bir skor elde edildi (~0.87). Bu, veri kümesinin doğal olarak 4 kümeye ayrıldığını gösterir.</li>
    <li><strong>Elbow Grafiği:</strong> WCSS grafiğinde belirgin bir kırılma noktası (dirsek) k=3-4 civarında oluştu. Bu da ideal küme sayısının 4 olduğunu doğruladı.</li>
    <li><strong>Farklı k Değerleri:</strong> k=2 veya k=5 denendiğinde, Silhouette Score belirgin şekilde düştü. Bu, yanlış küme sayısının nasıl etki ettiğini gösterdi.</li>
  </ul>

  <h2>✅ Sonuç</h2>
  <p>
    Bu proje, <strong>k-means</strong> algoritmasının kümeleme görevinde nasıl kullanıldığını, 
    <strong>Elbow Yöntemi</strong> ve <strong>Silhouette Score</strong> gibi metriklerin küme sayısı seçimini nasıl desteklediğini açıkça göstermektedir.
  </p>
 
</body>
</html>
