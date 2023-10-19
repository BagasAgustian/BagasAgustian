# POLYGLOT SIRI APPLE

PolyglotSiri didasarkan pada ChatGPT-Siri dan meningkatkan kemampuan multibahasa dan kemampuan bicara.
Sekarang Anda dapat berbicara dengan siri dengan bahasa apa pun. Dan siri merespons dua bahasa (Inggris dan Mandarin seperti yang saya tetapkan) dengan suara yang lebih alami. Sekarang Anda dapat memperlakukan Siri sebagai teman asing dan berlatih pelatihan bahasa dengannya.

Selain API chat GPT Open AI, Tiga API REST lainnya digunakan:

- OpenAI Whisper API: digunakan sebagai layanan STT yang dapat menangani banyak bahasa. Siri asli hanya dapat memahami satu bahasa dalam satu waktu.
- Azure Language Cognitive API: digunakan untuk mengenali bahasa teks untuk konfigurasi bahasa Azure TTS selanjutnya.
- Azure TTS: menggunakan Azure TTS untuk menggantikan TTS asli iOS, sehingga menghasilkan suara yang terdengar lebih alami.

  # Shortchut Link
https://www.icloud.com/shortcuts/9bd65fdaf1714ce09f862253d3324086

# Configuration and Customization
0. Anda harus mendaftar untuk openai api dan Azure cloud
- Masuk ke OpenAI, https://platform.openai.com
- Masuk ke Azure, https://portal.azure.com/
- Di Azure cloud, dua sumber daya yang dibutuhkan, ucapan dan bahasa. Depoly mereka.
1. Isi kunci api Anda di pintasan ini.
- Anda membutuhkan dua kunci openai, satu untuk berbisik dan yang lainnya untuk penyelesaian.
- Isi Azure tts dan Kunci layanan kognitif bahasa Azure.
2. Gantikan url REST API layanan Azure. Ada tiga di antaranya, satu untuk kognisi bahasa teks, dan dua untuk Azure TTS (bertujuan untuk dukungan suara bilingual, Anda dapat menyesuaikan lebih banyak untuk beberapa bahasa).
3. Menyesuaikan parameter Azure TTS.
- Pengaturan bahasa dan suara, di badan permintaan TTS, sesuaikan pengaturan bahasa dan vocie Anda. Temukan semua vocie di sini, https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/language-support?tabs=tts#supported-languages
- Di header permintaan TTS, Anda dapat menentukan kualitas output audio "X-Microsoft-OutputFormat". Temukan semua output audio di sini, https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/rest-text-to-speech?tabs=streaming#audio-outputs
4.Tentukan pernyataan if mulit-bahasa
- Untuk membuat azure TTS mendukung multi-bahasa vocie, kita perlu menggunakan kognisi bahasa Azure untuk mengenali bahasa teks.
  
# Usage
1. Download the shortcut. https://www.icloud.com/shortcuts/9bd65fdaf1714ce09f862253d3324086
2. Cukup ketuk Shortcut dan biarkan keajaiban terjadi.
3. Rekaman audio akan berhenti setelah 15 detik secara default. Anda dapat menghentikannya dengan mengetuk atau menunggu hitungan mundur berakhir.
4. Tunggu jawaban.

# Acknowledge
https://github.com/Yue-Yang/ChatGPT-Siri
