<h3 align="center">
    <img src="https://github.com/niskala5570/jawi-keyboard/assets/34799053/f5eb4516-2457-4510-9d8b-552f17cd32f2" alt="Kekunci Jawi">
    <img src="https://readme-typing-svg.demolab.com?font=Reem+Kufi&size=30&pause=3000&color=F7F7F7&center=true&vCenter=true&random=true&width=435&lines=KEKUNCI+%E2%80%84JAWI;JAWI%E2%80%84KEYBOARD"/>
</h3><hr>

## NKL Jawi (QWERTY) - Windows

Sama seperti MNH48 tetapi sedikit penambahan.

### Pemasangan

Muat turun fail zip melalui [_Release_](https://github.com/niskala5570/jawi-keyboard/releases/tag/Kartika) atau seperti gambar di bawah dan ekstrak di folder pilihan.
Dwiketik setup.exe, berikan kebenaran admin bila diminta.

Selesai ^^

<details>
<summary>Gambar</summary>

![image](https://github.com/niskala5570/jawi-keyboard/assets/34799053/ced3220d-0286-4941-b37c-32e2eaedec68)
![image](https://github.com/niskala5570/jawi-keyboard/assets/34799053/f7946dbb-3670-4086-9922-6c5b0bf03ec2)

</details>

---

### Nyahpasang

Dwiketik setup.exe dan beri kebenaran admin bila diminta.
Pilih _Remove the keyboard layout_ dan ketik _finish_.

Selesai ^^
<details>
<summary>Gambar</summary>

![image](https://github.com/niskala5570/jawi-keyboard/assets/34799053/d7d847c9-9b19-4a22-8a64-f81decce8e74)

</details>

---


## NKL Jawi (QWERTY) - Linux (X11 XKB Symbols)
### Persediaan
Perlu diambil perhatian yang setiap sistem mungkin berbeza caranya. Walaupun memang namanya X11, tetapi Wayland boleh sahaja.

Dan ya, aku tahu semuanya boleh dibuat menggunakan terminal, tetapi aku malas menulis skrip dan aku malas menulis skrip.

Aku menggunakan Suasana Semeja K (_K Desktop Environment_; KDE) yang telah aku pasangakn FCITX5 (fai.tiks.faiv) kerana hendakkan _Mozc_ (kekunci Jepun spt. Google JP IME). Jadi tangkapan layar dan cara pemasangan mungkin berbeza untuk pengguna seperti Cinnamon ataupun GNOME.

1. Buka folder akar (_root_) kalian, dan pergi ke `usr/share/X11/xkb/`.
2. Akan ada dua folder yang kalian perlu buka iaitu `rules` dan juga `symbols`.
3. Buat salinan untuk fail `symbols/my` dan `rules/evdev.xml`. Jangan risau jika terpadam, aku ada, tetapi mungkin tidak sama. Sediakan payung sebelum hujan.

### Pemasangan
#### symbols/my

Akan ada dua peta kekunci, tambahkan peta kekunci yang ketiga. Boleh salin dan tampal sahaja dari fail (`ms`)[NKL Jawi (QWERTY) - Linux xkb symbols/symbols/my] ini.

Ketiga yang dimaksudkan:

```
partial alphanumeric_keys
xkb_symbols "jawiniskala"
{
    name[Group1] = "Malay (Jawi NISKALA, phonetic)";

*sampai habis*
```

#### rules/evdev.xml
Cari `<!-- Keyboard indicator for Malay layouts -->` kemudian salin dan tampal sahaja dari (`evdev.xml`)[NKL Jawi (QWERTY) - Linux xkb symbols/rules/evdev.xml].

Maka akan jadi seperti ini:

```
    <layout>
      <configItem>
        <name>my</name>
        <!-- Keyboard indicator for Malay layouts -->
        <shortDescription>ms</shortDescription>
        <description>Malay (Jawi, Arabic Keyboard)</description>
        <countryList>
          <iso3166Id>MY</iso3166Id>
        </countryList>
        <languageList>
          <iso639Id>ind</iso639Id>
          <iso639Id>msa</iso639Id>
          <iso639Id>min</iso639Id>
          <iso639Id>ace</iso639Id>
          <iso639Id>bjn</iso639Id>
          <iso639Id>tsg</iso639Id>
          <iso639Id>mfa</iso639Id>
        </languageList>
      </configItem>
      <variantList>
        <variant>
          <configItem>
            <name>phonetic</name>
            <description>Malay (Jawi, phonetic)</description>
          </configItem>
        </variant>
        <variant>
          <configItem>
            <name>jawiniskala</name>
            <description>Malay (Jawi NISKALA)</description>
          </configItem>
        </variant>
      </variantList>
    </layout>
```

#### Tetapan sistem
1. Fcitx

Buka tetapan sistem, cari `fcitx` / `input method` jika guna fcitx.

Tekan butang `add input method` dan cari nama `(Jawi NISKALA)`.

!()[NKL Jawi (QWERTY) - Linux xkb symbols/gambar/Screenshot_20250501_003515.png]

2. Biasa

Buka tetapan sistem, cari `keyboard`.

Kemudian tekan butang `Add layout` dan taip sahaja `Niskala`

!()[NKL Jawi (QWERTY) - Linux xkb symbols/gambar/Screenshot_20250501_004455.png]


#### Tetapkan kekunci pintas.

Jangan lupa tetapkan kekunci pintas untuk menukar antara Rumi dan Jawi. Aku gunakan `Meta(Win)` + `Spacebar` sama spt. Windows.

Walaupun aku gunakan fcitx, tetapan pintasan masih ada pada yang biasa (`keyboard`) melalui butang `Configure Switching`.

!()[NKL Jawi (QWERTY) - Linux xkb symbols/gambar/Screenshot_20250501_004730.png]


# Selesai! سلامت منجاوي!
---

### Soalan Mungkin Ditanya

<details>
<summary align=center><h4>Apple Macintosh? iPhone?</h4></summary>
Malangnya aku tak ada peranti tersebut untuk kaji buat atur letak sendiri.

- [Papan Huruf atau Keyboard Jawi di Mac - Akademi Jawi Malaysia](https://www.youtube.com/watch?v=1XeQuzrYQdU&t=62s)
- [Gunakan terbina atur letak terbina dalam iOS, cari Bahasa Melayu (Arab)](https://x.com/koleksijawi/status/1703638217608814818)

</details>
<details>
<summary align=center><h4>Linux?</h4></summary>
Kemaskini: Boleh guna pemetaan xkb yg aku sudah sediakan. Lihat cara pasang di atas.


Boleh lihat [FCITX Table Jawi oleh Jawi MNH](https://github.com/jawi-mnh48/fcitx-table-jawi), malangnya aku tak dapat mengesahkan kerana gagal membolehkan ia berfungsi di komputer aku. (arch btw).
Kedepannya aku akan cuba buat sendiri dengan [xremap](https://github.com/xremap/xremap) (mempunyai sokongan X11 dan Wayland).

</details>

<details>
<summary align=center><h4>Android?</h4></summary>

Aku ada cadang nak tambah pada [FlorisBoard](https://github.com/florisboard/florisboard), apapun boleh guna alternatif ini dahulu:
- [Kekunci Google](https://play.google.com/store/apps/details?id=com.google.android.inputmethod.latin&hl=en), pilih Bahasa Melayu (Arab). [Percuma] (Mirip QWERTY, kaf dan ga arab ك ڬ, bukan Jawi ک ݢ dan tiada ye ى)
- [Jawi Pro](https://play.google.com/store/apps/details?id=com.zairo.zairokeyboardpro&hl=en) [RM5.49] (Mempunyai atur letak QWERTY dan lain lagi)
- [Jawi / Arabic Keyboard](https://play.google.com/store/apps/details?id=com.gogo.nurul.keyboardjawi&pcampaignid=web_share) [Percuma]
- [Mobile Jawi](https://play.google.com/store/apps/details?id=com.murasu.mobilejawi&hl=en) [Percuma]
- [eJawiMakmur](https://play.google.com/store/apps/details?id=my.gov.muip.ejawi&hl=en) [Percuma] (Bukan kekunci tetapi penukar, dibangun oleh Majlis Adat Resam Melayu Pahang [MUIP])
- SwiftKeyboard dan Samsung Keyboard juga ada rasanya, tak pasti, cari Bahasa Melayu (Arab) dalamnya.
</details>

----

<details>
<summary align=center><h2> Pemetaan // Mapping </h2></summary>
<img src="https://github.com/niskala5570/jawi-keyboard/assets/34799053/95783848-d008-47c2-8f69-edd6a1f03b34"

![Shift_copy_1](https://github.com/niskala5570/jawi-keyboard/assets/34799053/5c3e3020-8642-4840-87bb-e6c40e20e377)
![Ctrl Alt](https://github.com/niskala5570/jawi-keyboard/assets/34799053/b70f8c8c-c418-4572-9f07-43a284bbe33d)
![Ctrl Alt Shift](https://github.com/niskala5570/jawi-keyboard/assets/34799053/acd36833-ee74-4ce4-b11b-1b1a39046620)

</details>

<details>
<summary align=center><h2> MNH48 Jawi (QWERTY) - Windows </h2></summary>

The directory contains the keyboard layout source file in `klc` format,
that is used in Microsoft Keyboard Layout Creator (MSKLC), as well as
the resulting compiled installation files and libraries, minus the
bootstrapper. Because the bootstrapper seemed to not be generated by
MSKLC but rather just copied over, it is technically copyrighted by
Microsoft and I cannot distribute it. The other files are actually
compiled and I have the copyrights on them, so I can distribute them.

You can also generate the files on your side from the source `klc`.
Install MSKLC from Microsoft's website, load the `klc` file, then click
`Project` and select `Build DLL and Setup Package`.

**For users who just want to install keyboard layout and not do anything
else, download the [latest release archive](https://github.com/jawi-mnh48/jawi-keyboard/releases/latest/download/mnh48-jawi-qwerty-windows.zip) and then open it, then
double click on `MNHjawi_amd64.msi` to install and you're done.**

If you cannot run `MNHjawi_amd64.msi`, for example, it gives you the
error: `Error message: The version of this file is not compatible with
the version of Windows you're running.`, then please run `MNHjawi_i386.msi`
instead because it means that your Windows or your processor doesn't
support amd64 instruction set. In rare cases such as on certain old
computers with Windows XP, even `MNHjawi_i386.msi` might not work and
you need `MNHjawi_ia64.msi` instead in those cases.

The files are built on Windows 10 and has been tested to be functioning
properly under Windows 10. The version of MSKLC used is 1.4.6000.2
released on 2nd October 2020. The Unicode data bundled was Unicode 5.0
but I've manually downloaded Unicode 13.0 data to use with MSKLC before
compiling, so the keyboard layout I generate has support for Unicode 13.0.


## License

All of the layout themselves, as in the character position arrangement, are
all released under The MIT license.

The license for the specific files varies from one another, check the
subsection for specific license.


### MNH48 Jawi (QWERTY) - Windows

I would actually want to release this as full featured open source, but
there might had been some violation with Microsoft's licensing terms.
If I read correctly, what it don't allow is the bundling of the keyboard
layout in paid software or selling the layout itself. You can still use
my files to install and modify as long as you abide with that terms.
Those terms were set by Microsoft, not me.
</details>
