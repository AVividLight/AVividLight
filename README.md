# Michael Bethke

![header](/Resources/Header/0705.png)

Thank you for viewing my profile. Please expand the sections below to find out a bit more about me, my skills and certifications, and access a guided overview of my projects.

<details>
<summary>Skills</summary>

## Top Skills

* C++
* Embedded Software Engineering
* Object-Oriented Design

|Languages||
|---|---|
|C++|C|
|Objective-C|C#|

|Tools & Technologies||
|---|---|
|Git|GitHub|
|JSON|REST APIs|
|Docker|CMake|
|SharePoint|Azure|
|Microsoft PowerApps|Microsoft PowerBI|
|Microsoft Flow|Microsoft PowerAutomate|

|Interpersonal Skills||
|---|---|
|Project Management|Administration|
|Leadership|Public Speaking|
|Organization|Teamwork|
</details>

<details>
<summary>Certifications</summary>

<br>

&emsp;[Embedded Systems and C++ (TestDome)](https://app.testdome.com/cert/5a7e81e587284d4eb45a6c25787d0990)

&emsp;[Embedded Systems and C (TestDome)](https://app.testdome.com/cert/1664d8fd9fb34203b1d26e6ac9cf4113)

&emsp;[C++, C, C#, JSON, REST APIs (LinkedIn)](https://www.linkedin.com/in/michael-bethke-081ba6140/)
</details>

<details>
<summary>More About Me</summary>

<br>

&emsp;I started teaching myself programming in middle-school, and immediately fell in love with designing systems and the structured, logical way of interfacing with computers. I've never stopped learning about software engineering and have spent time in game development, application design, embedded software, and scalable cloud-based web apps.

&emsp;My passion is writing highly-efficient code in mission-critical spaces, but I've found that good programming can get many different things done. C-based languages are my go-to, having spent many years in C++ alone, as well as pure C, C#, and Objective-C. My hobby projects range from video games to embedded applications for Arduino, and my professional experience includes embedded software for real-time operating systems and cloud-based web apps using Microsoft Azure and the Office 365 suite. I currently work at RFA Engineering as an Embedded Software Engineer.
</details>

<details>
<summary>Overview of Projects</summary>

### [glEEmail (2021)](https://github.com/Matt-and-Gib/gleemail)

---

&emsp;glEEmail is hardware and software: a real-time chat application for Arduino which features tactile Morse Code input, a robust networking layer, and end-to-end encryption. It started as a fun way to get my friend up to speed with C++ and embedded programming, so we utilized the Agile concept of Pair Programming for almost the entire project, and designed core systems in diagrams and UML prior to implementation. In addition to writing the code, we also sourced and designed the hardware.

&emsp;Processing time is critical on Arduino, especially for real-time communication and synchronization, and accurately parsing Morse Code input, so development focused on efficiency and finding creative ways to optimize performance. At it's core, glEEmail is a finite state machine alternating between getting input, reading and writing on the network, and updating the hardware (LCD and SD card), but we tried to keep physical components separate in software, so the project utilizes low coupling, respects domains, and avoids hardcoded values.

### [Markov Chain (2018)](https://github.com/AVividLight/Markov-Chain)

---

&emsp;My implementation of a Markov Chain in C++ lets users procedurally generate entirely new text based on a reference input. Incidentally, it also utilizes a framework I wrote for supporting runtime translation. Anyway, when running the Markov Chain, you provide a source body of text which the tool will parse into small pieces, then assemble into a dictionary of natural phrases. After that setup is done, it picks a random place to start in the dictionary, and starts walking through possible combinations, creating sentences and paragraphs.

&emsp;The key concept in my Markov Chain is parsing a sentence into short phrases and collecting those in a dictionary. As a simple example, if the phrase length is set to two words, this short sentence "_the honey and the bee_" is parsed into the following phrases: "the honey," "honey and," "and the," and "the bee" Once this is done for the full text, you end up with a set of phrases that can be mapped to one another. Using this example, the dictionary would look like:

|Key|Value|
|---|---|
|the|honey, bee|
|honey|and|
|and|the|

&emsp;Critically, phrases can traverse from value to key, so once the dictionary is built, traversing is simply following the mapping. When a key with multiple values is encountered (as in key "the" above), the generator makes a decision about which path to follow and continues from there. In our example, Any generated text would be trivial (and likely nonsense), but if a large source text is provided as input, the dictionary can become rich with each key containing numerous values, ultimately producing a much more complex output.

### [KISS SDL contribution (2016)](https://github.com/actsl/kiss_sdl)

---

&emsp;I was using the SDL2 library as an underlying graphics framework for a C++ project back in 2016, and needed a toolkit to provide interactive on-screen elements in the user-interface layer. I settled on KISS SDL by Tarvo Korrovits because it was lightweight and extensible, however as I integrated it, I discovered that it couldn't push high-DPI graphics to my "retina display" MacBook.

&emsp;Since KISS SDL is open source, I dug into the C library, found the functions responsible for graphics loaded from the disk, and rewrote them to be able to safely handle both standard and high-DPI images. I contacted the author in order to contribute back to the project and eventually the changes were integrated into the project. My code has been in the source since then and I was credited for my work in the project README.

### [Website for 2CatStudios (2016)](https://2catstudios.github.io/main.html)

---

&emsp;2Cat Studios was the team name that me and a friend from The Netherlands chose when we were working together on projects around 2014, and every good team needs a website. 2catstudios.github.io was built with response-time and user privacy in mind, so the focus was on primary content with no distractions. It consists of mostly static HTML and CSS, XML for our RSS feed, and light scripts written in JavaScript. The website also utilized Google Analytics to help us track usage and improve our content.

### [UnityMusicPlayer (2014)](https://github.com/2CatStudios/UnityMusicPlayer)

---

&emsp;UnityMusicPlayer is a local-disk, audio streaming program with an embedded online store and real-time audio visualization and audio effects. It was written using C#, XML, and GLSL, in the Unity3D engine. I originally designed it to replace iTunes for my personal music library, so its initial functionality was limited to music organization and playback, however user feedback prompted the development of features for live DJ performances, and UMP was used for a least one live event.

&emsp;Later, feedback from musicians lead me to implement a music store which helped promote independent musicians and enable music discovery for listeners. All available downloads were set up with the artists' permission, however some files were encrypted to ensure that playback was limited to UnityMusicPlayer.

</details>
