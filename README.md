# Scene Text Recognition Resources

[<p align='right'>Author: 陈晓雪</p>](https://github.com/CCchenxiaoxue)

## Updates

Dec 24, 2019: added 20 papers and the C-SVT dataset, and updated corresponding tables. You can download the new [Excel](https://pan.baidu.com/s/1CvyMGm3a5KzPNOpK8Fs5gA) prepared by us. (Password: teqv)

***

<!-- MarkdownTOC -->

- [1. Datasets](#1-datasets)
    - [1.1 Regular Scene Text Datasets](#11-regular-scene-text-datasets)
    - [1.2 Irregular Scene Text Datasets](#12-irregular-scene-text-datasets)
 	- [1.3 Bilingual Scene Text Datasets \(mainly in Chinese and English\)](#13-bilingual-scene-text-datasets-mainly-in-chinese-and-english)
    - [1.4 Synthetic Datasets](#14-synthetic-datasets)
    - [1.5 Comparison of Datasets](#15-comparison-of-datasets)
- [2. Summary of Scene Text Recognition Results](#2-summary-of-scene-text-recognition-results)
    - [2.1 Comparison of methods](#21-comparison-of-methods)
    - [2.2 Recognition Results](#22-recognition-results)
        - [2.2.1 Recognition Results on Regular Dataset](#221-recognition-results-on-regular-dataset)
        - [2.2.2 Recognition Results on Irregular Dataset](#222-recognition-results-on-irregular-dataset)
        - [2.2.3 Recognition Results on Bilingual Scene Text Dataset](#223-recognition-results-on-bilingual-scene-text-dataset)
- [3. Survey](#3-field-survey)
- [4. OCR Service](#4-ocr-service)
- [5. References](#5-references)
- [6. Help](#6help)
- [7. Copyright](#7copyright)

<!-- /MarkdownTOC -->

<a id="1-datasets"></a>

## 1. Datasets

<a id="11-regular-scene-text-datasets"></a>

### 1.1 Regular Scene Text Datasets

- IIIT5K[31]：
  * **Introduction:** It contains 5,000 images in total, 2,000 for training and 3,000 for testing. Every image is associated with a  50-word lexicon and a 1000-word lexicon. The lexicon consists of a  ground truth and some randomly picked words.
  * **Link:** [IIIT5K-download](http://cvit.iiit.ac.in/research/projects/cvit-projects/the-iiit-5k-word-dataset)
- SVT[1]：
  * **Introduction:** It contains 647 cropped word images. Many images are severely corrupted by noise, blur, and low resolution. SVT was collected from the Google Street View, and every image is associated with a 50-word lexicon. Specifically, it only provides word-level annotations.
  * **Link:** [SVT-download](http://vision.ucsd.edu/~kai/svt/)
- ICDAR 2003(IC03)[33]：
  * **Introduction:** It contains 509 images in total, 258 for training and 251 for testing. Specifically, it contains 867 cropped word images after discarding images that contain non-alphanumeric characters or those have less than three characters. Every image is associated with a 50-word lexicon and a full-word lexicon.  The full lexicon combines all lexicon words.
  * **Link:** [IC03-download](http://www.iapr-tc11.org/mediawiki/index.php?title=ICDAR_2003_Robust_Reading_Competitions)
- ICDAR 2013(IC13)[34]：
  * **Introduction:** It contains 1,015 cropped word images and inherits most of its samples from IC03. No lexicon is associated with this dataset.
  * **Link:** [IC13-download](http://dagdata.cvc.uab.es/icdar2013competition/?ch=2&com=downloads)
- COCO-Text[38]：
  - **Introduction:** It contains 63,686 images in total. Specifically, it contains 145,859  cropped word images for testing, including handwritten and printed, clear and blur, English and non-English.
  - **Link:** [COCO-Text-download](https://vision.cornell.edu/se3/coco-text-2/)
- SVHN[45]：
  * **Introduction:** It contains more than 600,000 digits of house numbers in natural scenes. The images were collected from the Google View images, and were used to digit recognition.
  * **Link:** [SVHN-download](http://ufldl.stanford.edu/housenumbers/)

<a id="12-irregular-scene-text-datasets"></a>
### 1.2 Irregular Scene Text Datasets

- SVT-P[35]：
  - **Introduction:** It contains 639 cropped word images for testing. Images were selected from the side-view angle snapshots in Google Street View. Therefore, most images are heavily distorted by the non-frontal view angle. Every image is associated with a 50-word lexicon and a full-word lexicon.
  - **Link:** [SVT-P-download](https://pan.baidu.com/s/1rhYUn1mIo8OZQEGUZ9Nmrg )  \(Password : vnis)
- CUTE80[36]：
  - **Introduction:** It contains 80 high-resolution images taken in natural scenes. Specifically, it contains 288 cropped word images for testing. The dataset focuses on curved text. No lexicon is provided.
  - **Link:** [CUTE80-download](http://cs-chan.com/downloads_CUTE80_dataset.html)
- ICDAR 2015(IC15)[37]：
  - **Introduction:** It contains 1,500 images in total, 1,000 for training and 500 for testing. Specifically, it contains 2,077 cropped images including more than 200 irregular text. No lexicon is associated with this dataset.
  - **Link:** [IC15-download](http://rrc.cvc.uab.es/?ch=4&com=downloads)
- Total-Text[39]：
  - **Introduction:** It contains 1,555 images in total. Specifically, it contains 11,459  cropped word images with more than three different text orientations: horizontal, multi-oriented and curved.
  - **Link:** [Total-Text-download](https://github.com/cs-chan/Total-Text-Dataset)

<a id="13-bilingual-scene-text-datasets-mainly-in-chinese-and-english"></a>
### 1.3 Bilingual Scene Text Datasets (mainly in Chinese and English)

- RCTW-17(RCTW competition，ICDAR17)[40]：
  - **Introduction:** It contains 12,514 images in total, 11,514 for training and 1,000 for testing. Images in RCTW-17 were mostly collected by camera or mobile phone, and others were generated images. Text instances are annotated with parallelograms. It is the first large scale Chinese dataset, and was also the largest published one by then.
  - **Link:** [RCTW-17-download](http://rctw.vlrlab.net/dataset/)
- MTWI(competition)[41]：
  - **Introduction:** It contains 20,000 images. The dataset mainly consists of Chinese or English web text. The competition includes three tasks: web text recognition, web text detection and end-to-end web text detection and recognition.
  - **Link:** [MTWI-download ](https://pan.baidu.com/s/1SUODaOzV7YOPkrun0xSz6A#list/path=%2F)  \(Password:gox9)
- CTW[42]：
  - **Introduction:** It contains 32,285 high resolution street view images of Chinese text, with 1,018,402 character instances in total. All images are annotated at the character level, including its underlying character type, bounding box, and 6 other attributes. These attributes indicate whether its background is complex, whether it’s raised, whether it’s hand-written or printed, whether it’s occluded, whether it’s distorted, whether it uses word-art.
  - **Link:** [CTW-download](https://ctwdataset.github.io/)
- SCUT-CTW1500[43]：
  - **Introduction:** It contains 1,500 images in total, 1,000 for training and 500 for testing. Specifically, it contains 10,751 cropped word images for testing. Annotations in SCUT-CTW1500 are polygons with 14 vertexes. The dataset mainly consists of Chinese and English.
  - **Link:** [SCUT-CTW1500-download](https://github.com/Yuliang-Liu/Curve-Text-Detector)
* LSVT(LSVT competition, ICDAR2019)[57]:
  * **Introduction:** It contains 20,000 testing data, 30,000 training data in full annotations and 400,000 training data in weak annotations, which are referred to as partial labels. For most of the training data in weak labels, only one transcription per image is provided.  All the images were captured from streets, which consist of a large variety of complicated real-world scenarios, e.g., store fronts and landmarks.
  * **Link:** [LSVT-download](https://rrc.cvc.uab.es/?ch=16&com=downloads)
* ArT(ArT competition, ICDAR2019)[58]:
  * **Introduction:** It contains 10,166 images in total, 5,603 for training and 4,563 for testing. ArT is a combination of Total-Text, SCUT-CTW1500 and Baidu Curved Scene Text, which were collected with the motive of introducing the arbitrary-shaped text problem to the scene text community.  The ArT dataset was collected with text shape diversity, hence all existing text shapes (i.e. horizontal, multi-oriented, and curved) have high number of existence in the dataset.
  * **Link:** [ArT-download](https://rrc.cvc.uab.es/?ch=16&com=downloads)
* ReCTS(ReCTS competition, ICDAR2019)[59]:
  * **Introduction:** A practical and challenging multi-orientation natural scene text dataset (ReCTS) was collected with 25,000 images, which consist of lots of signboards. In the dataset, all text lines and characters are labeled with locations and character codes.
  * **Link:** [ReCTS-download](https://rrc.cvc.uab.es/?ch=16&com=downloads)
* Chinese Street View Text(C-SVT) [63]:
  * **Introduction:** It contains more than 430,000 street view images in total, including 30,000 fully annotated images with locations and text labels for the regions and 400,000 more images in which only the annotations of the text-of-interest are given.  It is the largest one compared with existing Chinese text reading datasets.
  <!-- * **Link:** No publicly available resources. -->

<a id="14-synthetic-datasets"></a>

### 1.4 Synthetic Datasets

* Synth90k [53] : 
  * **Introduction:** It contains 8 million cropped word images generated from a set of 90k common English words. Words are rendered onto natural images with random transformations and effects. Every image is annotated with a ground-truth word.
  * **Link:** [Synth90k-download](http://www.robots.ox.ac.uk/~vgg/data/text/)
* SynthText [54] : 
  * **Introduction:** It contains 6 million cropped word images. The generation process is similar to that of Synth90k.
  * **Link:** [SynthText-download](https://github.com/ankush-me/SynthText)

<a id="15-comparison-of-datasets"></a>
### 1.5 Comparison of Datasets

<body>
<table cellspacing="0" border="0">
  <colgroup span="15" width="85"></colgroup>
  <tr>
    <td colspan=15 height="20" align="center"><b>Comparison of Datasets</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Datasets&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Language</td>
    <td colspan=6 align="center">Images</td>
    <td colspan=4 align="center">Lexicon</td>
    <td colspan=2 align="center">Label</td>
    <td rowspan=2 align="center">Type</td>
  </tr>
  <tr>
    <td align="center">Pictures</td>
    <td align="center">Instances</td>
    <td align="center">Training Pictures</td>
    <td align="center">Training Instances</td>
    <td align="center">Testing Pictures</td>
    <td align="center">Testing Instances</td>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">1k</td>
    <td align="center">Full</td>
    <td align="center">None</td>
    <td align="center">Char</td>
    <td align="center">Word</td>
    </tr>
  <tr>
    <td height="20" align="center">IIIT5K[31]</td>
    <td align="center">English</td>
    <td align="center" sdval="1120" sdnum="2052;">1120</td>
    <td align="center" sdval="5000" sdnum="2052;">5000</td>
    <td align="center" sdval="380" sdnum="2052;">380</td>
    <td align="center" sdval="2000" sdnum="2052;">2000</td>
    <td align="center" sdval="740" sdnum="2052;">740</td>
    <td align="center" sdval="3000" sdnum="2052;">3000</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SVT[32]</td>
    <td align="center">English</td>
    <td align="center" sdval="350" sdnum="2052;">350</td>
    <td align="center" sdval="725" sdnum="2052;">725</td>
    <td align="center" sdval="100" sdnum="2052;">100</td>
    <td align="center" sdval="211" sdnum="2052;">211</td>
    <td align="center" sdval="250" sdnum="2052;">250</td>
    <td align="center" sdval="514" sdnum="2052;">514</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">IC03[33]</td>
    <td align="center">English</td>
    <td align="center" sdval="509" sdnum="2052;">509</td>
    <td align="center" sdval="2268" sdnum="2052;">2268</td>
    <td align="center" sdval="258" sdnum="2052;">258</td>
    <td align="center" sdval="1157" sdnum="2052;">1157</td>
    <td align="center" sdval="251" sdnum="2052;">251</td>
    <td align="center" sdval="1111" sdnum="2052;">1111</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">IC13[34]</td>
    <td align="center">English</td>
    <td align="center" sdval="561" sdnum="2052;">561</td>
    <td align="center" sdval="5003" sdnum="2052;">5003</td>
    <td align="center" sdval="420" sdnum="2052;">420</td>
    <td align="center" sdval="3564" sdnum="2052;">3564</td>
    <td align="center" sdval="141" sdnum="2052;">141</td>
    <td align="center" sdval="1439" sdnum="2052;">1439</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">COCO-Text[38]</td>
    <td align="center">English</td>
    <td align="center" sdval="63686" sdnum="2052;">63686</td>
    <td align="center" sdval="145859" sdnum="2052;">145859</td>
    <td align="center" sdval="43686" sdnum="2052;">43686</td>
    <td align="center" sdval="118309" sdnum="2052;">118309</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center" sdval="27550" sdnum="2052;">27550</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SVHN[45]</td>
    <td align="center">Digits</td>
    <td align="center" sdval="600000" sdnum="2052;">600000</td>
    <td align="center" sdval="600000" sdnum="2052;">600000</td>
    <td align="center" sdval="573968" sdnum="2052;">573968</td>
    <td align="center" sdval="573968" sdnum="2052;">573968</td>
    <td align="center" sdval="26032" sdnum="2052;">26032</td>
    <td align="center" sdval="26032" sdnum="2052;">26032</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SVT-P[35]</td>
    <td align="center">English</td>
    <td align="center" sdval="238" sdnum="2052;">238</td>
    <td align="center" sdval="639" sdnum="2052;">639</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="238" sdnum="2052;">238</td>
    <td align="center" sdval="639" sdnum="2052;">639</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">CUTE80[36]</td>
    <td align="center">English</td>
    <td align="center" sdval="80" sdnum="2052;">80</td>
    <td align="center" sdval="288" sdnum="2052;">288</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="80" sdnum="2052;">80</td>
    <td align="center" sdval="288" sdnum="2052;">288</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">IC15[37]</td>
    <td align="center">English</td>
    <td align="center" sdval="1500" sdnum="2052;">1500</td>
    <td align="center">-</td>
    <td align="center" sdval="1000" sdnum="2052;">1000</td>
    <td align="center">-</td>
    <td align="center" sdval="500" sdnum="2052;">500</td>
    <td align="center" sdval="2077" sdnum="2052;">2077</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">Total-Text[39]</td>
    <td align="center">English</td>
    <td align="center" sdval="1555" sdnum="2052;">1555</td>
    <td align="center" sdval="11459" sdnum="2052;">11459</td>
    <td align="center" sdval="1255" sdnum="2052;">1255</td>
    <td align="center">-</td>
    <td align="center" sdval="300" sdnum="2052;">300</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">RCTW-17[40]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="12514" sdnum="2052;">12514</td>
    <td align="center">-</td>
    <td align="center" sdval="11514" sdnum="2052;">11514</td>
    <td align="center">-</td>
    <td align="center" sdval="1000" sdnum="2052;">1000</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">MTWI[41]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="20000" sdnum="2052;">20000</td>
    <td align="center">-</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center">-</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">CTW[42]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="32285" sdnum="2052;">32285</td>
    <td align="center" sdval="1018402" sdnum="2052;">1018402</td>
    <td align="center" sdval="25887" sdnum="2052;">25887</td>
    <td align="center" sdval="812872" sdnum="2052;">812872</td>
    <td align="center" sdval="3269" sdnum="2052;">3269</td>
    <td align="center" sdval="103519" sdnum="2052;">103519</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SCUT-CTW1500[43]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="1500" sdnum="2052;">1500</td>
    <td align="center" sdval="10751" sdnum="2052;">10751</td>
    <td align="center" sdval="1000" sdnum="2052;">1000</td>
    <td align="center">-</td>
    <td align="center" sdval="500" sdnum="2052;">500</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">LSVT[57]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="450000" sdnum="2052;">450000</td>
    <td align="center">-</td>
    <td align="center" sdval="30000" sdnum="2052;">30000</td>
    <td align="center">-</td>
    <td align="center" sdval="20000" sdnum="2052;">20000</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">ArT[58]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="10166" sdnum="2052;">10166</td>
    <td align="center">-</td>
    <td align="center" sdval="5603" sdnum="2052;">5603</td>
    <td align="center">-</td>
    <td align="center" sdval="4563" sdnum="2052;">4563</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">ReCTS[59]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="25000" sdnum="2052;">25000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">Synth90k[53]</td>
    <td align="center">English</td>
    <td align="center" sdval="8000000" sdnum="2052;">8000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SynthText[54]</td>
    <td align="center">English</td>
    <td align="center" sdval="6000000" sdnum="2052;">6000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">C-SVT(full annotations)[63]</td>
    <td align="center">Chinese</td>
    <td align="center" sdval="29966" sdnum="2052;">29966</td>
    <td align="center" sdval="908305" sdnum="2052;">908305</td>
    <td align="center" sdval="20157" sdnum="2052;">20157</td>
    <td align="center" sdval="620368" sdnum="2052;">620368</td>
    <td align="center" sdval="4841" sdnum="2052;">4841</td>
    <td align="center" sdval="143849" sdnum="2052;">143849</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
</table>

***

<a id="2-summary-of-scene-text-recognition-results"></a>
## 2. Summary of Scene Text Recognition Results

<a id="21-comparison-of-methods"></a>
### 2.1 Comparison of methods

It is notable that 1) "Reg" stands for regular scene text datasets. 2) "Irreg" stands for irregular scene text datasets. 3) "Seg" denotes the method based on segmentation. 4) "Extra" means the method uses the extra datasets in addition to Synth90k and SynthText. 5) "CTC" represents the method applies the CTC-based algorithm to decode. 6) "Attn" represents the method applies the attention mechanism to decode.

You can also download the new [Excel](https://pan.baidu.com/s/1CvyMGm3a5KzPNOpK8Fs5gA) prepared by us. (Password: teqv)

<body>
<table cellspacing="0" border="0">
  <colgroup span="11" width="85"></colgroup>
  <tr>
    <td colspan=11 height="20" align="center"><b>Comparison of methods</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Code</td>
    <td rowspan=2 align="center">Regular</td>
    <td rowspan=2 align="center">Irregular</td>
    <td rowspan=2 align="center">Segmentation</td>
    <td rowspan=2 align="center">Extra data</td>
    <td rowspan=2 align="center">CTC</td>
    <td rowspan=2 align="center">Attention</td>
    <td rowspan=2 align="center">Source</td>
    <td rowspan=2 align="center">Time</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Highlight&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : ABBYY</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
    <td align="center">A state-of-the-art text detector + a leading commercial OCR engine</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : SYNTH+PLEX</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
    <td align="center">The baseline of scene text recognition.</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [2]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
    <td align="center">1) Incorporating higher order statistical language models to recognize words in an unconstrained manner. 2) Introducing IIIT5K-word dataset.</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [3]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
    <td align="center">CNNs + Non-maximal suppression + beam search</td>
  </tr>
  <tr>
    <td height="20" align="center">Goel et al. [4] : wDTW</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
    <td align="center">Recognizing the text in the image by matching the scene and synthetic image features with wDTW.</td>
  </tr>
  <tr>
    <td height="20" align="center">Bissacco et al. [5] : PhotoOCR</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
    <td align="center">Applying a network with five hidden layers for character classification.</td>
  </tr>
  <tr>
    <td height="20" align="center">Phan et al. [6]</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
    <td align="center">1) MSER + SIFT descriptors + SVM 2) Introducing the SVT-P datasets.</td>
  </tr>
  <tr>
    <td height="20" align="center">Alsharif et al. [7] : HMM/Maxout</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">Convolutional Maxout networks + Hybrid HMM</td>
  </tr>
  <tr>
    <td height="20" align="center">Almazan et al [8] : KCSR</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">Embedding word images and text string in a common vectorial subspace and allowing one to cast recognition and retrieval tasks as a nearest neighbor problem.</td>
  </tr>
  <tr>
    <td height="20" align="center">Yao et al. [9] : Strokelets</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">Proposing a novel multi-scale representation for scene text recognition: strokelets.</td>
  </tr>
  <tr>
    <td height="20" align="center">R.-Serrano et al.[10] : Label embedding</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">Embedding word labels and word images into a common Euclidean space and finding the cloest word label in this space.</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [11]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">1) Enabling efficient feature sharing for text detection and classification. 2) Making technical changes over the traditional CNN architectures. 3) Proposing a method of automated data mining of Flickr.</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [12]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ACCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">HOG + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Gordo[13] : Mid-features</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">Proposing to learn local mid-level features suitable for building word image representations.</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [14]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">1) Treating each word as a category and training very large convolutional neural networks to perform word recognition on the whole proposal region. 2) Generating 9 million images, with equal numbers of word samples from a 90k word dictionary.</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [15]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">CNN + CRF</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi, Bai, and Yao [16] : CRNN</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">CNN + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [17] : RARE</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">STN + CNN + Attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Lee and Osindero [18] : R2AM</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">Presenting recursive recurrent neural networks with attention modeling.</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [19] : STAR-Net</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">STN + ResNet + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [78]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">integrating the CNN and WFST classification model</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [77]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">CVIU</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">character detection (HOG/CNN + SVM +Sliding window) + CRF, combining bottom-up cues from character detections and top-down cues from lexicon.</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [76]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">PR</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">HOG(different scale) + BLSTM + CTC (ensemble)</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [20]</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">IJCAI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">1) CNN + 2D-Attention-based RNN, applying an auxiliary dense character detection task that helps to learn text specific visual patterns. 2) Developing a large-scale synthetic dataset.</td>
  </tr>
  <tr>
    <td height="20" align="center">Yin et al. [21]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">CNN + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[66] : GRCNN</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">Gated Recurrent Convulution Layer + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">*Cheng et al. [22] : FAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">1) Proposing the concept of attention drift. 2)Introducing focusing network to focus deviated attention back on the target areas.</td>
  </tr>
  <tr>
    <td height="20" align="center">Cheng et al. [23] : AON</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">1) Extracting scene text features in four directions. 2)CNN + Attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [24]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">Attentional ResNet + CNN + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [25] : Char-Net</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">CNN + STN (facilitating the rectification of individual characters) + LSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al.  [26] : SqueezedText</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">Binary convolutional encoder-decoder network + Bi-RNN</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhan et al.[73]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">CRNN, achieving verisimilar scene text image synthesis by combining three novel designs including semantic coherence, visual attention and adaptive text appearance.</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bai et al. [27] : EP</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">Proposing edit probability to effectively handle the misalignment between the training text and the output probability distribution sequence.</td>
  </tr>
  <tr>
    <td height="20" align="center">Fang et al.[74]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">MultiMedia</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">ResNet + [2D Attentional CNN, CNN-based language module]</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.[75] : EnEsCTC</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">proposing a novel maximum entropy based regularization for CTC(EnCTC) and an entropy-based pruning method(EsCTC) to effectively reduce the space of the feasible set.</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [28]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">Designing a multi-task network with an encoder-discriminator-generator architecture to guide the feature of the original image toward that of the clean image.</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[61] : MAAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICFHR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">ResNet + BLSTM + Memory-Augmented Attentional Decoder</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [29]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">Attentional DenseNet + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [30] : ASTER</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">TPS + ResNet + Bidirectional attention-based BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : ASTER + AEG</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">TPS + ResNet + Bidirectional attention-based BLSTM + AEG</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [46] : MORAN</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Multi-object rectification network + CNN + Attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [61] : MORAN-v2</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Multi-object rectification network + ResNet + Attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : MORAN-v2 + AEG</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Multi-object rectification network + ResNet + Attentional BLSTM + AEG</td>
  </tr>
  <tr>
    <td height="20" align="center">Xie et al. [47] : CAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ACM</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet + CNN + GLU</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al.[48] : CA-FCN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Performing character classification at each pixel location and needing character-level annotations.</td>
  </tr>
  <tr>
    <td height="20" align="center">*Li et al. [49] : SAR</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet + 2D Attentional LSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhan el at. [55]: ESIR</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Iterative rectification Network + ResNet + Attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [56]: SSDAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Attentional CNN + GAS + GRU</td>
  </tr>
  <tr>
    <td height="20" align="center">Yang et al. [62]: ScRN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Symmetry-constrained Rectification Network + ResNet + BLSTM + Attentional GRU</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [64]: GCAM</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICME</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Convolutional Block Attention Module (CBAM) + ResNet + BLSTM + the proposed Gated Cascade Attention Module (GCAM)</td>
  </tr>
  <tr>
    <td height="20" align="center">Jeonghun et al. [65]</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">TPS + ResNet + BLSTM + Attentional Mechanism</td>
  </tr>
  <tr>
    <td height="20" align="center">Huang et al. [67] : EPAN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">learning to sample features from the text region of 2D feature maps, and innovatively introducing a two-stage attention mechanism</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [68]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Attentional DenseNET + 4-layer CNN + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Qi et al. [69] : CCL</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet + [CTC, CCL]</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [70] : ReELFA</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">VGG + Attentional LSTM, utilizing one-hot encoded coordinates to indicate the spatial relationship of pixels and character center masks to help focus attention on the right feature areas.</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhu et al. [71] : HATN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet50 + Hierarchical Attention Mechanism (Transformer structure)</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhan et al. [72] : SF-GAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet50 + Attentional Decoder, synthesising realistic scene text image for training better recognition models.</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : SAM</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Spatial attentional module (SAM)</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : seg-SAM</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Character segmentation module + Spatial attention module (SAM)</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [80] : DAN</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">decoupling the decoder of the traditional attention mechanism into a convolutional alignment module and a decoupled text decoder</td>
  </tr>
</table>

<a id="22-recognition-results"></a>
### 2.2 Recognition Results

In this section, we list the results on different scene text recognition benchmarks, including IIIT5K，SVT，IC03，IC13，SVT-P，CUTE80，IC15，RCTW-17, MWTI, CTW，SCUT-CTW1500, LSVT, ArT and ReCTS.

It is notable that 1) The '*' indicates the methods use the extra datasets in addition to Synth90k and SynthText. 2) The **bold** represents the best recognition results. 3) '^' denotes the best recognition results of using the extra datasets. 4) '@' represents the methods under different evaluation which only uses 1811 test images. 5) 'SK', 'ST', 'ExPu', 'ExPr' and 'Un' indicates the methods use Synth90K, SynthText, Extra Public Data, Extra Private Data and unknown data, respectively. 6) 'D_A' means data augmentation.

<a id="221-recognition-results-on-regular-dataset"></a>
#### 2.2.1 Recognition Results on Regular Dataset

<body>
<table cellspacing="0" border="0">
  <colgroup span="14" width="85"></colgroup>
  <tr>
    <td colspan=14 height="20" align="center"><b>Recognition Results on Regular Dataset</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td colspan=3 align="center">IIIT5K</td>
    <td colspan=2 align="center">SVT</td>
    <td colspan=4 align="center">IC03</td>
    <td align="center">IC13</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Source</td>
    <td rowspan=2 align="center">Time</td>
  </tr>
  <tr>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">1K</td>
    <td align="center">None</td>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">None</td>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">Full</td>
    <td align="center">50k</td>
    <td align="center">None</td>
    <td align="center">None</td>
    </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : ABBYY</td>
    <td align="center" sdval="24.3" sdnum="2052;">24.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="35" sdnum="2052;">35</td>
    <td align="center">-</td>
    <td align="center" sdval="56" sdnum="2052;">56</td>
    <td align="center" sdval="55" sdnum="2052;">55</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : SYNTH+PLEX</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="57" sdnum="2052;">57</td>
    <td align="center">-</td>
    <td align="center" sdval="76" sdnum="2052;">76</td>
    <td align="center" sdval="62" sdnum="2052;">62</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [2]</td>
    <td align="center" sdval="64.1" sdnum="2052;">64.1</td>
    <td align="center" sdval="57.5" sdnum="2052;">57.5</td>
    <td align="center">-</td>
    <td align="center" sdval="73.2" sdnum="2052;">73.2</td>
    <td align="center">-</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center" sdval="67.8" sdnum="2052;">67.8</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [3]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="70" sdnum="2052;">70</td>
    <td align="center">-</td>
    <td align="center" sdval="90" sdnum="2052;">90</td>
    <td align="center" sdval="84" sdnum="2052;">84</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Goel et al. [4] : wDTW</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="77.3" sdnum="2052;">77.3</td>
    <td align="center">-</td>
    <td align="center" sdval="89.7" sdnum="2052;">89.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Bissacco et al. [5] : PhotoOCR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="90.4" sdnum="2052;">90.4</td>
    <td align="center" sdval="78" sdnum="2052;">78</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="87.6" sdnum="2052;">87.6</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Phan et al. [6]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.7" sdnum="2052;">73.7</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Alsharif et al. [7] : HMM/Maxout</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="74.3" sdnum="2052;">74.3</td>
    <td align="center">-</td>
    <td align="center" sdval="93.1" sdnum="2052;">93.1</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center" sdval="85.1" sdnum="2052;">85.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Almazan et al [8] : KCSR</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center" sdval="75.6" sdnum="2052;">75.6</td>
    <td align="center">-</td>
    <td align="center" sdval="87" sdnum="2052;">87</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Yao et al. [9] : Strokelets</td>
    <td align="center" sdval="80.2" sdnum="2052;">80.2</td>
    <td align="center" sdval="69.3" sdnum="2052;">69.3</td>
    <td align="center">-</td>
    <td align="center" sdval="75.9" sdnum="2052;">75.9</td>
    <td align="center">-</td>
    <td align="center" sdval="88.5" sdnum="2052;">88.5</td>
    <td align="center" sdval="80.3" sdnum="2052;">80.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">R.-Serrano et al.[10] : Label embedding</td>
    <td align="center" sdval="76.1" sdnum="2052;">76.1</td>
    <td align="center" sdval="57.4" sdnum="2052;">57.4</td>
    <td align="center">-</td>
    <td align="center" sdval="70" sdnum="2052;">70</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [11]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="86.1" sdnum="2052;">86.1</td>
    <td align="center">-</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="91.5" sdnum="2052;">91.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [12]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83" sdnum="2052;">83</td>
    <td align="center">-</td>
    <td align="center" sdval="92" sdnum="2052;">92</td>
    <td align="center" sdval="82" sdnum="2052;">82</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ACCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Gordo[13] : Mid-features</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center" sdval="86.6" sdnum="2052;">86.6</td>
    <td align="center">-</td>
    <td align="center" sdval="91.8" sdnum="2052;">91.8</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [14]</td>
    <td align="center" sdval="97.1" sdnum="2052;">97.1</td>
    <td align="center" sdval="92.7" sdnum="2052;">92.7</td>
    <td align="center">-</td>
    <td align="center" sdval="95.4" sdnum="2052;">95.4</td>
    <td align="center" sdval="80.7" sdnum="2052;">80.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="98.6" sdnum="2052;"><b>98.6<b></td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center" sdval="93.1" sdnum="2052;">93.1</td>
    <td align="center" sdval="90.8" sdnum="2052;">90.8</td>
    <td align="center">ExPr</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [15]</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center">-</td>
    <td align="center" sdval="93.2" sdnum="2052;">93.2</td>
    <td align="center" sdval="71.7" sdnum="2052;">71.7</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center" sdval="93.4" sdnum="2052;">93.4</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center">SK + ExPr</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi, Bai, and Yao [16] : CRNN</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="81.2" sdnum="2052;">81.2</td>
    <td align="center" sdval="97.5" sdnum="2052;">97.5</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center" sdval="95.7" sdnum="2052;"><b>95.7<b></td>
    <td align="center" sdval="91.9" sdnum="2052;">91.9</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center">SK</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [17] : RARE</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="93.8" sdnum="2052;">93.8</td>
    <td align="center" sdval="81.9" sdnum="2052;">81.9</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center" sdval="81.9" sdnum="2052;">81.9</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="94.8" sdnum="2052;">94.8</td>
    <td align="center" sdval="90.1" sdnum="2052;">90.1</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Lee and Osindero [18] : R2AM</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="78.4" sdnum="2052;">78.4</td>
    <td align="center" sdval="96.3" sdnum="2052;">96.3</td>
    <td align="center" sdval="80.7" sdnum="2052;">80.7</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center">-</td>
    <td align="center" sdval="88.7" sdnum="2052;">88.7</td>
    <td align="center" sdval="90" sdnum="2052;">90</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [19] : STAR-Net</td>
    <td align="center" sdval="97.7" sdnum="2052;">97.7</td>
    <td align="center" sdval="94.5" sdnum="2052;">94.5</td>
    <td align="center" sdval="83.3" sdnum="2052;">83.3</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="96.9" sdnum="2052;">96.9</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">-</td>
    <td align="center" sdval="89.9" sdnum="2052;">89.9</td>
    <td align="center" sdval="89.1" sdnum="2052;">89.1</td>
    <td align="center">SK + ExPr</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al. [78]</td>
    <td align="center" sdval="94.1" sdnum="2052;">94.1</td>
    <td align="center" sdval="84.7" sdnum="2052;">84.7</td>
    <td align="center">-</td>
    <td align="center" sdval="92.5" sdnum="2052;">92.5</td>
    <td align="center">-</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="92.2" sdnum="2052;">92.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Mishra et al. [77]</td>
    <td align="center" sdval="78.07" sdnum="2052;">78.07</td>
    <td align="center">-</td>
    <td align="center" sdval="46.73" sdnum="2052;">46.73</td>
    <td align="center" sdval="78.2" sdnum="2052;">78.2</td>
    <td align="center">-</td>
    <td align="center" sdval="88" sdnum="2052;">88</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="67.7" sdnum="2052;">67.7</td>
    <td align="center" sdval="60.18" sdnum="2052;">60.18</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">CVIU</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Su and Lu [76]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91" sdnum="2052;">91</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="89" sdnum="2052;">89</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="76" sdnum="2052;">76</td>
    <td align="center">SK + ExPu</td>
    <td align="center">PR</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [20]</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="96.1" sdnum="2052;">96.1</td>
    <td align="center">-</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center">-</td>
    <td align="center" sdval="97.7" sdnum="2052;">97.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCAI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Yin et al. [21]</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="96.1" sdnum="2052;">96.1</td>
    <td align="center" sdval="78.2" sdnum="2052;">78.2</td>
    <td align="center" sdval="95.1" sdnum="2052;">95.1</td>
    <td align="center" sdval="72.5" sdnum="2052;">72.5</td>
    <td align="center" sdval="97.6" sdnum="2052;">97.6</td>
    <td align="center" sdval="96.5" sdnum="2052;">96.5</td>
    <td align="center">-</td>
    <td align="center" sdval="81.1" sdnum="2052;">81.1</td>
    <td align="center" sdval="81.4" sdnum="2052;">81.4</td>
    <td align="center">SK</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[66] : GRCNN</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center" sdval="95.6" sdnum="2052;">95.6</td>
    <td align="center" sdval="80.8" sdnum="2052;">80.8</td>
    <td align="center" sdval="96.3" sdnum="2052;">96.3</td>
    <td align="center" sdval="81.5" sdnum="2052;">81.5</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center">-</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Cheng et al. [22] : FAN</td>
    <td align="center" sdval="99.3" sdnum="2052;">99.3</td>
    <td align="center" sdval="97.5" sdnum="2052;">97.5</td>
    <td align="center" sdval="87.4" sdnum="2052;">87.4</td>
    <td align="center" sdval="97.1" sdnum="2052;">97.1</td>
    <td align="center" sdval="85.9" sdnum="2052;">85.9</td>
    <td align="center" sdval="99.2" sdnum="2052;">99.2</td>
    <td align="center" sdval="97.3" sdnum="2052;">97.3</td>
    <td align="center">-</td>
    <td align="center" sdval="94.2" sdnum="2052;">94.2</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Cheng et al. [23] : AON</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6<b></td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="87" sdnum="2052;">87</td>
    <td align="center" sdval="96" sdnum="2052;">96</td>
    <td align="center" sdval="82.8" sdnum="2052;">82.8</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="97.1" sdnum="2052;">97.1</td>
    <td align="center">-</td>
    <td align="center" sdval="91.5" sdnum="2052;">91.5</td>
    <td align="center">-</td>
    <td align="center">SK + ST (D_A)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [24]</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="96.7" sdnum="2052;">96.7</td>
    <td align="center">-</td>
    <td align="center" sdval="89.2" sdnum="2052;">89.2</td>
    <td align="center" sdval="88" sdnum="2052;">88</td>
    <td align="center">SK</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [25] : Char-Net</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center">-</td>
    <td align="center" sdval="84.4" sdnum="2052;">84.4</td>
    <td align="center">-</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center">-</td>
    <td align="center" sdval="91.5" sdnum="2052;">91.5</td>
    <td align="center" sdval="90.8" sdnum="2052;">90.8</td>
    <td align="center">SK (D_A)</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al.  [26] : SqueezedText</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center" sdval="94.1" sdnum="2052;">94.1</td>
    <td align="center" sdval="87" sdnum="2052;">87</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center">-</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="93.8" sdnum="2052;">93.8</td>
    <td align="center" sdval="93.1" sdnum="2052;">93.1</td>
    <td align="center" sdval="92.9" sdnum="2052;">92.9</td>
    <td align="center">ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al.[73]</td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center" sdval="79.3" sdnum="2052;">79.3</td>
    <td align="center" sdval="96.7" sdnum="2052;">96.7</td>
    <td align="center" sdval="81.5" sdnum="2052;">81.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="87.1" sdnum="2052;">87.1</td>
    <td align="center">Pr(5 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bai et al. [27] : EP</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="88.3" sdnum="2052;">88.3</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center">-</td>
    <td align="center" sdval="94.6" sdnum="2052;">94.6</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Fang et al.[74]</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="86.7" sdnum="2052;">86.7</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="86.7" sdnum="2052;">86.7</td>
    <td align="center" sdval="99.3" sdnum="2052;"><b>99.3<b></td>
    <td align="center" sdval="98.4" sdnum="2052;">98.4</td>
    <td align="center">-</td>
    <td align="center" sdval="94.8" sdnum="2052;">94.8</td>
    <td align="center" sdval="93.5" sdnum="2052;">93.5</td>
    <td align="center">SK + ST</td>
    <td align="center">MultiMedia</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.[75] : EnEsCTC</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82" sdnum="2052;">82</td>
    <td align="center">-</td>
    <td align="center" sdval="80.6" sdnum="2052;">80.6</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="92" sdnum="2052;">92</td>
    <td align="center" sdval="90.6" sdnum="2052;">90.6</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [28]</td>
    <td align="center" sdval="97.3" sdnum="2052;">97.3</td>
    <td align="center" sdval="96.1" sdnum="2052;">96.1</td>
    <td align="center" sdval="89.4" sdnum="2052;">89.4</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="87.1" sdnum="2052;">87.1</td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="97.5" sdnum="2052;">97.5</td>
    <td align="center">-</td>
    <td align="center" sdval="94.7" sdnum="2052;">94.7</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center">SK</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[61] : MAAN</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center" sdval="96.4" sdnum="2052;">96.4</td>
    <td align="center" sdval="84.1" sdnum="2052;">84.1</td>
    <td align="center" sdval="96.4" sdnum="2052;">96.4</td>
    <td align="center" sdval="83.5" sdnum="2052;">83.5</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="96.4" sdnum="2052;">96.4</td>
    <td align="center">-</td>
    <td align="center" sdval="92.2" sdnum="2052;">92.2</td>
    <td align="center" sdval="91.1" sdnum="2052;">91.1</td>
    <td align="center">SK</td>
    <td align="center">ICFHR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [29]</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="97.2" sdnum="2052;">97.2</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="97.7" sdnum="2052;">97.7</td>
    <td align="center" sdval="83.9" sdnum="2052;">83.9</td>
    <td align="center" sdval="98.6" sdnum="2052;">98.6</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center">-</td>
    <td align="center" sdval="91.4" sdnum="2052;">91.4</td>
    <td align="center" sdval="89.5" sdnum="2052;">89.5</td>
    <td align="center">SK</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [30] : ASTER</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6<b></td>
    <td align="center" sdval="98.8" sdnum="2052;"><b>98.8<b></td>
    <td align="center" sdval="93.4" sdnum="2052;">93.4</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="89.5" sdnum="2052;">89.5</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center">-</td>
    <td align="center" sdval="94.5" sdnum="2052;">94.5</td>
    <td align="center" sdval="91.8" sdnum="2052;">91.8</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : ASTER + AEG</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="90.3" sdnum="2052;">90.3</td>
    <td align="center" sdval="99" sdnum="2052;">99</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center">-</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [46] : MORAN</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center" sdval="88.3" sdnum="2052;">88.3</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="92.4" sdnum="2052;">92.4</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [61] : MORAN-v2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.4" sdnum="2052;">93.4</td>
    <td align="center">-</td>
    <td align="center" sdval="88.3" sdnum="2052;">88.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.2" sdnum="2052;">94.2</td>
    <td align="center" sdval="93.2" sdnum="2052;">93.2</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : MORAN-v2 + AEG</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="94.6" sdnum="2052;"><b>94.6<b></td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="90.4" sdnum="2052;">90.4</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center">-</td>
    <td align="center" sdval="95.3" sdnum="2052;"><b>95.3<b></td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Xie et al. [47] : CAN</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center" sdval="94.2" sdnum="2052;">94.2</td>
    <td align="center" sdval="80.5" sdnum="2052;">80.5</td>
    <td align="center" sdval="96.9" sdnum="2052;">96.9</td>
    <td align="center" sdval="83.4" sdnum="2052;">83.4</td>
    <td align="center" sdval="98.4" sdnum="2052;">98.4</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center">-</td>
    <td align="center" sdval="91" sdnum="2052;">91</td>
    <td align="center" sdval="90.5" sdnum="2052;">90.5</td>
    <td align="center">SK</td>
    <td align="center">ACM</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al.[48] : CA-FCN</td>
    <td align="center"><b>^99.8<b></td>
    <td align="center" sdval="98.9" sdnum="2052;">98.9</td>
    <td align="center" sdval="92" sdnum="2052;">92</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="82.1" sdnum="2052;">82.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91.4" sdnum="2052;">91.4</td>
    <td align="center">SK + ST+ ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Li et al. [49] : SAR</td>
    <td align="center" sdval="99.4" sdnum="2052;">99.4</td>
    <td align="center" sdval="98.2" sdnum="2052;">98.2</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center">SK + ST + ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhan el at. [55]: ESIR</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6<b></td>
    <td align="center" sdval="98.8" sdnum="2052;"><b>98.8<b></td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="90.2" sdnum="2052;">90.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91.3" sdnum="2052;">91.3</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [56]: SSDAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83.8" sdnum="2052;">83.8</td>
    <td align="center">-</td>
    <td align="center" sdval="84.5" sdnum="2052;">84.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="92.1" sdnum="2052;">92.1</td>
    <td align="center" sdval="91.8" sdnum="2052;">91.8</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [62]: ScRN</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="97.2" sdnum="2052;">97.2</td>
    <td align="center" sdval="88.9" sdnum="2052;">88.9</td>
    <td align="center" sdval="99" sdnum="2052;">99</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [64]: GCAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center">-</td>
    <td align="center" sdval="91.3" sdnum="2052;"><b>91.3<b></td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95.3" sdnum="2052;"><b>95.3<b></td>
    <td align="center" sdval="95.7" sdnum="2052;"><b>95.7<b></td>
    <td align="center">SK + ST</td>
    <td align="center">ICME</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Jeonghun et al. [65]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="87.9" sdnum="2052;">87.9</td>
    <td align="center">-</td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="92.3" sdnum="2052;">92.3</td>
    <td align="center">SK + ST</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="25" align="center">Huang et al. [67]：EPAN</td>
    <td align="center" sdval="98.9" sdnum="2052;">98.9</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center" sdval="88.9" sdnum="2052;">88.9</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="94.5" sdnum="2052;">94.5</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [68]</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="96.7" sdnum="2052;">96.7</td>
    <td align="center">-</td>
    <td align="center" sdval="89.2" sdnum="2052;">89.2</td>
    <td align="center" sdval="88" sdnum="2052;">88</td>
    <td align="center">SK</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Qi et al. [69] : CCL</td>
    <td align="center" sdval="99.6" sdnum="2052;">99.6</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="91.1" sdnum="2052;">91.1</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center" sdval="85.9" sdnum="2052;">85.9</td>
    <td align="center" sdval="99.2" sdnum="2052;">99.2</td>
    <td align="center"><b>^98.8<b></td>
    <td align="center">-</td>
    <td align="center" sdval="93.5" sdnum="2052;">93.5</td>
    <td align="center" sdval="92.8" sdnum="2052;">92.8</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Wang et al. [70] : ReELFA</td>
    <td align="center" sdval="99.2" sdnum="2052;">99.2</td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="90.9" sdnum="2052;">90.9</td>
    <td align="center">-</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhu et al. [71] : HATN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91.3" sdnum="2052;">91.3</td>
    <td align="center" sdval="91.1" sdnum="2052;">91.1</td>
    <td align="center">SK(D_A) + Pu</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al. [72] : SF-GAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="63" sdnum="2052;">63</td>
    <td align="center">-</td>
    <td align="center" sdval="69.3" sdnum="2052;">69.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="61.8" sdnum="2052;">61.8</td>
    <td align="center">Pr(1 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : SAM</td>
    <td align="center" sdval="99.4" sdnum="2052;">99.4</td>
    <td align="center" sdval="98.6" sdnum="2052;">98.6</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center" sdval="98.6" sdnum="2052;"><b>98.6<b></td>
    <td align="center" sdval="90.6" sdnum="2052;">90.6</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center">-</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al. [79] : seg-SAM</td>
    <td align="center"><b>^99.8<b></td>
    <td align="center"><b>^99.3<b></td>
    <td align="center"><b>^95.3<b></td>
    <td align="center"><b>^99.1<b></td>
    <td align="center"><b>^91.8<b></td>
    <td align="center" sdval="99" sdnum="2052;">99</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">SK + ST (char-level)</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [80] : DAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.3" sdnum="2052;">94.3</td>
    <td align="center">-</td>
    <td align="center" sdval="89.2" sdnum="2052;">89.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center">SK + ST</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
</table>

<a id="222-recognition-results-on-irregular-dataset"></a>

#### 2.2.2 Recognition Results on Irregular Dataset

<body>
<table cellspacing="0" border="0">
  <colgroup span="10" width="85"></colgroup>
  <tr>
    <td colspan=10 height="20" align="center"><b>Recognition Results on Irregular Datasets</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td colspan=3 align="center">SVT-P</td>
    <td align="center">CUTE80</td>
    <td align="center">IC15</td>
    <td align="center">COCO-TEXT</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Source</td>
    <td rowspan=2 align="center">Time</td>
  </tr>
  <tr>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">Full</td>
    <td align="center">None</td>
    <td align="center">None</td>
    <td align="center">None</td>
    <td align="center">None</td>
    </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : ABBYY</td>
    <td align="center" sdval="40.5" sdnum="2052;">40.5</td>
    <td align="center" sdval="26.1" sdnum="2052;">26.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : SYNTH+PLEX</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [2]</td>
    <td align="center" sdval="45.7" sdnum="2052;">45.7</td>
    <td align="center" sdval="24.7" sdnum="2052;">24.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [3]</td>
    <td align="center" sdval="40.2" sdnum="2052;">40.2</td>
    <td align="center" sdval="32.4" sdnum="2052;">32.4</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Goel et al. [4] : wDTW</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Bissacco et al. [5] : PhotoOCR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Phan et al. [6]</td>
    <td align="center" sdval="62.3" sdnum="2052;">62.3</td>
    <td align="center" sdval="42.2" sdnum="2052;">42.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Alsharif et al. [7] : HMM/Maxout</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Almazan et al [8] : KCSR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Yao et al. [9] : Strokelets</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">R.-Serrano et al.[10] : Label embedding</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [11]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [12]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ACCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Gordo[13] : Mid-features</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [14]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [15]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ExPr</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi, Bai, and Yao [16] : CRNN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [17] : RARE</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center" sdval="77.4" sdnum="2052;">77.4</td>
    <td align="center" sdval="71.8" sdnum="2052;">71.8</td>
    <td align="center" sdval="59.2" sdnum="2052;">59.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Lee and Osindero [18] : R2AM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [19] : STAR-Net</td>
    <td align="center" sdval="94.3" sdnum="2052;">94.3</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="73.5" sdnum="2052;">73.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ExPr</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al. [78]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Mishra et al. [77]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">CVIU</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Su and Lu [76]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ExPu</td>
    <td align="center">PR</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [20]</td>
    <td align="center" sdval="93" sdnum="2052;">93</td>
    <td align="center" sdval="80.2" sdnum="2052;">80.2</td>
    <td align="center" sdval="75.8" sdnum="2052;">75.8</td>
    <td align="center" sdval="69.3" sdnum="2052;">69.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCAI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Yin et al. [21]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[66] : GRCNN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Cheng et al. [22] : FAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>*85.3<b></td>
    <td align="center">-</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Cheng et al. [23] : AON</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center" sdval="83.7" sdnum="2052;">83.7</td>
    <td align="center" sdval="73" sdnum="2052;">73</td>
    <td align="center" sdval="76.8" sdnum="2052;">76.8</td>
    <td align="center" sdval="68.2" sdnum="2052;">68.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST (D_A)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [24]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [25] : Char-Net</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.5" sdnum="2052;">73.5</td>
    <td align="center">-</td>
    <td align="center" sdval="60" sdnum="2052;">60</td>
    <td align="center">-</td>
    <td align="center">SK (D_A)</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al.  [26] : SqueezedText</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al.[73]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Pr(5 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bai et al. [27] : EP</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Fang et al.[74]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="71.2" sdnum="2052;">71.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">MultiMedia</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.[75] : EnEsCTC</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [28]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center" sdval="62.5" sdnum="2052;">62.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[61] : MAAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ICFHR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [29]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [30] : ASTER</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="78.5" sdnum="2052;">78.5</td>
    <td align="center" sdval="79.5" sdnum="2052;">79.5</td>
    <td align="center" sdval="76.1" sdnum="2052;">76.1</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : ASTER + AEG</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="89.5" sdnum="2052;">89.5</td>
    <td align="center" sdval="82" sdnum="2052;">82</td>
    <td align="center" sdval="80.9" sdnum="2052;">80.9</td>
    <td align="center" sdval="76.7" sdnum="2052;">76.7</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [46] : MORAN</td>
    <td align="center" sdval="94.3" sdnum="2052;">94.3</td>
    <td align="center" sdval="86.7" sdnum="2052;">86.7</td>
    <td align="center" sdval="76.1" sdnum="2052;">76.1</td>
    <td align="center" sdval="77.4" sdnum="2052;">77.4</td>
    <td align="center" sdval="68.8" sdnum="2052;">68.8</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [61] : MORAN-v2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="79.7" sdnum="2052;">79.7</td>
    <td align="center" sdval="81.9" sdnum="2052;">81.9</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : MORAN-v2 + AEG</td>
    <td align="center" sdval="94.7" sdnum="2052;"><b>94.7<b></td>
    <td align="center" sdval="89.6" sdnum="2052;"><b>89.6<b></td>
    <td align="center" sdval="82.8" sdnum="2052;">82.8</td>
    <td align="center" sdval="81.3" sdnum="2052;">81.3</td>
    <td align="center" sdval="77.4" sdnum="2052;">77.4</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Xie et al. [47] : CAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ACM</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al.[48] : CA-FCN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="78.1" sdnum="2052;">78.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST+ ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Li et al. [49] : SAR</td>
    <td align="center"><b>^95.8<b></td>
    <td align="center"><b>^91.2<b></td>
    <td align="center"><b>^86.4<b></td>
    <td align="center"><b>^89.6<b></td>
    <td align="center" sdval="78.8" sdnum="2052;">78.8</td>
    <td align="center"><b>^66.8<b></td>
    <td align="center">SK + ST + ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhan el at. [55]: ESIR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="79.6" sdnum="2052;">79.6</td>
    <td align="center" sdval="83.3" sdnum="2052;">83.3</td>
    <td align="center" sdval="76.9" sdnum="2052;">76.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [56]: SSDAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [62]: ScRN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="80.8" sdnum="2052;">80.8</td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center" sdval="78.7" sdnum="2052;">78.7</td>
    <td align="center">-</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [64]: GCAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="85.7" sdnum="2052;"><b>85.7<b></td>
    <td align="center" sdval="83.3" sdnum="2052;">83.3</td>
    <td align="center" sdval="83.5" sdnum="2052;"><b>83.5<b></td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">ICME</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Jeonghun et al. [65]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="79.2" sdnum="2052;">79.2</td>
    <td align="center" sdval="74" sdnum="2052;">74</td>
    <td align="center" sdval="71.8" sdnum="2052;">71.8</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="25" align="center">Huang et al. [67]：EPAN</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center" sdval="86.4" sdnum="2052;">86.4</td>
    <td align="center" sdval="79.4" sdnum="2052;">79.4</td>
    <td align="center" sdval="82.6" sdnum="2052;">82.6</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [68]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="62.3" sdnum="2052;">62.3</td>
    <td align="center" sdval="40" sdnum="2052;">40</td>
    <td align="center">SK</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Qi et al. [69] : CCL</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="72.9" sdnum="2052;">72.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Wang et al. [70] : ReELFA</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82.3" sdnum="2052;">82.3</td>
    <td align="center" sdval="68.5" sdnum="2052;">68.5</td>
    <td align="center">-</td>
    <td align="center">ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhu et al. [71] : HATN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.5" sdnum="2052;">73.5</td>
    <td align="center" sdval="75.7" sdnum="2052;">75.7</td>
    <td align="center" sdval="70.1" sdnum="2052;">70.1</td>
    <td align="center">-</td>
    <td align="center">SK(D_A) + Pu</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al. [72] : SF-GAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="48.6" sdnum="2052;">48.6</td>
    <td align="center" sdval="40.6" sdnum="2052;">40.6</td>
    <td align="center" sdval="39" sdnum="2052;">39</td>
    <td align="center">-</td>
    <td align="center">Pr(1 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : SAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center" sdval="87.8" sdnum="2052;"><b>87.8<b></td>
    <td align="center" sdval="77.3" sdnum="2052;">77.3</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al. [79] : seg-SAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="88.5" sdnum="2052;">88.5</td>
    <td align="center" sdval="78.2" sdnum="2052;">78.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST (char-level)</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [80] : DAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="80" sdnum="2052;">80</td>
    <td align="center" sdval="84.4" sdnum="2052;">84.4</td>
    <td align="center" sdval="74.5" sdnum="2052;">74.5</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
</table>

<a id="223-recognition-results-on-bilingual-scene-text-dataset"></a>

#### 2.2.3 Recognition Results on Bilingual Scene Text Dataset

In this section, we only list the top three results of each competition. Please refer to the competition website for more information.

<body>
<table cellspacing="0" border="0">
  <colgroup span="9" width="85"></colgroup>
  <tr>
    <td colspan=9 height="20" align="center"><b>Recognition Results on Bilingual Scene Text Dataset</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RCTW&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MTWI&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">CTW</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LSVT&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ArT&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ReCTS&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Time</td>
    <td rowspan=2 align="center">Source</td>
  </tr>
  <tr>
    </tr>
  <tr>
    <td height="20" align="center">Lv et al. : NLPR PAL</td>
    <td align="center"><b>0.3201 (end-to-end)<b></td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">RCTW Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">Jin et al. : SCUT_DLVC</td>
    <td align="center">0.2374 (end-to-end)</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">RCTW Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">Dai et al. : CCFLAB</td>
    <td align="center">0.2143 (end-to-end)</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">RCTW Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">IFLYTEK : nelslip(iflytek&amp;ustc)</td>
    <td align="center">-</td>
    <td align="center"><b>85.8 (AR)<b></td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">MTWI Competition</td>
  </tr>
  <tr>
    <td height="46" align="center">Samsung R&amp;D China, Beijing : <br>SRC-B-MachineLearningLab</td>
    <td align="center">-</td>
    <td align="center">85.7(AR)</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">MTWI Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">NetEase : NTAI</td>
    <td align="center">-</td>
    <td align="center">82.6(AR)</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">MTWI Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">Yuan et al.[42] : CTW</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>80.5 (AR)<b></td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">CTW</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [43] : SCUT-CTW1500</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">SCUT-CTW1500</td>
  </tr>
  <tr>
    <td height="20" align="center">Tencent-DPPR Team</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>66.66 (end-to-end)<b></td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">LSVT Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">HUST VLRGROUP</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">63.42 (end-to-end)</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">LSVT Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">PMTD</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">63.36 (end-to-end)</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">LSVT Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">Clova AI OCR Team, NAVER/LINE Corp</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>85.32 (AR)<b></td>
    <td align="center">-</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ArT Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">SenseTime Group</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">85.2 (AR)</td>
    <td align="center">-</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ArT Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">USTC-iFLYTEK</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">81.23 (AR)</td>
    <td align="center">-</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ArT Competition</td>
  </tr>
  <tr>
    <td height="46" align="center">SCUT, The University of Adelaide, Northwestern Polytechnical University, <br>Lenovo, HUAWEI</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>95.55 (AR)<b></td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ReCTS Competition</td>
  </tr>
  <tr>
    <td height="46" align="center">Tencent<br>(Data Platform Precision Recommendation)</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">94.86 (AR)</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ReCTS Competition</td>
  </tr>
  <tr>
    <td height="20" align="center">Huazhong University of Science and Technology</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">94.83 (AR)</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ReCTS Competition</td>
  </tr>
</table>

***

<a id="3-field-survey"></a>
## 3. Survey

**[50] \[TPAMI-2015]** Ye Q, Doermann D. Text detection and recognition in imagery: A survey[J]. IEEE transactions on pattern analysis and machine intelligence, 2015, 37(7): 1480-1500. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6945320)

**[51] \[Frontiers-Comput. Sci-2016]** Zhu Y, Yao C, Bai X. Scene text detection and recognition: Recent advances and future trends[J]. Frontiers of Computer Science, 2016, 10(1): 19-36. [paper](https://link.springer.com/article/10.1007/s11704-015-4488-0)

**[52] \[arXiv-2018]** Long S, He X, Ya C. Scene Text Detection and Recognition: The Deep Learning Era[J]. arXiv preprint arXiv:1811.04256, 2018. [paper](https://arxiv.org/pdf/1811.04256.pdf)

***

<a id="4-ocr-service"></a>
## 4. OCR Service

|                             OCR                              | API  | Free | Code |
| :----------------------------------------------------------: | :--: | :--: | :--: |
| [Tesseract OCR Engine](https://github.com/tesseract-ocr/tesseract) |  ×   |  √   |  √   |
| [Azure](https://azure.microsoft.com/zh-cn/services/cognitive-services/computer-vision/#Analysis) |  √   |  √   |  ×   |
| [ABBYY](https://www.abbyy.cn/real-time-recognition-sdk/technical-specifications/) |  √   |  √   |  ×   |
|               [OCR Space](https://ocr.space/)                |  √   |  √   |  ×   |
|       [SODA PDF OCR](https://www.sodapdf.com/ocr-pdf/)       |  √   |  √   |  ×   |
|          [Free Online OCR](https://www.newocr.com/)          |  √   |  √   |  ×   |
|           [Online OCR](https://www.onlineocr.net/)           |  √   |  √   |  ×   |
|             [Super Tools](https://www.wdku.net/)             |  √   |  √   |  ×   |
|   [Online Chinese Recognition](http://chongdata.com/ocr/)    |  √   |  √   |  ×   |
|   [Calamari OCR](https://github.com/Calamari-OCR/calamari)   |  ×   |  √   |  √   |
| [ Tencent OCR](https://cloud.tencent.com/product/ocr?lang=cn) |  √   |  ×   |  ×   |

***

<a id="5-references"></a>
## 5. References

**[1] \[ICCV-2011]** K. Wang, B. Babenko, and S. Belongie. End-to-end scene text recognition. In Proceedings of International Conference on Computer Vision (ICCV), pages 1457–1464, 2011. [paper ](https://www.researchgate.net/profile/Serge_Belongie/publication/221110077_End-to-end_scene_text_recognition/links/09e4150b34908d2ebb000000/End-to-end-scene-text-recognition.pdf)

**[2] \[BMVC-2012]** A. Mishra, K. Alahari, and C. Jawahar. Scene text recognition using higher order language priors. In Proceedings of British Machine Vision Conference (BMVC), pages 1–11, 2012. [paper](https://hal.inria.fr/hal-00818183/document) [dataset](http://cvit.iiit.ac.in/research/projects/cvit-projects/the-iiit-5k-word-dataset)

**[3] \[ICPR-2012]** T. Wang, D. J. Wu, A. Coates, and A. Y. Ng. End-to-end text recognition with convolutional neural networks. In Proceedings of International Conference on Pattern Recognition (ICPR), pages 3304–3308, 2012. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6460871&tag=1)

**[4] \[ICDAR-2013]** V. Goel, A. Mishra, K. Alahari, and C. Jawahar. Whole is greater than sum of parts: Recognizing scene text words. In Proceedings of International Conference on Document Analysis and Recognition (ICDAR), pages 398–402, 2013. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6628652) 

**[5] \[ICCV-2013]** A. Bissacco, M. Cummins, Y. Netzer, and H. Neven. Photoocr: Reading text in uncontrolled conditions. In Proceedings of International Conference on Computer Vision (ICCV), pages 785–792, 2013. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Bissacco_PhotoOCR_Reading_Text_2013_ICCV_paper.pdf)

**[6] \[ICCV-2013]** T. Quy Phan, P. Shivakumara, S. Tian, and C. Lim Tan. Recognizing text with perspective distortion in natural scenes.In Proceedings of International Conference on Computer Vision (ICCV), pages 569–576, 2013. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Phan_Recognizing_Text_with_2013_ICCV_paper.pdf)

**[7] \[ICLR-2014]** O. Alsharif and J. Pineau, End-to-end text recognition with hybrid HMM maxout models, in: Proceedings of International Conference on Learning Representations (ICLR), 2014. [paper](https://arxiv.org/pdf/1310.1811.pdf)

**[8] \[TPAMI-2014]** J. Almaz ́ an, A. Gordo, A. Forn ́ es, and E. Valveny. Word spotting and recognition with embedded attributes. IEEE Trans.Pattern Anal. Mach. Intell ., 36(12):2552–2566, 2014. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6857995) [code](https://github.com/almazan/watts)

**[9] \[CVPR-2014]** C. Yao, X. Bai, B. Shi, and W. Liu. Strokelets: A learned multi-scale representation for scene text recognition. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 4042–4049, 2014. [paper](http://openaccess.thecvf.com/content_cvpr_2014/papers/Yao_Strokelets_A_Learned_2014_CVPR_paper.pdf)

**[10] \[IJCV-2015]** J. A. Rodriguez-Serrano, A. Gordo, and F. Perronnin. Label embedding: A frugal baseline for text recognition. International Journal of Computer Vision (IJCV) , 113(3):193–207, 2015. [paper](https://link.springer.com/content/pdf/10.1007%2Fs11263-014-0793-6.pdf)

**[11] \[ECCV-2014]** M. Jaderberg, A. Vedaldi, and A. Zisserman. Deep features for text spotting. In Proceedings of European Conference on Computer Vision (ECCV), pages 512–528, 2014. [paper](https://link.springer.com/content/pdf/10.1007%2F978-3-319-10593-2_34.pdf) [code](https://bitbucket.org/jaderberg/eccv2014_textspotting/src/master/)

**[12] \[ACCV-2014]** B. Su and S. Lu. Accurate scene text recognition based on recurrent neural network. In Proceedings of Asian Conference on Computer Vision (ACCV), pages 35–48, 2014. [paper](https://link.springer.com/content/pdf/10.1007%2F978-3-319-16865-4_3.pdf)

**[13] \[CVPR-2015]** A. Gordo. Supervised mid-level features for word image representation. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 2956–2964, 2015. [paper](http://openaccess.thecvf.com/content_cvpr_2015/papers/Gordo_Supervised_Mid-Level_Features_2015_CVPR_paper.pdf)

**[14] \[IJCV-2015]** M. Jaderberg, K. Simonyan, A. Vedaldi, and A. Zisserman. Reading text in the wild with convolutional neural networks. Int. J.Comput. Vision, 2015. [paper](https://link.springer.com/content/pdf/10.1007%2Fs11263-015-0823-z.pdf) [code](http://www.robots.ox.ac.uk/~vgg/research/text/)

**[15] \[ICLR-2015]** M. Jaderberg, K. Simonyan, A. Vedaldi, A. Zisserman, Deep structured output learning for unconstrained text recognition, in: Proceedings of International Conference on Learning Representations (ICLR), 2015. [paper](https://arxiv.org/pdf/1412.5903.pdf) 

**[16] \[TPAMI-2017]** B. Shi, X. Bai, and C. Yao. An end-to-end trainable neural network for image-based sequence recognition and its application to scene text recognition. IEEE Trans. Pattern Anal. Mach. Intell., 39(11):2298–2304, 2017. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7801919) [code-Torch7](https://github.com/bgshih/crnn) [code-Pytorch](https://github.com/meijieru/crnn.pytorch)

**[17] \[CVPR-2016]** B. Shi, X. Wang, P. Lyu, C. Yao, and X. Bai. Robust scene text recognition with automatic rectification. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 4168–4176, 2016. [paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Shi_Robust_Scene_Text_CVPR_2016_paper.pdf)

**[18] \[CVPR-2016]** C.-Y. Lee and S. Osindero. Recursive recurrent nets with attention modeling for OCR in the wild. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 2231–2239, 2016. [paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Lee_Recursive_Recurrent_Nets_CVPR_2016_paper.pdf)

**[19] \[BMVC-2016]** W. Liu, C. Chen, K.-Y. K. Wong, Z. Su, and J. Han. STAR-Net: A spatial attention residue network for scene text recognition. In Proceedings of British Machine Vision Conference (BMVC), page 7, 2016. [paper](https://i.cs.hku.hk/~kykwong/publications/wliu_bmvc16.pdf)

**[20] \[IJCAI-2017]** X. Yang, D. He, Z. Zhou, D. Kifer, and C. L. Giles. Learning to read irregular text with attention mechanisms. Proceedings of International Joint Conference on Artificial Intelligence (IJCAI), 2017. [paper](https://pdfs.semanticscholar.org/1259/f7533abe2fe85fd9dead92853e2ff07a8792.pdf)

**[21] \[ICCV-2017]** F. Yin, Y.-C. Wu, X.-Y. Zhang, and C.-L. Liu. Scene text recognition with sliding convolutional character models. In Proceedings of International Conference on Computer Vision (ICCV), 2017. [paper](https://arxiv.org/pdf/1709.01727.pdf) [code](https://github.com/lsvih/Sliding-Convolution)

**[22] \[ICCV-2017]** Z. Cheng, F. Bai, Y. Xu, G. Zheng, S. Pu, and S. Zhou. Focusing attention: Towards accurate text recognition in natural images. In Proceedings of International Conference on Computer Vision (ICCV), pages 5086–5094, 2017. [paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Cheng_Focusing_Attention_Towards_ICCV_2017_paper.pdf)

**[23] \[CVPR-2018]** Cheng Z, Xu Y, Bai F, et al. AON: Towards Arbitrarily-Oriented Text Recognition.In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 5571-5579, 2018. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Cheng_AON_Towards_Arbitrarily-Oriented_CVPR_2018_paper.pdf) [code](https://github.com/huizhang0110/AON)

**[24] \[arXiv-2017]** Gao Y, Chen Y, Wang J, et al. Reading Scene Text with Attention Convolut ional Sequence Modeling[J]. arXiv preprint arXiv:1709.04303, 2017. [paper](https://arxiv.org/pdf/1709.04303.pdf)

**[25] \[AAAI-2018]** Liu W, Chen C, Wong K Y K. Char-Net: A Character-Aware Neural Network for Distorted Scene Text Recognition[C]//AAAI. 2018. [paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16327/16307)

**[26] \[AAAI-2018]** Liu Z, Li Y, Ren F, et al. SqueezedText: A Real-Time Scene Text Recognition by Binary Convolutional Encoder-Decoder Network[C]//AAAI. 2018. [paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16354/16312)

**[27] \[CVPR-2018]** Bai, F, Cheng, Z, Niu, Y, Pu, S and Zhou,S. Edit probability for scene text recognition, pages 1508-1516, 2018. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Bai_Edit_Probability_for_CVPR_2018_paper.pdf)

**[28] \[ECCV-2018]** Liu Y, Wang Z, Jin H, et al. Synthetically Supervised Feature Learning for Scene Text Recognition[C]//Proceedings of the European Conference on Computer Vision (ECCV). 2018: 435-451. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Yang_Liu_Synthetically_Supervised_Feature_ECCV_2018_paper.pdf)

**[29] \[ICIP-2018]** Gao Y, Chen Y, Wang J, et al. Dense Chained Attention Network for Scene Text Recognition[C]//2018 25th IEEE International Conference on Image Processing (ICIP). IEEE, 2018: 679-683. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8451273)

**[30] \[TPAMI-2018]** Shi B, Yang M, Wang X, et al. Aster: An attentional scene text recognizer with flexible rectification[J]. IEEE transactions on pattern analysis and machine intelligence, 2018. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8395027) [code](https://github.com/bgshih/aster)

**[31] \[CVPR-2012]** A. Mishra, K. Alahari, and C. V. Jawahar. Top-down and bottom-up cues for scene text recognition. In CVPR, 2012. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6247990)

**[32]** https://github.com/Canjie-Luo/MORAN_v2

**[33] \[IJDAR-2005]** S. M. Lucas, A. Panaretos, L. Sosa, A. Tang, S. Wong, R. Young,K. Ashida, H. Nagai, M. Okamoto, H. Yamamoto, H. Miyao,J. Zhu, W. Ou, C. Wolf, J. Jolion, L. Todoran, M. Worring, and X. Lin. ICDAR 2003 robust reading competitions:entries, results,and future directions. IJDAR, 7(2-3):105–122, 2005. [paper](https://link.springer.com/content/pdf/10.1007%2Fs10032-004-0134-3.pdf)

**[34] \[ICDAR-2013]** D. Karatzas, F. Shafait, S. Uchida, M. Iwamura, L. G. i Bigorda,S. R. Mestre, J. Mas, D. F. Mota, J. Almaz ́ an, and L. de las Heras. ICDAR 2013 robust reading competition. In ICDAR, 2013. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6628859)

**[35] \[ICCV-2013]** T. Q. Phan, P. Shivakumara, S. Tian, and C. L. Tan. Recognizing text with perspective distortion in natural scenes. In ICCV, 2013. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Phan_Recognizing_Text_with_2013_ICCV_paper.pdf)

**[36] \[Expert Syst.Appl-2014]** A. Risnumawan, P. Shivakumara, C. S. Chan, and C. L. Tan. A robust arbitrary text detection system for natural scene images. Expert Syst. Appl., 41(18):8027–8048, 2014. [paper](https://pdf.sciencedirectassets.com/271506/1-s2.0-S0957417414X00114/1-s2.0-S0957417414004060/main.pdf?x-amz-security-token=AgoJb3JpZ2luX2VjEIn%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJGMEQCIGRhldIzSEiSi38FQg8SKy0nbkjetbYc6MOZN8lXbsg7AiB5pY6PoVDS8%2F3qS%2FPqd0zaHjqWrjqvDrAtTiZVSrpKmyrjAwiC%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAIaDDA1OTAwMzU0Njg2NSIMoRUcs%2Ft3M%2Blz7DI3KrcDKVODcJNpq1tNel77UHdAJVSUDWRkG7Fx5loyHhQsb2V3MFfHqAGKJpbdr7xHlDY7CaTl5nrTdNe91InXfpM25fFyYQlANwrhlcYGiPEsN14mSBe%2F5gy0gipiPaN835Viwb0O1Raw9MP9Clc84q%2BHvW5YyQ02NIZYE7OlHYSWN6mbI0F9r7reRa2zNLjFVcvJRkAyt4I9L1Pbehf4WwFF1Er0ResczdJ2FbwKCZNaKWznwhdjVp8hw0SFC%2F9uxnDHzu8DTPeutA3mHeUetMOEtKspkSvIj%2FWQDI1OTECcNv0N7CfmUKSh9m5tOYn%2Fb7KQx8pPA450Snd3faB7euDzPwvCmtfeUzYs0n0UxWt9JWXxKONmvrMlxf9bjZL0RBR1NNeNgwFuCCCRZDAKogbBI%2FclJmPUiNO38mHO10B1unMow9XtojodS3U6Iz2n8jeERhaR4Rt4KeWB9ojZTQhUr5d1uUX%2FVpmJmFQhgvPXmEi%2Fnlp65TXeZNdbUncQPqZ8PaKGYxJn1F%2FwnuJH1Ww6ksTur4rcggGAEHTBgXL5vmLjJG2ZhH1vxaoY8qtUO5EuXwVVfBXCtzCit9jmBTq1Abb%2BixDckXLEYAwidBhA%2B4MKpbhmH4LItnjE3tSuFgOHFbwaq9g0MZyGtL3OUxCKc3eAkkLzOrJnEag%2F2eV%2BdMcU9%2F%2BKI5h8yQsz5PEFeqkY3BID%2BY7oIU6qhqhb38PVrbt1oyF420cS%2BoSpt2Nj6E%2FuCZZTrgMakE%2B9QXvAaTIBWG%2Fc0xOv6d3rGTAnZTkkscgD7j%2FP1jqFkf388YT5jCbAWlx8OiMbj%2BVPkK8UvXhgSh1ZPMk%3D&AWSAccessKeyId=ASIAQ3PHCVTY6VYAY5FB&Expires=1557539079&Signature=HF7E%2BOACBDJPtLAerMWH6MTKDCw%3D&hash=8fe7c8a1c5599e4659a2b26919b2a59f4aff8c452e5a07793dc187e49c69dc9e&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0957417414004060&tid=spdf-7bd6a860-4c57-4e39-87ce-bd2f050badcf&sid=57f9f09d5d026341242a7bd2fb38b97c5897gxrqb&type=client)

**[37] \[ICDAR-2015]** D. Karatzas, L. Gomez-Bigorda, A. Nicolaou, S. K. Ghosh, A. D.Bagdanov, M. Iwamura, J. Matas, L. Neumann, V. R. Chandrasekhar, S. Lu, F. Shafait, S. Uchida, and E. Valveny. ICDAR 2015 competition on robust reading. In ICDAR, pages 1156–1160,2015. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7333942)

**[38] \[arXiv-2016]** Veit A, Matera T, Neumann L, et al. Coco-text: Dataset and benchmark for text detection and recognition in natural images[J]. arXiv preprint arXiv:1601.07140, 2016. [paper](https://arxiv.org/pdf/1601.07140.pdf) [code](https://github.com/andreasveit/coco-text)

**[39] \[ICDAR-2017]** Ch'ng C K, Chan C S. Total-text: A comprehensive dataset for scene text detection and recognition[C]//Document Analysis and Recognition (ICDAR), 2017 14th IAPR International Conference on. IEEE, 2017, 1: 935-942. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8270088) [code](https://github.com/cs-chan/Total-Text-Dataset)

**[40] \[ICDAR-2017]** Shi B, Yao C, Liao M, et al. ICDAR2017 competition on reading chinese text in the wild (RCTW-17)[C]//Document Analysis and Recognition (ICDAR), 2017 14th IAPR International Conference on. IEEE, 2017, 1: 1429-1434. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8270164)

**[41] \[ICPR-2018]** He M, Liu Y, Yang Z, et al. ICPR2018 Contest on Robust Reading for Multi-Type Web Images[C]//2018 24th International Conference on Pattern Recognition (ICPR). IEEE, 2018: 7-12. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8546143)

**[42] \[arXiv-2018]** Yuan T L, Zhu Z, Xu K, et al. Chinese Text in the Wild[J]. arXiv preprint arXiv:1803.00085, 2018. [paper](https://arxiv.org/pdf/1803.00085.pdf) [code](https://github.com/yuantailing/ctw-baseline)

**[43] \[arXiv-2017]** Yuliang L, Lianwen J, Shuaitao Z, et al. Detecting curve text in the wild: New dataset and new solution[J]. arXiv preprint arXiv:1712.02170, 2017. [paper](https://arxiv.org/pdf/1712.02170.pdf) [code](https://github.com/Yuliang-Liu/Curve-Text-Detector)

**[44] \[ECCV-2018]** Yao C, Wu W. Mask TextSpotter: An End-to-End Trainable Neural Network for Spotting Text with Arbitrary Shapes.//Proceedings of the European Conference on Computer Vision (ECCV). 2018: 71-88. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Pengyuan_Lyu_Mask_TextSpotter_An_ECCV_2018_paper.pdf) [code](https://github.com/lvpengyuan/masktextspotter.caffe2)

**[45] \[NIPS-WORKSHOP-2011]** Yuval Netzer, Tao Wang, Adam Coates, Alessandro Bissacco,Bo Wu, and Andrew YNg. Reading digits in natural images with unsupervised feature learning. In NIPS workshop on deep learning and unsupervised feature learning, volume 2011, page 5, 2011. [paper](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/37648.pdf)

**[46] \[PR-2019]**  C. Luo, L. Jin, and Z. Sun, “MORAN: A multi-object rectified attention network for scene text recognition,” Pattern Recognition, vol. 90, pp. 109–118, 2019. [paper](https://pdf.sciencedirectassets.com/272206/1-s2.0-S0031320319X00023/1-s2.0-S0031320319300263/main.pdf?x-amz-security-token=AgoJb3JpZ2luX2VjEHcaCXVzLWVhc3QtMSJIMEYCIQCceDsmz9xCoE%2FnPRGjEfK6RAdvbVW7B%2B7rvG4viZPq%2BAIhALnS8lFI9N7LE3%2BNey3EgbWZU8f%2BJIAJIxlk5ewtKNTgKtoDCG8QAhoMMDU5MDAzNTQ2ODY1IgxbFmRrlDI1X0pjiscqtwMyG%2F2gaQjY2Ol3wnc2MtQwmfUOBotnxAj7F7lPnLyeRqPWJo6swI52Tz0YWuSI%2FTXRk3wuLNZthvTkLRWlD5wejFNGIAM9VNUuaYmfhLPT%2Ft33yaDBMGBe3wP%2BdsH0OXHn7JtbzLAFK%2BFPBYXLfSMth4IbmdKzLPAR77noWqY3NvtbYRJEvpw4r9N7yvM%2Fo1lBQnoulBsX%2B7sKRKm9SxWrreldzSuX2EIbnk5FPyXAkTlzYfH%2FCjoTOGYrReZl1VeFSnml73TaF1RImYbO0t155QfM8X90oEMKxlfd1IU8PzuYy14%2Bo0TAmHB3kYh3aKN6CEZ%2FEAHhxxhGrysEhBZWLF0RMp2oZFGDPxiOJVo3QES2GR38d9uBYjXF0dzjxgFnn40SuYTRE29nIjspgjZbsqeWyP%2BbsFHJcteX3w0eN6wq%2B%2Bbd5yPuAELoAy246KPZvRwBXGYUH1%2Bgm%2BqIIKidMGUedx98L2%2FO%2FAnbQ7gPCKW9HIWRdExufStWHid2r8gPpwB3%2Fb%2FKtCbA7iqm7cedZaqgjvaBbKM0hgBlgfXMGJTniXSmGYAIhvgH0aAlUCAAGeNsovbGMMCw1OYFOrMBESogEL75zcwF5QSaTC8s2DdSVFWjhwza7lgexCXY7r6aW4Y80XYluSj6%2BPWj2x6qH23kIlPIEfmyXL%2FJbbBzxTh%2FBbA9UVu04wph8eB%2BNGtvajIx%2FZFVNJSHc3WHz2DWlSAkLnuNGtahDLdXTG3ZD9jhdbweN7QdKYXsPPLh6ysos7v0hO9f7mM2%2BWsA5yOwB8lg9d2xmYu2PU6RKCQcv8hC1ASHgZh5PiYGBUjTfdv0cfI%3D&AWSAccessKeyId=ASIAQ3PHCVTYXA3CRTFK&Expires=1557473755&Signature=eBwdaj8gPpxtBnisCTPveLqX3iw%3D&hash=6f612616f8fba56ffd779d1eee8bfb19e39b7276f2b922ed529a46e51075049d&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0031320319300263&tid=spdf-5d02711b-ea3c-46c1-bb55-4d301d13f947&sid=57f9f09d5d026341242a7bd2fb38b97c5897gxrqb&type=client) [code](https://github.com/Canjie-Luo/MORAN_v2)

**[47] \[ACM-2019]** Xie H, Fang S, Zha Z J, et al, “Convolutional Attention Networks for Scene Text Recognition,” ACM Transactions on Multimedia Computing, Communications, and Applications (TOMM), vol. 15, pp. 3 2019. [paper](https://dl.acm.org/citation.cfm?id=3231737)

**[48] \[AAAI-2019]** Liao M, Zhang J, Wan Z, et al, “Scene text recognition from two-dimensional perspective,” //AAAI. 2019. [paper](https://arxiv.org/pdf/1809.06508.pdf) 

**[49] \[AAAI-2019]** Li H, Wang P, Shen C, et al, “Show, Attend and Read: A Simple and Strong Baseline for Irregular Text Recognition,” //AAAI. 2019. [paper](https://arxiv.org/pdf/1811.00751.pdf) [code](https://tinyurl.com/ShowAttendRead)

**[50] \[TPAMI-2015]** Ye Q, Doermann D. Text detection and recognition in imagery: A survey[J]. IEEE transactions on pattern analysis and machine intelligence, 2015, 37(7): 1480-1500. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6945320)

**[51] \[Frontiers-Comput. Sci-2016]** Zhu Y, Yao C, Bai X. Scene text detection and recognition: Recent advances and future trends[J]. Frontiers of Computer Science, 2016, 10(1): 19-36. [paper](https://link.springer.com/article/10.1007/s11704-015-4488-0)

**[52] \[arXiv-2018]** Long S, He X, Ya C. Scene Text Detection and Recognition: The Deep Learning Era[J]. arXiv preprint arXiv:1811.04256, 2018. [paper](https://arxiv.org/pdf/1811.04256.pdf)

**[53] \[NIPS-WORKSHOP-2014]** M. Jaderberg, K. Simonyan, A. Vedaldi, A. Zisserman, Synthetic data and artificial neural networks for natural scene text recognition, in: Proceedings of Advances in Neural Information Processing Deep Learn. Workshop (NIPS-W).2014. [paper](https://arxiv.org/pdf/1406.2227.pdf) [code](http://www.robots.ox.ac.uk/~vgg/publications/2014/Jaderberg14c/)

**[54] \[CVPR-2016]** A. Gupta, A. Vedaldi, A. Zisserman, Synthetic data for text localisation in natural images, in: Proceedings of Computer Vision and Pattern Recognition (CVPR), 2016, pp. 2315–2324. [paper](http://www.robots.ox.ac.uk/~ankush/textloc.pdf) [code](https://github.com/ankush-me/SynthText)

**[55] \[CVPR-2019]** Zhan F, Lu S. Esir: End-to-end scene text recognition via iterative image rectification, in: Proceedings of Computer Vision and Pattern Recognition (CVPR), 2019, pp. 2059-2068. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhan_ESIR_End-To-End_Scene_Text_Recognition_via_Iterative_Image_Rectification_CVPR_2019_paper.pdf)

**[56] \[CVPR-2019]** Zhang Y, Nie S, Liu W, et al. Sequence-To-Sequence Domain Adaptation Network for Robust Text Image Recognition, in: Proceedings of Computer Vision and Pattern Recognition (CVPR), 2019, pp. 2740-2749. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Sequence-To-Sequence_Domain_Adaptation_Network_for_Robust_Text_Image_Recognition_CVPR_2019_paper.pdf) [code](https://github.com/AprilYapingZhang/Seq2SeqAdapt)

**[57]** ICDAR2019 Robust Reading Challenge on Large-scale Street View Text with Partial Labeling. [Link](https://rrc.cvc.uab.es/?ch=16)

**[58]** ICDAR2019 Robust Reading Challenge on Arbitrary-Shaped Text. [Link](https://rrc.cvc.uab.es/?ch=14) 

**[59]** ICDAR 2019 Robust Reading Challenge on Reading Chinese Text on Signboard. [Link](https://rrc.cvc.uab.es/?ch=12)

**[60] \[arXiv-2019]**  X. Chen, T. Wang, Y. Zhu, L. Jin, and C. Luo. Adaptive Embedding Gate for Attention-Based Scene Text Recognition.[J] arXiv preprint arXiv:1908.09475, 2019. [paper](https://arxiv.org/pdf/1908.09475.pdf)

***
**Newly added references**

**[61]** \[ICFHR-2018] Wang C, Yin F, Liu C L. Memory-Augmented Attention Model for Scene Text Recognition[C] //2018 16th International Conference on Frontiers in Handwriting Recognition (ICFHR). IEEE, 2018: 62-67.  [paper](https://ieeexplore.ieee.org/abstract/document/8563227)

**[62]** \[ICCV-2019] Yang M K, Guan Y, Liao M, et al. Symmetry-constrained Rectification Network for Scene Text Recognition[J]. arXiv preprint arXiv:1908.01957, 2019. [paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Yang_Symmetry-Constrained_Rectification_Network_for_Scene_Text_Recognition_ICCV_2019_paper.pdf)

**[63]** \[ICCV-2019] Sun Y, Liu J, Liu W, et al. Chinese Street View Text: Large-scale Chinese Text Reading with Partially Supervised Learning[J]. arXiv preprint arXiv:1909.07808, 2019. [paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Sun_Chinese_Street_View_Text_Large-Scale_Chinese_Text_Reading_With_Partially_ICCV_2019_paper.pdf)

**[64]** \[ICME-2019] Wang S, Wang Y, Qin X, et al. Scene Text Recognition via Gated Cascade Attention[C]//2019 IEEE International Conference on Multimedia and Expo (ICME). IEEE, 2019: 1018-1023. [paper](https://ieeexplore.ieee.org/abstract/document/8784914)

**[65]** \[ICCV-2019] Baek J, Kim G, Lee J, et al. What is wrong with scene text recognition model comparisons? dataset and model analysis[J]. arXiv preprint arXiv:1904.01906, 2019. [paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Baek_What_Is_Wrong_With_Scene_Text_Recognition_Model_Comparisons_Dataset_ICCV_2019_paper.pdf) [code](https://github.com/clovaai/deep-text-recognition-benchmark)

**[66]** \[Nips-2017] Wang J, Hu X. Gated recurrent convolution neural network for ocr[C]//Advances in Neural Information Processing Systems. 2017: 335-344. [paper](http://papers.nips.cc/paper/6637-gated-recurrent-convolution-neural-network-for-ocr.pdf) [code](https://github.com/Jianfeng1991/GRCNN-for-OCR)

**[67]** \[NC-2019] Huang, Yunlong, et al. "EPAN: Effective parts attention network for scene text recognition." *Neurocomputing* (2019). [paper](https://www.sciencedirect.com/science/article/pii/S0925231219313839)

**[68]** \[NC-2019] Gao, Yunze, et al. "Reading scene text with fully convolutional sequence modeling." *Neurocomputing* 339 (2019): 161-170. [paper](https://www.sciencedirect.com/science/article/pii/S0925231219301870)

**[69]** \[ICDAR-2019] Qi, Xianbiao, et al. "A Novel Joint Character Categorization and Localization Approach for Character-Level Scene Text Recognition." *2019 International Conference on Document Analysis and Recognition Workshops (ICDARW)*. Vol. 5. IEEE, 2019. [paper](https://ieeexplore.ieee.org/abstract/document/8892915)

**[70]** \[ICDAR-2019] Wang, Qingqing, et al. "ReELFA: A Scene Text Recognizer with Encoded Location and Focused Attention." *2019 International Conference on Document Analysis and Recognition Workshops (ICDARW)*. Vol. 5. IEEE, 2019. [paper](https://ieeexplore.ieee.org/abstract/document/8892900)

**[71]** \[ICIP-2019] Zhu, Yiwei, et al. "Text Recognition in Images Based on Transformer with Hierarchical Attention." *2019 IEEE International Conference on Image Processing (ICIP)*. IEEE, 2019. [paper](https://ieeexplore.ieee.org/abstract/document/8803203)

**[72]** \[CVPR-2019] Zhan, Fangneng, Hongyuan Zhu, and Shijian Lu. "Spatial fusion gan for image synthesis." *Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition*. 2019. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhan_Spatial_Fusion_GAN_for_Image_Synthesis_CVPR_2019_paper.pdf)

**[73]** \[ECCV-2018] Zhan, Fangneng, Shijian Lu, and Chuhui Xue. "Verisimilar image synthesis for accurate detection and recognition of texts in scenes." *Proceedings of the European Conference on Computer Vision (ECCV)*. 2018. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Fangneng_Zhan_Verisimilar_Image_Synthesis_ECCV_2018_paper.pdf) [code](https://github.com/fnzhan/Verisimilar-Image-Synthesis-for-Accurate-Detection-and-Recognition-of-Texts-in-Scenes)

**[74]** \[MultiMedia-2018] Fang, Shancheng, et al. "Attention and language ensemble for scene text recognition with convolutional sequence modeling." *2018 ACM Multimedia Conference on Multimedia Conference*. ACM, 2018. [paper](https://dl.acm.org/citation.cfm?id=3240571) [code](https://github.com/FangShancheng/conv-ensemble-str)

**[75]** \[Nips-2018] Liu, Hu, Sheng Jin, and Changshui Zhang. "Connectionist temporal classification with maximum entropy regularization." *Advances in Neural Information Processing Systems*. 2018. [paper](http://papers.nips.cc/paper/7363-connectionist-temporal-classification-with-maximum-entropy-regularization) [code](https://github.com/liuhu-bigeye/enctc.crnn )

**[76]** \[PR-2017] Su, Bolan, and Shijian Lu. "Accurate recognition of words in scenes without character segmentation using recurrent neural network." *Pattern Recognition* 63 (2017): 397-405. [paper](https://www.sciencedirect.com/science/article/pii/S0031320316303314)

**[77]** \[CVIU-2016] Mishra, Anand, Karteek Alahari, and C. V. Jawahar. "Enhancing energy minimization framework for scene text recognition with top-down cues." *Computer Vision and Image Understanding* 145 (2016): 30-42. [paper](https://www.sciencedirect.com/science/article/pii/S107731421600014X)

**[78]** \[ICPR-2016] Liu, Xinhao, et al. "Scene text recognition with CNN classifier and WFST-based word labeling." *2016 23rd International Conference on Pattern Recognition (ICPR)*. IEEE, 2016. [paper](https://ieeexplore.ieee.org/abstract/document/7900259)  

**[79]** \[TPAMI-2019] Liao M, Lyu P, He M, et al. Mask textspotter: An end-to-end trainable neural network for spotting text with arbitrary shapes[J]. IEEE transactions on pattern analysis and machine intelligence, 2019. [paper](https://ieeexplore.ieee.org/abstract/document/8812908) [code](https://github.com/MhLiao/MaskTextSpotter)

**[80]** \[AAAI-2020] T. Wang, Y. Zhu, L. Jin, C. Luo and X. Chen. Decoupled Attention Network for Text Recognition[C]//AAAI. 2020. [paper](https://arxiv.org/abs/1912.10205) [code](https://github.com/Wang-Tianwei/Decoupled-attention-network)

***

<a id="6help"></a>

<a id="6help"></a>
## 6.Help

If you find any problems in our resources, or any good papers/codes we have missed, please inform us at xxuechen@foxmail.com. Thank you for your contribution.

***

<a id="7copyright"></a>
## 7.Copyright

Copyright © 2019 SCUT-DLVC. All Rights Reserved.

<p align="center">
    <img src="scut-dlvc.jpeg" alt="Sample"  width="150" height="75">
    <p align="center">
        <em></em>
    </p>
</p>
