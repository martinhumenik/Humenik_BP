# Analýza dát z oblasti zákrytových premenných hviezd

## Martin Humeník - Bakalárska práca

### Hospodárska informatika, KKUI, FEI TUKE 2023

## Datasety

Vytvorenie datasetov:

-   Pre oddelené systémy: detached_curves_samples_knn.pkl,
    detached_curves_samples_svr.pkl - súbor
    [**data_det_curves_load.ipynb**](data_det_curves_load.ipynb)

-   Pre dotykové systémy: overcontact_curves_samples_knn.pkl,
    overcontact_curves_samples_svr.pkl - súbor
    [**data_over_curves_load.ipynb**](data_over_curves_load.ipynb)

-   Pôvodné dáta observačných kriviek - všetky súbory v priečinku
    [**krivky**](krivky)

-   Spracované observačné dáta: observed.csv - súbor
    [**data_obs.ipynb**](data_obs.ipynb)

-   [Link](https://mega.nz/file/AC8QxBrY#wWzDR-50neomCTYyusG-va5f3L62QfMsdqo43UJ80uY)
    pre stiahnutie súboru **det_curves_samples_knn.pkl**

-   [Link](https://mega.nz/file/UT8FFS5Y#v5UWzyBB2U0H5Gske4UuHNQbp6Ndsnx8kNSigt59mFs)
    pre stiahnutie súboru **det_curves_samples_svr.pkl**

-   [Link](https://mega.nz/file/EfkSgbYZ#1NbrIE0_bWP79l6SBERTyz40v9YX5QAI0yl2MkIDE5w)
    pre stiahnutie súboru **over_curves_samples_knn.pkl**

-   [Link](https://mega.nz/file/AC1GCRoS#4idS-JgYjv9fVZ3fe3vWPIrjFQHIuMvCxuBX9JexSSQ)
    pre stiahnutie súboru **over_curves_samples_svr.pkl**

## Zobrazenie svetelných kriviek

Vizualizácia syntetických a observačných svetelných kriviek

1.  súbor [**data_visualization.ipynb**](data_visualization.ipynb)

## Predikcie fyzikálnych parametrov binárnych systémov

Trénovanie, validácia a testovanie modelov, uloženie vytvorených
modelov.

Modelovanie metódou k-NN:

-   Predikcia vybraných fyzikálnych parametrov syntetických oddelených
    systémov - súbor
    [**knn_pred_det_syn.ipynb**](knn_pred_det_syn.ipynb)
-   Predikcia vybraných fyzikálnych parametrov syntetických dotykových
    systémov - súbor
    [**knn_pred_over_syn.ipynb**](knn_pred_over_syn.ipynb)
-   Predikcia vybraných fyzikálnych parametrov observačných oddelených
    systémov, vizualizácia výsledkov - súbor
    [**knn_pred_det_obs.ipynb**](knn_pred_det_obs.ipynb)
-   Predikcia vybraných fyzikálnych parametrov observačných dotykových
    systémov, vizualizácia výsledkov - súbor
    [**knn_pred_over_obs.ipynb**](knn_pred_over_obs.ipynb)

Modelovanie metódou SVR:

-   Predikcia vybraných fyzikálnych parametrov syntetických oddelených
    systémov - súbor
    [**svr_pred_det_syn.ipynb**](svr_pred_det_syn.ipynb)
-   Predikcia vybraných fyzikálnych parametrov syntetických dotykových
    systémov - súbor
    [**svr_pred_over_syn.ipynb**](svr_pred_over_syn.ipynb)
-   Predikcia vybraných fyzikálnych parametrov observačných oddelených
    systémov, vizualizácia výsledkov - súbor
    [**svr_pred_det_obs.ipynb**](svr_pred_det_obs.ipynb)
-   Predikcia vybraných fyzikálnych parametrov observačných dotykových
    systémov, vizualizácia výsledkov - súbor
    [**svr_pred_over_obs.ipynb**](svr_pred_over_obs.ipynb)

## Spracovanie predikovaných hodnôt - observačné svetelné krivky

Spojenie predikovaných a skutočných hodnôt fyzikálnych parametrov hodnôt
do csv súborov podľa kategórie binárneho systému a filtra danej
svetelnej krivky pre následné vykreslenie svetelných kriviek systémom
ELISa

-   Spracovanie predikovaných a skutočných hodnôt fyzikálnych
    parametrov- súbor
    [**process_data_for_plots.ipynb**](process_data_for_plots.ipynb)
-   Výsledné csv súbory sú v priečinku [**data_to_plot**](data_to_plot)
    rozdelené podľa použitej metódy

## Modely

Modely kontrolovaného učenia k-NN a SVR:

-   k-NN model pre predikciu fyzikálnych parametrov oddelených systémov
    trénovaný na svetelných krivkách bez pridaného šumu -
    [Link](https://mega.nz/file/pXkWDC4L#eQgXBWnFqoRqh9AT2fHdycp08hx3AxDbNoYGigkcmy4)
    na stiahnutie súboru
    [**knn_detached_model.pkl**](knn_detached_model.pkl)

-   k-NN model pre predikciu fyzikálnych parametrov oddelených systémov
    trénovaný na svetelných krivkách s pridaným šumom -
    [Link](https://mega.nz/file/Va8yzKID#-xoPkxe6eUZDuQIQQ8d0KYsVGUmc26LOAvBb9x9Ktng)
    na stiahnutie súboru
    [**knn_detached_noise_model.pkl**](knn_detached_noise_model.pkl)

-   k-NN model pre predikciu fyzikálnych parametrov dotykových systémov
    trénovaný na svetelných krivkách bez pridaného šumu -
    [Link](https://mega.nz/file/VGtCwIqQ#4qn7z00XS4PL7zsW8jqG9jBc3qrI2ahU-smPYSGg2G0)
    na stiahnutie súboru
    [**knn_overcontact_model.pkl**](knn_overcontact_model.pkl)

-   k-NN model pre predikciu fyzikálnych parametrov dotykových systémov
    trénovaný na svetelných krivkách s pridaným šumom -
    [Link](https://mega.nz/file/gLtBhBgY#Ir3qd3JJegR80WH4_RvjcjfK5nSM5HvaMl4F_K_jbdE)
    na stiahnutie súboru
    [**knn_overcontact_noise_model.pkl**](knn_overcontact_noise_model.pkl)

-   SVR model pre predikciu fyzikálnych parametrov oddelených systémov
    trénovaný na svetelných krivkách bez pridaného šumu -
    [Link](https://mega.nz/file/cHEDVCoY#FBQIuo_FDtstyrbGKdifqv-hNuGiZCucBvVYmoqxx-Q)
    na stiahnutie súboru
    [**svr_detached_model.pkl**](svr_detached_model.pkl)

-   SVR model pre predikciu fyzikálnych parametrov oddelených systémov
    trénovaný na svetelných krivkách s pridaným šumom -
    [Link](https://mega.nz/file/ZD8QTKjQ#P-KueHg-cmwbpy470awQdEyGMa_PUJxQQfSLTsY6Fy0)
    na stiahnutie súboru
    [**svr_detached_noise_model.pkl**](svr_detached_noise_model.pkl)

-   SVR model pre predikciu fyzikálnych parametrov dotykových systémov
    trénovaný na svetelných krivkách bez pridaného šumu -
    [Link](https://mega.nz/file/EflXHYyA#wmW3BJ9OquyX_KCRGKNkRgb9nZhngnYeMLeATJkqigA)
    na stiahnutie súboru
    [**svr_overcontact_model.pkl**](svr_overcontact_model.pkl)

-   SVR model pre predikciu fyzikálnych parametrov dotykových systémov
    trénovaný na svetelných krivkách s pridaným šumom -
    [Link](https://mega.nz/file/oPlz0BCJ#2kg6WSD6pM90h6l4htMnzBuOlCbjwAU7jsWZ247w0x0)
    na stiahnutie súboru
    [**svr_overcontact_noise_model.pkl**](svr_overcontact_noise_model.pkl)

## ELISa
Potrebné knižnice a postup, ako si pripraviť prostredie pre systém ELISa je opísaný na https://github.com/mikecokina/elisa.