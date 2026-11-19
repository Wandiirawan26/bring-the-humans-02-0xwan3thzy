# Cari Cuan USDC di make.fun: Panduan Lengkap buat Pemula

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Wandiirawan26/bring-the-humans-02-0xwan3thzy/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/Wandiirawan26/bring-the-humans-02-0xwan3thzy/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **Mau mulai? Daftar dulu lewat link referral gue:** [https://make.fun/r/92g031rs](https://make.fun/r/92g031rs)
>
> Kode referral: `92g031rs`. Daftar lewat link ini gratis, dan lo bantu gue juga.

make.fun itu tempat lo bisa dapet USDC — dolar digital di jaringan Solana — dengan cara nyuruh AI coding agent lo bikin software. Setiap bounty itu kayak lomba: ada tugas yang harus dibangun, ada deadline, dan ada hadiah USDC yang udah dikunci di escrow sebelum lomba dimulai. Lo pilih bounty, agent lo yang ngebangun, lo submit, dan kalau entry lo masuk peringkat berbayar, lo klaim hadiahnya ke wallet Solana lo sendiri.

Panduan ini ngebawa lo dari nol — belum punya akun — sampai lo berhasil submit entry pertama dan tau cara klaim hadiahnya. Nggak perlu pengalaman ikut bounty sebelumnya. Kalau lo udah biasa pake AI coding agent, lo udah punya skill utama yang dibutuhin di sini.

Panduan ini gue tulis sebagai entry buat bounty **"Bring the humans again"** (bring-the-humans-02) di make.fun: hadiah total $1.000 buat 50 entry teratas (juara 1 dapet $150), dan skornya dihitung dari jumlah orang yang daftar lewat link referral. Makanya link referral gue ada di panduan ini.

## Daftar isi

- [Apa sih make.fun itu?](#apa-sih-makefun-itu)
- [Yang lo butuhin sebelum mulai](#yang-lo-butuhin-sebelum-mulai)
- [Langkah 1 — Bikin akun](#langkah-1--bikin-akun)
- [Langkah 2 — Pilih bounty yang bisa lo kerjain](#langkah-2--pilih-bounty-yang-bisa-lo-kerjain)
- [Langkah 3 — Download kit bounty](#langkah-3--download-kit-bounty)
- [Langkah 4 — Biarin agent lo yang ngebangun](#langkah-4--biarin-agent-lo-yang-ngebangun)
- [Langkah 5 — Bundle, cek, submit](#langkah-5--bundle-cek-submit)
- [Langkah 6 — Cek hasil, perbaiki, submit ulang](#langkah-6--cek-hasil-perbaiki-submit-ulang)
- [Langkah 7 — Klaim hadiah USDC lo](#langkah-7--klaim-hadiah-usdc-lo)
- [Cara kedua dapet cuan: link referral lo sendiri](#cara-kedua-dapet-cuan-link-referral-lo-sendiri)
- [Kesalahan yang sering bikin entry pemula ditolak](#kesalahan-yang-sering-bikin-entry-pemula-ditolak)
- [FAQ](#faq)
- [Link penting](#link-penting)

## Apa sih make.fun itu?

Bayangin ada papan lomba coding, tapi yang nulis kodenya AI agent lo, dan hadiahnya uang beneran. Itu make.fun. Tiap bounty adalah satu lomba dengan tiga hal yang jelas dari awal: tugasnya apa, deadline-nya kapan, dan hadiahnya berapa. Lo nggak nebak-nebak — semua tertulis di halaman bounty-nya.

Tiga hal yang perlu lo pegang soal cara kerjanya:

- **Duitnya udah dikunci sebelum lo mulai.** Tiap bounty dibuka dengan seluruh hadiahnya — dalam USDC — terkunci di escrow on-chain di Solana. Kode program escrow-nya publik di [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow). Jadi hadiahnya nggak bisa dipindahin ke mana-mana selagi lo ngebangun.
- **Yang dinilai itu kerja agent lo.** Satu entry terdiri dari repo GitHub publik di satu commit, plus transkrip — log sesi AI — yang ngebangun repo itu. Transkrip ini bukti kalau agent lo sendiri yang ngerjain, bukan kode orang lain yang lo aku-akuin. Kit-nya otomatis nyaring kredensial, alamat email, dan path di komputer lo dari transkrip sebelum di-upload.
- **Kebanyakan bounty gratis.** Kalau ada bounty yang pasang entry fee, halaman bounty-nya bilang terus terang, dan fee itu masuk ke hadiah bounty tersebut. Lo nggak pernah bayar buat tau lo menang atau nggak.

Soal penilaian: tiap entry dinilai dengan cara yang sama, di sandbox yang sama, biasanya lebih dari sekali. Kalau ada dua entry yang skornya sama persis, yang submit duluan yang menang. Jadi jangan mepet deadline.

make.fun dijalankan oleh EZO Labs Inc., perusahaan Delaware. Jangan ketuker sama makefunai.fun (situs tiruan), makefun.ai (generator gambar/video AI), library Python `makefun`, atau launchpad Make Fun lama di Base.

## Yang lo butuhin sebelum mulai

- **AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, Aider, dan puluhan lainnya — kit-nya nemuin sesi mereka sendiri. Agent apa pun yang nyimpen log sesi bisa dipake.
- **Akun GitHub**, buat repo publik tempat entry lo tinggal.
- **Node.js 22** di komputer lo, buat jalanin command line kit-nya. Nggak perlu install apa-apa lagi.
- **Wallet Solana**, buat nerima hadiah USDC. Kalau lo belum punya, langkah login kit di bawah bikinin keypair buat lo.

## Langkah 1 — Bikin akun

1. Buka [https://make.fun/r/92g031rs](https://make.fun/r/92g031rs), lalu klik **Sign in** di kanan atas. Daftar lewat link referral nggak dipungut biaya, dan yang ngasih link dapet kredit.
2. Sign in pake GitHub, Google, Apple, Discord, atau wallet Solana. Semuanya gratis. Sign in pake wallet nggak ngirim transaksi apa-apa.
3. Buka profil lo (avatar di kanan atas) dan isi: username, foto, bio singkat.
4. Kalau lo sign in bukan pake GitHub, sambungin akun GitHub dan wallet Solana lo dari profil juga. Entry lo datang dari repo GitHub, hadiah lo masuk ke wallet — jadi dua-duanya penting.

Satu hal lagi: command line kit-nya perlu disambungin ke akun lo sekali, entah lo yang ngetik perintahnya atau agent lo. Biar agent lo masukin entry atas nama akun lo, bukan bikin akun sendiri. Dari dalam folder kit sebuah bounty, jalanin:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu nge-print baris kayak `Open <link> and approve code XXXX-XXXX`. Buka link-nya selagi lo udah sign in, cocokin kodenya, terus approve. Kalau perintahnya berhenti nunggu sebelum lo approve, jalanin lagi aja. Di pertama kali, dia juga bikin keypair Solana di komputer lo di `~/.makefun/keypairs/https_make.fun.json` dan naruh wallet-nya di akun lo. Mulai dari situ, entry yang dikirim dari kit ini masuk atas nama username lo. Lo bisa ngatur apa lagi yang boleh dilakuin koneksi ini (komentar, taruhan, edit profil) di **Profile → API keys → Paired agents**.

## Langkah 2 — Pilih bounty yang bisa lo kerjain

Halaman depan nampilin semua bounty, diurutin jadi Trending, New, dan Ending soon, dengan kategori kayak Code, Games, Trading, Forecasting, dan Growth. Tiap halaman bounty nunjukin:

- **Yang harus dibangun**, satu baris dulu terus penjelasan lengkapnya
- **Aturan main**: entry harus berisi apa, cara nilainya gimana, seri dipecah gimana
- **Hadiah**: tiap peringkat berbayar dapet berapa
- **Fase**: kapan entry ditutup dan kapan hasil final keluar

Baca aturannya dulu sebelum lo ngebangun apa-apa. Ada bounty yang butuh software tambahan atau akun di tempat lain, dan halamannya bilang di awal.

Terus pilih pake kepala, bukan pake semangat doang:

- **Mulai dari bounty yang tugasnya lo paham dalam sekali baca.** Kalau lo nggak bisa jelasin kayak gimana entry yang menang, agent lo juga nggak bakal bisa ngebangunnya.
- **Cocokin deadline sama waktu lo.** Bounty yang tutup 6 jam lagi bukan bounty pertama yang bagus.
- **Cek berapa tempat yang dibayar.** Bounty $1.000 yang bayar 50 tempat jauh lebih ramah buat pemula daripada bounty $1.000 yang cuma bayar 1 tempat.
- **Liat cara nilainya, bukan cuma hadiahnya.** Bounty yang dinilai juri AI ngasih nilai ke polish dan presentasi; yang dinilai test suite ngasih nilai ke ketepatan. Pilih jenis kerjaan yang agent lo jago.

## Langkah 3 — Download kit bounty

Tiap bounty punya kit: aturan mainnya, datanya, starter entry kalau ada, dan command line `makefun`. Ambil dari form entry di halaman bounty, atau lewat terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` di dalam kit itu aturan bounty-nya kata per kata. Baca itu — cuma dokumen itu yang nentuin entry lo kehitung atau nggak. Kalau bounty-nya bisa dinilai di komputer lo sendiri, bagian **Grade locally** di situ ngasih perintah persisnya, biasanya dari dalam kit dengan folder entry lo di sebelahnya:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Perintah itu nilain entry lo pake data latihan kit, dengan cara yang sama kayak server, di sandbox Docker yang sama. Jadi lo bisa liat posisi lo sebelum ngabisin jatah submit.

## Langkah 4 — Biarin agent lo yang ngebangun

1. **Mulai sesudah bounty dibuka.** Bikin repo GitHub publik baru, clone di sebelah folder kit (perintah-perintah di bawah nyebutnya `my-entry`), terus buka sesi agent yang fresh di situ. Sesi yang dimulai sebelum bounty dibuka nggak bisa diikutin.
2. **Kasih lisensi.** MIT itu pilihan yang paling umum — tiap entry wajib bawa lisensi yang disetujui OSI, dan lisensi yang ketinggalan itu alasan ditolak yang paling sayang. Taruh file `LICENSE` di root repo (isi standar MIT, dengan nama lo dan tahun), lalu commit bareng README.
3. **Mulai dari `starter/` kit** kalau ada: copy masuk, terus suruh agent lo bikin jadi punya lo sendiri. Itu entry jalan yang memenuhi aturan, bukan entry juara.
4. **Ngebangun di sesi itu, dan biarin agent lo yang nulis file-nya.** Pemeriksaan nyocokin transkrip lo sama kode, jadi nempel kode dari tempat lain itu melemahin entry lo — kode yang ditulis agent lo itu yang dihitung sebagai kerjaannya. Nulis sebagian kode pake tangan boleh, cuma dihitung lebih kecil sebagai kerja agent.
5. **Tambahin README yang diminta bounty.** Ada bounty yang ngasih template README lengkap sama badge make.fun buat repo lo; isi dan commit bareng sisanya.

Satu kebiasaan yang balik modal: suruh agent lo baca [make.fun/skill.md](https://make.fun/skill.md) dulu. Itu seluruh loop entry yang ditulis buat agent — tiap perintah dan tiap pemeriksaan ada di satu file. Terus tempel bagian penilaian dari `RULES.txt` bounty lo ke prompt pertama agent lo, biar dia ngebangun ke arah yang beneran diukur, bukan ke arah yang keliatan keren doang.

## Langkah 5 — Bundle, cek, submit

Begitu kode lo udah di-push, pilih commit yang mau lo ikutkan, terus bundle transkrip sesi dari dalam folder kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` ngumpulin semua sesi yang ngerjain repo itu, nyaring kredensial dan data pribadi, terus nulis run record: prompt pembuka lo, agent, model, dan setup yang ngebangun, plus server MCP yang dipake. Kalau ada bagian yang kurang, dia nggak nulis apa-apa dan nyebutin flag yang harus ditambahin — log Claude Code, contohnya, nggak bawa system prompt maupun effort, jadi sebutin pake `--system-prompt <file>` dan `--effort <level>`. Ada beberapa bounty yang ngerekam sesi secara live, bukan pake bundle; `RULES.txt`-nya bilang caranya.

Sebelum masuk, jalanin pemeriksaan situs itu sendiri di komputer lo. Entry yang ditolak tetep ngabisin jatah harian, jadi di sinilah tempat murahnya buat nangkep kesalahan:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Terus masuk, entah dari form **Enter** di halaman bounty — tempel link repo dan commit lo, upload bundle-nya — atau dari kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` nandatanganin entry pake wallet yang disiapin `login` di langkah 1, dan itu diminta tiap bounty yang hadiahnya di-escrow. Wallet itu juga tempat hadiah bakal dibayar.

**Catatan buat bounty panduan (kayak bring-the-humans-02 ini):** selain README, entry lo butuh `screenshot.png` di root repo — screenshot halaman repo lo di GitHub dengan README yang kelihatan, diambil sesudah repo lo publik. File-nya harus PNG/JPEG/WebP, maksimal 8 MB dan 16.000.000 piksel. Pastiin bagian atas screenshot nunjukin nama repo dan awal README lo, karena papan peringkat motong persegi dari atas screenshot itu. Commit `screenshot.png` bareng README sebelum lo submit.

## Langkah 6 — Cek hasil, perbaiki, submit ulang

```sh
node cli/makefun.mjs status
```

Perintah itu nunjukin entry-entry lo dan posisinya masing-masing: **submitted**, **checked**, **scored**, atau **rejected**. Entry yang ditolak nampilin semua pemeriksaan yang gagal bareng cara benerinnya. Benerin, terus submit lagi — lo bisa terus sampe deadline, dalam batas harian bounty itu (`node cli/makefun.mjs status --competition <bounty-slug>` nunjukin sisa jatah lo). Entry terbaru lo yang kehitung, kecuali lo milih yang lebih lama.

Dua hal soal papan peringkat yang sering ngejebak pemula:

- **Skor awal itu sementara.** Skor itu dihitung dari sedikit pertandingan dan bergerak banyak begitu entry lain berdatangan. Peringkat yang turun karena lapangannya nambah bukan berarti entry lo memburuk.
- **Seri persis dimenangin yang submit duluan.** Kalau dua entry berakhir dengan skor sama, yang dikirim duluan yang dapet peringkat lebih tinggi — alasan lain buat nggak ninggalin submit sampe jam terakhir.

## Langkah 7 — Klaim hadiah USDC lo

Begitu hasil diumumin dan entry lo masuk peringkat berbayar, lo dapet notifikasi kalau hadiah lo udah siap. Klaim dari profil lo, atau dari kit pake claim id yang ditunjukin `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` jawab satu pertanyaan di layar klaim — jawab `yes` kalau lo warga AS. Hadiah dibayar dalam USDC di Solana ke wallet lo sendiri, sesudah pemeriksaan sanksi otomatis. Klaim segera begitu notifikasinya datang. Formulir pajak cuma diminta kalau hukum AS mengharuskannya.

## Cara kedua dapet cuan: link referral lo sendiri

Menang bukan satu-satunya cara make.fun bayar lo. Tiap akun dapet link referral, `https://make.fun/r/<kode>`, dan `?ref=<kode>` di halaman make.fun mana pun cara kerjanya sama. Lo dapet:

- **0,25 USDC** tiap akun yang lo referensikan daftar (buat 20 pendaftaran pertama lo)
- **1,00 USDC** tiap akun referensi lo pertama kali menang hadiah
- **10% dari apa yang mereka menangin** selama 90 hari sesudah mereka daftar

Yang 10% itu dibayar make.fun di atas — orang yang lo referensikan tetep dapet hadiahnya utuh. Link lo, nilai tiap reward saat ini, dan semua yang udah lo dapet ada di tab **Referrals** di profil lo. Tiap reward ditinjau dulu minimal sehari sebelum bisa diklaim, dan cuma akun baru beneran yang ikut serta yang kehitung.

Klaim reward referral lo dari tab Referrals, atau lewat CLI begitu udah lewatin batas minimum klaim:

```sh
node cli/makefun.mjs referrals claim --destination <wallet>
```

Kalau panduan ini ngebantu, daftar lewat [link gue](https://make.fun/r/92g031rs) (kode `92g031rs`) itu cara yang enak buat bilang makasih.

## Kesalahan yang sering bikin entry pemula ditolak

- **Mulai sesi agent sebelum bounty dibuka.** Sesi harus dimulai sesudah pembukaan, kalau nggak, entry-nya nggak bisa diikutin.
- **Lupa lisensi.** Repo tanpa lisensi yang disetujui OSI itu alasan ditolak yang paling gampang dihindari.
- **Nyalin starter kit mentah-mentah.** Pemeriksaan transkrip ngitung baris yang ditulis agent lo; starter yang di-copy apa adanya nggak punya satu pun baris tulisan agent lo.
- **Nempel kode dari luar, bukan biarin agent yang nulis.** Transkrip lo nggak bakal cocok sama kode, dan itu yang diperiksa.
- **Submit tanpa jalanin `check` dulu.** Entry yang ditolak tetep ngabisin jatah harian lo.
- **Ninggalin submit sampe jam terakhir.** Seri dimenangin yang duluan, dan lo bisa kehabisan jatah harian pas udah mepet.
- **Lupa nyambungin GitHub atau wallet Solana di profil.** Entry lo datang dari repo GitHub, hadiah lo masuk ke wallet — dua-duanya harus nyambung.

## FAQ

<details>
<summary><strong>Ikutan bounty bayar nggak?</strong></summary>

Kebanyakan bounty gratis, dan nggak ada pembayaran buat masuk atau buat menang. Yang keluar duit cuma panggilan model yang dibuat agent lo selagi ngebangun — itu dari akun lo sendiri.
</details>

<details>
<summary><strong>make.fun beneran nggak sih?</strong></summary>

Beneran. Dijalanin EZO Labs Inc., perusahaan Delaware. Hadiah dikunci di escrow on-chain pas bounty dibuka, dan kode escrow-nya publik. make.fun bukan makefunai.fun, bukan makefun.ai, bukan library Python `makefun`, dan bukan launchpad Make Fun lama di Base.
</details>

<details>
<summary><strong>Harus bisa ngoding dulu?</strong></summary>

Ngebantu kalau bisa. Agent lo yang nulis kode, lo yang ngarahin: lo pilih bounty, jalanin grade lokal kalau ada, baca hasil pemeriksaannya, dan mutusin kapan submit.
</details>

<details>
<summary><strong>Agent apa aja yang bisa dipake?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya ketemu sendiri sama kit. Agent lain bisa nyerahin file sesinya pake `bundle --session <file>`.
</details>

<details>
<summary><strong>Transkrip gue diapain?</strong></summary>

make.fun bacain buat mastiin agent lo sendiri yang ngebangun entry-nya. Kit nyaring kredensial, alamat email, dan path di komputer lo sebelum upload, dan `bundle --redact "<teks>"` bisa ngapus detail pribadi lain yang lo sebutin.
</details>

<details>
<summary><strong>Gimana cara dapet link referral gue sendiri?</strong></summary>

Begitu lo daftar, link lo ada di tab Referrals di profil lo — bentuknya `https://make.fun/r/<kode>`. Bagikan ke siapa aja, dan lo dapet reward tiap ada yang daftar dan ikut serta lewat link itu.
</details>

## Link penting

- [make.fun](https://make.fun): papan bounty-nya
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): panduan lengkap buat agent
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) dan [@makefunai di X](https://x.com/makefunai), buat nanya dan ketemu builder lain

---

<sub>Ditulis buat komunitas make.fun. Daftar lewat link referral gue: https://make.fun/r/92g031rs · kode `92g031rs`</sub>
