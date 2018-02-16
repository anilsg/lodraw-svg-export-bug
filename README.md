# lodraw-svg-export-bug
LibreOffice Draw SVG Export Bug demonstration file

## LibreOffice Draw
- Version: 5.4.5.1
- Build ID: 5.4.5-1
- CPU threads: 4; OS: Linux 4.15; UI render: default; VCL: gtk3; Locale: en-AU (en_AU.UTF-8); Calc: group

## ArchLinux
- Linux 4.15.3-1-ARCH #1 SMP PREEMPT Mon Feb 12 23:01:17 UTC 2018 x86_64 GNU/Linux

## Report
https://bugs.documentfoundation.org/show_bug.cgi?id=115777

### Actual Results
SVG image is nothing like the actual image in LODraw. Vectors are relocated catastrophically: https://github.com/anilsg/lodraw-svg-export-bug/blob/master/disk.svg

### Expected Results
The expected SVG image should be like the PDF export, which is produced correctly: https://github.com/anilsg/lodraw-svg-export-bug/blob/master/disk.pdf

### Reproduce
1. Open this file: https://github.com/anilsg/lodraw-svg-export-bug/blob/master/disk.odg
2. Observe correct view of the image is rendered in LO Draw.
3. Export to PDF and observe correct view is retained when viewed in PDF viewer.
4. Export to SVG and when viewed in any viewer such as gpicview notice image corrupted.
