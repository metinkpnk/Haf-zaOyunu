# Haf-zaOyunu
## Windows Forms hafıza oyun projenizi oluşturma
Hafıza oyunumuzu oluşturduğunuzda, ilk adım bir Windows Forms Uygulama projesi oluşturmaktır. <br/>
1-Visual Studio'yu açın. <br/>
2-Başlangıç penceresinde Yeni proje oluştur'u seçin. <br/>
3-Yeni proje oluştur penceresinde Windows Forms arayın. Ardından Tüm proje türleri listesinden Masaüstü'nü seçin. <br/>
4-C#  için Windows Forms Uygulama (.NET Framework) şablonunu ve ardından İleri'yi seçin.<br/>
5-Yeni projenizi yapılandırın penceresinde projenize HafızaOyunu adını verin ve Oluştur'u seçin.<br/>
Visual Studio uygulamanız için bir çözüm oluşturur. Çözüm, uygulamanızın ihtiyaç duyduğu tüm projeler ve dosyalar için bir kapsayıcıdır.<br/>

Bu noktada Visual Studio, Windows Form Tasarımcısı'nda boş bir form görüntüler.<br/>
## Oyununuz için düzen oluşturma
1-forma tıklayarak Windows Forms Tasarımcısı'nı seçin. Sekmede C# için Form1.cs [Tasarım] veya Visual Basic için Form1.vb [Tasarım] okunur. Özellikler penceresinde aşağıdaki form özelliklerini ayarlayın. <br/>
Form1 olan Text özelliğini Eşleşen Oyun olarak değiştirin. Bu metin oyun penceresinin en üstünde görünür. <br/>
Formun boyutunu ayarlayın. Bunu, Boyut özelliğini 550, 550 olarak ayarlayarak veya Visual Studio IDE'nin en altında doğru boyutu görene kadar formun köşesini sürükleyerek değiştirebilirsiniz.<br/>
2-IDE'nin sol tarafındaki Araç Kutusu sekmesini seçin. Bunu görmüyorsanız, menü çubuğundanAraç KutusunuGörüntüle'yi> veya CtrlAlt+X'i+ seçin.<br/>
3-Araç kutusundaki Kapsayıcılar kategorisinden bir TableLayoutPanel denetimi sürükleyin veya çift tıklayın. Özellikler penceresinde panel için aşağıdaki özellikleri ayarlayın.<br/>
*BackColor özelliğini CornflowerBlue olarak ayarlayın. Bu özelliği ayarlamak için BackColor özelliğinin yanındaki oku seçin. BackColor iletişim kutusunda Web'i seçin. Kullanılabilir renk adlarında CornflowerBlue öğesini seçin.<br/>
*Büyük ortadaki düğmeyi seçerek açılan listeden Dock özelliğini Fill olarak ayarlayın. Bu seçenek, tabloyu formun tamamını kapsayan şekilde yayar.<br/>
*CellBorderStyle özelliğini Inset olarak ayarlayın. Bu değer, panodaki her hücre arasında görsel kenarlıklar sağlar.<br/>
*Görev menüsünü görüntülemek için TableLayoutPanel'in sağ üst köşesindeki üçgen düğmesini seçin. Görev menüsünde Satır Ekle'yi iki kez seçerek iki satır daha ekleyin. Ardından iki sütun daha eklemek için Sütun Ekle'yi iki kez seçin.<br/>
*Görev menüsünde Satırları ve Sütunları Düzenle'yi seçerek Sütun ve Satır Stilleri penceresini açın. Her sütun için Yüzde seçeneğini belirleyin ve her sütunun genişliğini yüzde 25 olarak ayarlayın.<br/>
*Pencerenin en üstündeki listeden Satırlar'ı seçin ve her satırın yüksekliğini yüzde 25 olarak ayarlayın.<br/>
*İşiniz bittiğinde, değişikliklerinizi kaydetmek için Tamam'ı seçin.<br/>
TableLayoutPanel'iniz artık eşit boyutta 16 kare hücre içeren dörte dört bir kılavuzdur. Bu satırlar ve sütunlar simgelerin daha sonra görüntülendiği yerdir.<br/>
## Görüntülenecek etiketleri ekleme ve biçimlendirme
Bu bölümde, oyun sırasında görüntülenecek etiketleri oluşturacak ve biçimlendireceksiniz.<br/>
1-Form düzenleyicisinde TableLayoutPanel seçildiğinden emin olun. Özellikler penceresinin en üstünde tableLayoutPanel1 öğesini görmeniz gerekir. Seçili değilse formdaki TableLayoutPanel öğesini seçin veya Özellikler penceresinin üst kısmındaki listeden seçin.<br/>
2-Araç kutusunu daha önce olduğu gibi açın ve Ortak Denetimler kategorisini açın. TableLayoutPanel'in sol üst hücresine denetim Label ekleyin. Etiket denetimi artık IDE'de seçilidir. Bu öğe için aşağıdaki özellikleri ayarlayın.<br/>
*Etiketin BackColor özelliğini CornflowerBlue olarak ayarlayın.<br/>
*AutoSize özelliğini False olarak ayarlayın.<br/>
*Dock özelliğini Fill olarak ayarlayın.<br/>
*Özelliğin yanındaki açılan düğmeyi ve ardından ortadaki düğmeyi seçerek TextAlign özelliğini MiddleCenter olarak ayarlayın. Bu değer, simgenin hücrenin ortasında görünmesini sağlar.<br/>
*Font özelliğini seçin. Üç nokta (...) düğmesi görüntülenir. Üç noktayı seçin ve Yazı Tipi değerini Webdings, Yazı Tipi Stili'niKalın ve Boyut değerini 48 olarak ayarlayın.<br/>
*Etiketin Text özelliğini c harfine ayarlayın.<br/>
3-Etiket denetiminizi seçin ve TableLayoutPanel içindeki bir sonraki hücreye kopyalayın. Ctrl+C tuşlarını seçin veya menü çubuğundaKopyayıDüzenle'yi seçin>. Ardından Ctrl+V veya Yapıştır düzenle'yi> kullanarakyapıştırın.<br/>
TableLayoutPanel'in ikinci hücresinde ilk Etiketin bir kopyası görüntülenir. Yeniden yapıştırdığınızda üçüncü hücrede başka bir Etiket görüntülenir. Tüm hücreler doldurulana kadar Etiket denetimlerini yapıştırmaya devam edin.<br/>
Bu adım formunuzun düzenini tamamlar.<br/>
## Rastgele nesne ve simge listesi ekleme
Bu bölümde, oyun için eşleşen semboller kümesi oluşturacaksınız. Her simge, form üzerindeki TableLayoutPanel denetiminde rasgele iki hücreye eklenir.<br/>
İki nesne oluşturmak için deyimleri kullanırsınız new . birincisi TableLayoutPanel'deki hücreleri rastgele seçen bir Random nesnedir. İkinci nesne bir List<T> nesnedir. Rastgele seçilen simgeleri depolar.<br/>
  1-C# kullanıyorsanız Form1.cs'yi veya Visual Basic kullanıyorsanız Form1.vb'yi seçin. ArdındanKoduGörüntüle'yi> seçin. Alternatif olarak F7 tuşunu seçin veya Form1'e çift tıklayın. Visual Studio IDE, Form1 için kod modülünü görüntüler.<br/>
  
  Farklı öğe türlerini izlemek için liste nesnelerini kullanabilirsiniz. Bir liste; sayıları, doğru/yanlış değerlerini, metinleri veya diğer nesneleri barındırabilir. Eşleşen oyununuzda, liste nesnesinin TableLayoutPanel panelindeki her hücre için bir tane olacak şekilde 16 dize vardır. Her dize, etiketlerdeki simgelere karşılık gelen tek bir harftir. Bu karakterler Webdings yazı tipinde veri yolu, bisiklet ve diğerleri olarak görünür.<br/>
  ## Etiketlere olay işleyicileri ekleme
  Bu eşleşen oyunda, bir oyuncu gizli bir simgeyi, ardından ikinci bir simgeyi gösterir. Simgeler eşleşirse görünür olarak kalırlar. Aksi takdirde, her iki simge de yeniden gizlenir.<br/>
  Oyununuzun bu şekilde çalışmasını sağlamak için, seçilen etiketin rengini arka planla eşleşecek şekilde değiştiren bir Click olay işleyicisi ekleyin.<br/>
  1-Formu Windows Forms Tasarımcısı'nda açın. Form1.cs veya Form1.vb'yi ve ardından Tasarımcıyı Görüntüle'yi> seçin.<br/>
  2-İlk etiket denetimini seçip çift tıklayarak koda Buton_Click() adlı bir Click olay işleyicisi ekleyin.<br/>
  3-Ardından, diğer etiketlerin her birini seçerken Ctrl tuşunu basılı tutun. Her etiketin seçildiğinden emin olun.<br/>
  4-Özellikler penceresinde, aydınlatma cıvatası olan Olaylar düğmesini seçin. Tıklama olayı için kutudan label1_Click seçin.<br/>
  5Enter tuşuna basın. IDE, koda Buton_Click() adlı bir Click olay işleyicisi ekler. Tüm etiketleri seçtiğinizden, işleyici etiketlerin her birine bağlı olur.<br/>
  Zamanlayıcı kullanarak etiketleri değiştirmeyi sonraki derslerde yapacağız...



  
