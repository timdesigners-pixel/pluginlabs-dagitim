# PluginLabs · Dağıtım

PluginLabs uygulamalarının **Windows sürüm dosyaları**. Bu depo yalnız ikili dağıtım içindir; kaynak kod ilgili ürün depolarındadır. [PluginLabs Hub](https://github.com/timdesigners-pixel/PluginLabs) uygulamaları buradan indirir ve kurmadan önce SHA-256 değerini doğrular.

## Etiket biçimi
Her sürüm `<uygulama-kimliği>-v<sürüm>` etiketiyle yayımlanır (ör. `pluginlabs-scrapper-v0.4.0`). Hub güncelleme denetimi yalnız kendi önekine uyan etiketleri okur.

| Uygulama | Kimlik | Kaynak sürüm |
|---|---|---|
| Mind Palace | `mind-palace` | mind-palace |
| Leo Helper | `leo-helper` | leo-helper |
| PluginLabs Scrapper (PL-004) | `pluginlabs-scrapper` | the-ultimate-scrapper |

## Doğrulama
Her sürümde `SHA256SUMS.txt` bulunur. Dosyalar kaynak depodaki sürümle bayt bayt aynıdır. Paketler **imzasızdır**; Windows SmartScreen uyarı verebilir.

Yeni sürüm eklemek: kaynak depodaki sürüm dosyasını aynı adla, `<kimlik>-v<sürüm>` etiketiyle buraya yükleyin ve PluginLabs `src/catalog.cjs` kaydını güncelleyin.
