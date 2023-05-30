# XOGame

https://user-images.githubusercontent.com/116784884/229263498-4d532513-477d-435c-be5e-8c653c6cd770.mp4



Bu kod bir X-O (Tic-Tac-Toe) oyununun basit bir Android uygulamasını temsil ediyor. Oyunda iki oyuncu X ve O olarak temsil ediliyor.

Kodun Açıklaması:

MainActivity sınıfı, AppCompatActivity sınıfından kalıtım alıyor ve ana aktiviteyi temsil ediyor.
currentPlayer değişkeni, sıradaki oyuncunun kim olduğunu takip etmek için kullanılıyor. Başlangıçta 0 (X oyuncusu) olarak ayarlanmış.
gameActive değişkeni, oyunun devam edip etmediğini belirlemek için kullanılıyor. Başlangıçta true olarak ayarlanmış.
gameState dizisi, tahtanın durumunu tutuyor. Başlangıçta tüm hücreler -1 olarak ayarlanmış.
winningPositions dizisi, kazanan kombinasyonları içeriyor. Oyunun kazanma koşullarını kontrol etmek için kullanılacak.
winner değişkeni, kazanan oyuncunun sembolünü tutuyor. Başlangıçta "X" olarak ayarlanmış.
onCreate metodu, aktivite oluşturulduğunda çağrılıyor ve görünümü ayarlıyor.
play metodu, bir hücreye tıklandığında çağrılıyor. Seçilen hücreyi işaretliyor ve oyun durumunu güncelliyor.
playAgain metodu, "Yeniden Oyna" düğmesine tıklandığında çağrılıyor. Oyunu sıfırlıyor ve yeni bir oyuna başlamak için görünümü yeniliyor.
Oyunun çalışma mantığı şu şekildedir:

Bir hücreye tıklandığında, play metodu çağrılır.
Seçilen hücre kontrol edilir, daha önce işaretlenmemişse devam edilir.
Seçilen hücre, şu anki oyuncunun sembolü ile işaretlenir.
Kazanma koşulları kontrol edilir. Eğer bir oyuncu kazanırsa, gameActive değişkeni false olarak ayarlanır ve kazanan oyuncu belirlenir. Kazanan oyuncu "X" veya "0" olarak winner değişkenine atanır.
Eğer tüm hücreler doldurulmuşsa ve bir kazanan yoksa, oyun berabere biter.
playAgain metodu çağrıldığında, oyun sıfırlanır ve yeni bir oyuna başlamak için görünüm güncellenir.
