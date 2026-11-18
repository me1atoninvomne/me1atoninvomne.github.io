# me1atoninvomne.github.io

**Live site: https://me1atoninvomne.github.io**

My personal portfolio site, built as a small retro operating system: **Avlastymov XP**. It boots, shows a desktop with icons, draggable windows, a taskbar and a start menu. Inside the windows you can build a computer in 3D, run an estimated benchmark, play a QA mini game and look at my projects.

## Why I built it

- **To show my work, not just describe it.** A recruiter can open one link and try everything in under a minute.
- **To turn a hobby into a project.** I like PC hardware, so I used it to combine what I do every day: data and rules (compatibility checks, power calculations), a clear interface and automation.
- **To practise new skills.** 3D graphics in the browser, plain JavaScript without frameworks, and publishing my own website with GitHub Pages.

## Features

**Avlastymov XP desktop** (`index.html`)
- **Two ways in**: the site first asks who you are. Recruiters get a **recruiter view**: the whole resume on one page, with contacts and a "print or save as PDF" button. Everyone else gets a dark room with an old computer that is switched off, and has to press its power button themselves.
- **Four languages**: after the computer starts you pick Ukrainian, English, German or Chinese on a screen styled like the XP log-on screen. The language can be changed any time from the taskbar, and the PC Builder follows it.
- **Live GitHub activity**: a window with my public repositories, languages and recent activity, loaded live from the GitHub API.
- **Link preview**: sharing the link in a chat or on LinkedIn shows a preview card.
- **3D intro**: an old coder's desk (a beige 90s tower with a MHz display and made-up stickers, a made-up local beer, an ashtray, floppy disks and a TODO sticky note) powers on when you press the button, and the CRT runs a BIOS check that lists the parts of *your* build from the PC Builder (and my skills) before the camera flies into the screen.
- **Applecat, the desktop assistant** (drawn by me): on the first visit it explains that the whole site is one big resume. Click it for a tour of the best features, the resume, a guided PC Builder walkthrough, or an original song it sings with music synthesised in the browser. You can drag and throw it (it has physics and always lands on the taskbar), but poke or throw it too much and it turns redder, steams and stomps, then sulks or yells gibberish; throw it really hard and it cries and runs away from your cursor.
- **Hacker mode screensaver**: after 2 minutes without input the screen turns into a movie-style "hack" (code rain, memory dump, trace route). The hacker keeps typing each command in English, then Chinese, then forgets to switch the keyboard layout, and finally gets it right in Ukrainian. Type `hack` in the terminal to start it right away.
- **Boot screen, desktop and windows**: draggable, resizable windows with minimise / maximise / close, a taskbar, a start menu, a clock and a live waveform wallpaper that reacts to the stress test.
- **Apps**: Home, My Computer (your build), Projects (explorer), PC Builder, Bug Hunter, Terminal, Task Manager, Resume, Contact (mail form), Avlamp (music synthesised in the browser) and a Recycle Bin.
- **Classic games** in the top-right corner: Minesweeper (3 levels, flags, best times), Solitaire (Klondike with drag and drop and the bouncing-cards win screen) and Paint (brush, shapes, fill, colour picker, undo, save as PNG).
- **Rubber-band selection** of desktop icons, like on Windows.
- **3D PC model** of your current build on a retro monitor: rotate it, open an exploded view, or pull out any part and turn it in your hands.
- **Bench widgets**: a sensor monitor (simulated temperatures, stress test, fan curve), an RGB controller that lights the model, a terminal (`help`, `whoami`, `skills`, `projects`, `build`, `game`) and a "your build" card.
- **Projects with live previews**: an animated n8n workflow, a prompt benchmark run, API calls and an invoice check.
- **Bug Hunter**: a small QA game. A fake online shop hides 6 random bugs (wrong maths, typos, impossible values); find them in 60 seconds and file the bug reports.

**PC Builder page** (`builder.html`)
- **134 real components** in 8 categories: CPU, cooler, motherboard, graphics card, memory, SSD, power supply and case, plus ready-made presets.
- **The 3D model rebuilds from your choice**: GPU length, thickness and fan count, air tower or liquid cooler with radiator, memory height and RGB, board size and colours, case colour and front panel.
- **Details down to the small parts**: motherboard screws and capacitors, socket lever, thermal paste, 24-pin, 8-pin EPS and GPU power cables, rear I/O ports, PCIe slot covers.
- **Step-by-step assembly** in 11 steps, in the real order: board, CPU, thermal paste, cooler, RAM, SSD, GPU, PSU, cables, fans, side panel.
- **Compatibility checks**: socket, board size against the case, GPU length and cooler height against the case, cooler against CPU power, power supply headroom, CPU/GPU balance.
- **Benchmark**: an animated run through 5 games and 3 synthetic tests with estimated FPS at 1080p, 1440p or 4K, CPU/GPU bottleneck and a comparison with other builds. If the parts are not compatible, the PC "fails to boot".
- The build is saved in the browser and shows up on the home page too.

## How it is made

- Plain HTML, CSS and JavaScript: no build step, no frameworks. `pc.js` holds the parts catalogue and the 3D model and is shared by both pages.
- [three.js](https://threejs.org) for the 3D scene. All textures are drawn in code on a canvas, so the site uses no image files.
- Every part is generated from data (size, colours, fan count), so adding a new product takes one line in the catalogue.
- Hosted on GitHub Pages.

## Notes

Prices are examples, sizes are approximate, and the sensor values and benchmark results are estimates, not measurements. The 3D models are simplified versions of the real products. Product names belong to their owners.

## Contact

slekktt@gmail.com · [GitHub profile](https://github.com/me1atoninvomne)
