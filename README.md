# Sürücüsüz Metro Simülasyonu (Rota Optimizasyonu)

Bu proje, bir metro ağı içerisinde:
- İki istasyon arasındaki **en hızlı rotayı**,
- **En az aktarmalı rotayı** bulan bir simülasyon geliştirmeyi hedefler.

Kullanıcılar, metro ağını modelleyerek farklı başlangıç ve bitiş noktaları arasındaki en iyi rotayı belirleyebilir. Proje, algoritmik düşünme becerilerini geliştirmek ve gerçek dünya problemlerine çözüm sunmak için tasarlanmıştır.

---

## 🚀 Proje Amacı

Projenin temel hedefleri:
1. Metro ağını **Graf veri yapısı** ile modellemek.
2. **BFS Algoritması** (Breadth-First Search) kullanarak en az aktarmalı rotayı bulmak.
3. **A* Algoritması** ile en hızlı rotayı hesaplamak.
4. Algoritmik düşünme ve gerçek dünya problemleri için etkin çözümler geliştirmek.

---

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler

### Programlama Dili:
- Python

### Kütüphaneler:
- **collections**: BFS algoritması için kuyruk yapısının oluşturulmasında kullanıldı.
- **heapq**: A* algoritması için öncelik kuyruğu oluşturulmasında kullanıldı.
- **networkx** ve **matplotlib**: Metro ağını görselleştirmek için kullanıldı.

---

## 📜 Algoritmaların Çalışma Mantığı

### BFS Algoritması:
- BFS (Breadth-First Search), bir graf üzerinde düğümleri seviyeler halinde araştırır.
- En az aktarmalı rotayı bulmak için, önce başlangıç noktası ve tüm komşuları ziyaret edilir. Daha sonra hedefe ulaşana kadar yeni komşular eklenir.
- Veri yapısı: Kuyruk (`deque`).

### A* Algoritması:
- A* algoritması, belirli bir hedefe en kısa yoldan ulaşmayı hedefler.
- Öncelikli olarak en düşük maliyetli rotalar seçilerek arama yapılır.
- Veri yapısı: Öncelik kuyruğu (`heapq`).
- Performansı artırmak için heuristik (örneğin, düz hat mesafesi) eklenebilir.

---

## 📊 Örnek Kullanım ve Test Senaryoları

### Örnek Test:
1. **AŞTİ'den OSB'ye:**
   - En az aktarmalı rota: AŞTİ -> Kızılay -> Ulus -> Demetevler -> OSB
   - En hızlı rota (25 dakika): AŞTİ -> Kızılay -> Ulus -> Demetevler -> OSB

2. **Batıkent'ten Keçiören'e:**
   - En az aktarmalı rota: Batıkent -> Demetevler -> Gar -> Keçiören
   - En hızlı rota (21 dakika): Batıkent -> Demetevler -> Gar -> Keçiören

3. **Keçiören'den AŞTİ'ye:**
   - En az aktarmalı rota: Keçiören -> Gar -> Sıhhiye -> Kızılay -> AŞTİ
   - En hızlı rota (19 dakika): Keçiören -> Gar -> Sıhhiye -> Kızılay -> AŞTİ

---

## 🌟 Projeyi Geliştirme Fikirleri

Projeyi daha etkileyici hale getirmek için aşağıdaki geliştirmeler yapılabilir:
1. **Heuristik Eklenmesi (A*):** Algoritmaya tahmin (heuristik) ekleyerek performansı artırabilirsiniz.
2. **Grafiksel Arayüz:** Kullanıcıların metro ağını görselleştirebileceği bir arayüz eklenebilir.
3. **Gerçek Zamanlı Veri Entegrasyonu:** Metro trafiği ve yoğun saatleri simüle etmek için dinamik veriler eklenebilir.
4. **Sesli Komut:** Kullanıcıların sesli komutlarla rota sorgulamasına olanak sağlayabilirsiniz.

---

## 📂 GitHub'da Paylaşma

Bu projeyi GitHub üzerinde paylaşmak için aşağıdaki adımları izleyebilirsiniz:
1. Yeni bir GitHub repository oluşturun.
2. Repository'yi "Public" olarak ayarlayın.
3. Kodunuzu ve README.md dosyanızı yükleyin.
4. Açıklayıcı commit mesajları yazın.

---

## 💡 Faydalı Kaynaklar

### BFS Algoritması:
- [GeeksForGeeks](https://www.geeksforgeeks.org/breadth-first-search-or-bfs-for-a-graph/)
- [YouTube Video](https://www.youtube.com/watch?v=oDqjPvD54Ss)

### A* Algoritması:
- [RedBlobGames](https://www.redblobgames.com/pathfinding/a-star/introduction.html)
- [GeeksForGeeks](https://www.geeksforgeeks.org/a-search-algorithm/)
