# TED Talks English–Indonesian Dataset

## Deskripsi Task  
Dataset ini digunakan untuk **Machine Translation** (MT), yaitu menerjemahkan transkrip TED Talks dari bahasa Inggris (en) ke bahasa Indonesia (id) dan sebaliknya.

## Dataset  
- **Nama dataset**: SEACrowd TED En–Id  
- **Sumber asli**: Koleksi WIT³ (Web Inventory of Transcribed & Translated Talks)  
- **Link Hugging Face**: https://huggingface.co/datasets/SEACrowd/ted_en_id  
- **Repository IndoNLG**: https://github.com/IndoNLP/indonlg  
- **Versi**: 1.0.0 (rilis SEACrowd 2024.06.20)  
- **Lisensi**: Creative Commons Attribution-ShareAlike 4.0 International

## Statistik  
- **Bahasa**: English (en), Indonesian (id)  
- **Split**:  
  - `train`: 87406 (75%)  
  - `validation`: 2677 (10%)  
  - `test`: 3179 (15%)

## Cara Penggunaan
```python
# Menggunakan Hugging Face datasets
from datasets import load_dataset
dataset = load_dataset("SEACrowd/ted_en_id", trust_remote_code=True)
print(dataset)

# Menggunakan seacrowd library
import seacrowd as sc
dataset_sc = sc.load_dataset("ted_en_id", schema="seacrowd")
print(dataset_sc.keys())
```

## Contoh
English
When Ebola broke out in March 2014, Pardis Sabeti and her team set out to sequence the virus’s genome, to learn how it was mutating and spreading.
“We worked openly, we shared, and we collaborated,” Sabeti says.
“We don’t want the world to be defined by a virus, but by the unity of millions of hearts and minds.”

Indonesian
Ketika Ebola meletus pada Maret 2014, Pardis Sabeti dan timnya berusaha mengurutkan genom virus tersebut, untuk mempelajari bagaimana virus itu bermutasi dan menyebar.
“Kami bekerja terbuka, kami berbagi, dan kami berkolaborasi,” kata Sabeti.
“Kami tidak ingin dunia didefinisikan oleh sebuah virus, melainkan oleh persatuan jutaan hati dan pikiran.”
