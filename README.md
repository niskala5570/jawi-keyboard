<h3 align="center">
    <img src="https://github.com/niskala5570/jawi-keyboard/assets/34799053/f5eb4516-2457-4510-9d8b-552f17cd32f2" alt="Kekunci Jawi">
    <img src="https://readme-typing-svg.demolab.com?font=Reem+Kufi&size=30&pause=3000&color=F7F7F7&center=true&vCenter=true&random=true&width=435&lines=KEKUNCI+%E2%80%84JAWI;JAWI%E2%80%84KEYBOARD"/>
</h3><hr>

## NKL Jawi (QWERTY) - Windows

Sama seperti MNH48 tetapi sedikit penambahan.

### Pemasangan

Muat turun fail zip dan ekstrak di folder pilihan.
Buka folder NKL Jawi (QWERTY) - Windows.
Klik pada Jawi_NKL_amd64.msi, tunggu sehingga selesai.

<details>
<summary>Gambar</summary>

![image](https://github.com/niskala5570/jawi-keyboard/assets/34799053/ced3220d-0286-4941-b37c-32e2eaedec68)

</details>

---

### Nyahpasang

Buka *control panel* , *programs and features*, cari Jawi NKL(QWERTY)

<details>
<summary>Gambar</summary>

![image](https://github.com/niskala5570/jawi-keyboard/assets/34799053/e4a980c4-438b-4669-a641-0f2ca66c5099)

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
