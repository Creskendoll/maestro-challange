# maestro-challange
Maestro platformu örnek proje.

Sizden beklentimiz bu projeyi kendi reponuza klonlamanız ve onun üstünde çalışmanızdır. İşiniz bittiğinde bize kendi reponuzun linkini ve sitenin host edildiği adresi atmalısınız.

## Giriş
Bu proje `create-react-app` kullanılarak yapılandırılmıştır. Daha çok bilgi için [Github reposuna](https://github.com/facebook/create-react-app) göz atabilirsiniz.

Projeyi Firebase'e bağlamanız beklenmektedir. Daha fazla bilgi için [Firebase dokümantasyonuna](https://firebase.google.com/docs/web/setup) göz atabilirsiniz.

İhtiyacınız olan komutlar aşağıdaki gibidir:

### `yarn start` veya `npm start`
Projeyi geliştirme modunda açacaktır. [http://localhost:3000](http://localhost:3000) adresine girerek görüntüleyebilirsiniz.

Kod üstünde değişiklik yaptığınızda sayfa otomatik olarak yenilenecektir. Ayrıca hataları konsolda görüntüleyebilirsiniz.

### `yarn build` veya `npm run build`
Projeyi derleyerek `build` adında bir klasör yaratacaktır. Firebase ile deploy ettiğinizde bu klasörün içerikleri host edilecektir.


## Proje Gerekçeleri
Sizden beklentimiz Firestore veritabanına bağlı bir TODO uygulaması geliştirmenizdir. Kullanıcı bir `TextField` kullanarak TODO başlığı girebilmeli ve Enter tuşu veya bir butona basarak listeye ekleyebilmelidir.

TODO girdi bilgileri Firestore üstünde saklanmalı ve her kullanıcıya aynı içerik gösterilmelidir.

Her bir TODO girdisinde başlıklari ve ne zaman listeye eklendikleri görüntülenmelidir. Kullanıcı her girdinin sağ tarafında bulunan sil tuşu ile bir uyarıyı onayladıktan sonra gidiyi silebilmelidir.

Kullanıcı girişi olmadığı için TODO girdileri herkes tarafından görüntülenebilmelidir.

Arayüz tasarımı tamamıyla size kalmış. Gerekçeler sağlandığı sürece tasarım o kadar önemli değil. İşlevselliğe daha çok zaman ayırmanızı tavsiye ederiz.

### [Firebase](https://firebase.google.com) Entegrasyonu
Proje arka planda Firebase kullanmalıdır. Veriler Firestore'da saklanmalı ve hosting Firebase üstünden sağlanmalıdır. Uygulamanız Firebase hostingin sağladığı varsayılan domain üstünde çalışmalıdır. 

Örnek: https://my-todo.web.app/

### [Material UI](https://material-ui.com) Kullanımı
Uygulama içi UI elemanları için [Material UI Komponentleri](https://material-ui.com/getting-started/installation/) kullanılmalıdır. Bu kütüphaneyi kullanmak haricinde görselliğe çok önem vermeseniz de olur.

### [React Hooks](https://reactjs.org/docs/hooks-intro.html) Kullanımı
Sıkı bir gerekçe olmasa da state management hooks kullanılarak yapılmalıdır.