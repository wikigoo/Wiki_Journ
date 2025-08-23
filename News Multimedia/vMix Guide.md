

# **The Complete Guide to vMix: Mastering Live Video Production and Streaming**

vMix stands as a powerful and versatile software solution for live video production, recording, and streaming. This guide offers a comprehensive exploration of its features, functionalities, and workflows, designed to equip users with the knowledge to harness vMix's full potential, from initial setup to advanced operations and customization.

Section 1: Introduction to vMix: Your Live Production Powerhouse

1.1 What is vMix? Core Capabilities and Use Cases.

vMix is a feature-rich live production software application that empowers users to record and stream professional-quality productions entirely from a single PC or Laptop. It offers robust support for Standard Definition (SD), High Definition (HD), and 4K video productions.1 The software's capabilities are extensive, encompassing video capture from various sources, seamless integration of Network Device Interface (NDI) feeds, playback of local video and audio files, creation of immersive virtual sets, dynamic title generation, and comprehensive audio mixing. Furthermore, vMix provides a suite of live video effects, multi-view configurations, sophisticated overlay management, playlist automation, and the ability to output to multiple formats simultaneously, including direct screen display, local recording, external hardware outputs, and live streaming to numerous online platforms. Advanced features such as multi-corder for isolated recordings, an integrated instant replay system, Pan-Tilt-Zoom (PTZ) camera control, and the vMix Call system for remote guest integration further solidify its position as a comprehensive production tool.1

The software's wide-ranging feature set makes it suitable for a diverse array of use cases. From individual content creators streaming to online platforms, educational institutions producing online lectures, houses of worship broadcasting services, corporate entities conducting webinars and live events, to even more complex sports productions requiring instant replay and multi-camera setups, vMix offers tools to meet these demands. The inherent scalability, demonstrated by its support for SD, HD, and 4K resolutions alongside a feature list that covers basic switching to intricate multi-camera replay and remote guest integration, allows users to begin with simpler configurations and expand their production complexity as their needs evolve, all within the same software environment.1 A core design philosophy appears to be the consolidation of numerous production tasks onto a single computer, which can offer significant efficiencies and cost savings compared to traditional broadcast workflows that often rely on multiple pieces of dedicated hardware.1

1.2 Overview of vMix Editions.

vMix is offered in several editions, with features tiered to cater to different user requirements and budgets. While the foundational live production capabilities are present across the board, more advanced functionalities are typically reserved for higher-tier versions. For instance, features like MultiCorder (for recording multiple isolated camera feeds), the sophisticated Instant Replay system, and the ability to use Scripting for advanced automation are primarily found in the vMix 4K and Pro Editions.1 The number of remote guests that can be integrated using vMix Call also varies by edition: vMix HD supports one guest, vMix 4K supports four guests, and vMix Pro allows for up to eight guests.1 Even features like Stinger Transitions, which utilize animated graphics for scene changes, are available in editions that support more than one overlay channel, such as vMix HD, indicating that even mid-tier versions possess significant capabilities.1

This tiered approach means that users must carefully assess their current and anticipated production needs when selecting an edition. However, the availability of core switching, basic recording and streaming, and a wide array of input types even in lower editions ensures that vMix remains an accessible option for those starting out, with a clear upgrade path as their requirements grow more complex.1

1.3 Understanding the vMix Ecosystem.

vMix is designed to function as a central hub within a broader production ecosystem, rather than a standalone, isolated application. It demonstrates extensive interoperability by integrating seamlessly with a variety of hardware components, other software applications, and web-based services. Hardware compatibility includes a wide range of video capture cards from manufacturers like AJA, Blackmagic Design, and Magewell, PTZ cameras controllable over the network, and various control surfaces including MIDI controllers and Elgato Stream Decks.1

On the software side, vMix embraces open and widely adopted standards. Its robust support for NDI allows for easy integration of video and audio sources from other NDI-enabled software and devices on the local network.1 It can interface with external streaming applications like Adobe Flash Media Live Encoder (FMLE), though FFMPEG is often the preferred built-in option, and supports VST3 audio plugins for expanded audio processing capabilities.1 Furthermore, vMix connects with numerous web services, facilitating direct streaming to popular platforms like YouTube Live and Facebook Live, integrating dynamic data into titles from sources like Google Sheets, and enabling remote guest participation through its vMix Call feature.1 This commitment to interoperability provides users with significant flexibility in designing their production workflows and integrating vMix with existing equipment or preferred third-party tools. The software-defined nature of vMix also means its performance and capabilities are directly amplified by the power of the underlying PC hardware, including CPU, GPU, and storage solutions, allowing the system to scale with hardware advancements.2

---

Section 2: Getting Started with vMix

2.1 System Requirements: Ensuring Your PC is Ready.

Before diving into vMix, it is crucial to ensure that the host computer meets the necessary system requirements. An underpowered system can lead to performance issues such as dropped frames, instability, and an overall unsatisfactory user experience. vMix provides general minimum and recommended specifications, but these can vary based on the complexity of the production, the resolution (SD, HD, 4K), and the use of demanding features like Instant Replay.2 For comprehensive and up-to-date details on supported hardware, users are directed to the official vMix website.1

A key takeaway from the system requirements is the critical role of storage speed, particularly for advanced features. The documentation explicitly recommends a "Dedicated SSD for Replay" and even "NVME SSD" for higher-channel Instant Replay configurations, with a general recommendation for a "Solid State Disk" for recordings.1 This emphasis arises because traditional Hard Disk Drives (HDDs), even those operating at 7200 RPM (listed as a minimum), often struggle with the sustained high-bitrate write speeds required for recording multiple HD or 4K video streams simultaneously. SSDs, and especially NVMe SSDs, offer vastly superior input/output performance, which directly impacts the reliability and capability of data-intensive tasks like multi-channel recording and the Instant Replay system.

The choice of Graphics Processing Unit (GPU) also significantly influences vMix's performance and feature availability. The general recommendation is for a "Dedicated Nvidia Card with 2GB+ Memory," with specific NVIDIA GeForce GTX models cited for different tiers of Instant Replay functionality.2 The GPU's role extends beyond merely displaying the interface; vMix leverages it for video processing, rendering effects, and hardware-accelerated encoding and decoding, such as for H.264 streaming or HEVC for SRT.1 Consequently, the GPU selection directly affects how many inputs, outputs, and advanced features can be run smoothly. NVIDIA GPUs are frequently mentioned, suggesting optimized support. A critical detail for users planning multiple simultaneous hardware-encoded operations is the typical two-encode limit on NVIDIA GeForce series cards, a restriction not usually found on their Quadro series counterparts.1

Table 2.1: Detailed vMix System Requirements.

|  |  |  |  |  |  |
| :---- | :---- | :---- | :---- | :---- | :---- |
| Component | Minimum (General) | Recommended (General) | 1-Channel HD Replay | 4-Channel HD / 1-Channel 4K Replay | 8-Channel HD / 2-Channel 4K Replay |
| Operating System | Windows 10 / 11 | Windows 10 / 11 | Windows 10 (64 bit only) | Windows 10 (64 bit only) | Windows 10 (64 bit only) |
| Processor | 2Ghz Quad-Core | Intel Core i7 3Ghz+ | Quad Core 3.4 Ghz | Six Core 3.6 Ghz | 18 Core 3.0 Ghz |
| Memory | 4GB DDR4 | 8GB DDR4 | 8GB DDR4 | 8GB DDR4 | 16GB DDR4 |
| Hard Drive | 7200 RPM HDD | Solid State Disk (SSD) | Dedicated SSD (200GB+) | Dedicated SSD (500GB+, 1TB recommended) | NVME SSD (min 500MB/s R/W) |
| Graphics Card | DirectX 10.1 Compatible | Dedicated Nvidia (2GB+) | NVIDIA GeForce GTX 1050+ | NVIDIA GeForce GTX 1060+ | NVIDIA GeForce GTX 1080 Ti+ |
| Screen Resolution | 1920x1080 | 1920x1080 | 1920x1080 | 1920x1080 | 1920x1080 |
| Storage Connection | N/A | N/A | Internal SATA or M.2 | Internal SATA 3, M.2 (M.2 recommended) | M.2 only |

This table consolidates critical hardware information, allowing users to quickly assess their needs based on intended use, particularly for demanding features like Instant Replay.

2.2 Installation and Initial Setup.

The installation process for vMix follows standard software procedures. The primary software package, along with utilities like the vMix Desktop Capture application, can be downloaded from the official vMix website (e.g., [http://www.vmix.com/software/download.aspx](http://www.vmix.com/software/download.aspx) is cited for the Desktop Capture tool).1 Once downloaded, running the installer will guide the user through the setup steps. After installation, vMix requires activation using a registration key. The software provides an interface for changing or upgrading this registration key, typically found within the "About" section of the settings.1 This centralized download and internal licensing mechanism is typical for professional software applications.

2.3 Navigating the vMix User Interface: A Guided Tour.

The vMix user interface is designed with live video mixing in mind and may appear familiar to those who have worked with traditional hardware video switchers.1 This design choice aims to provide a degree of comfort and a potentially lower learning curve for experienced operators transitioning to a software-based solution. The main window is organized into several key areas 1:

- Output Window: Prominently located in the top-right corner and distinguished by a green title bar, this window displays the final live program output. This is what is being recorded, streamed, or sent to a fullscreen display.  
    
- Preview Window: Positioned in the top-left corner with an orange title bar, the Preview Window serves as a staging area. Inputs are typically selected here before being transitioned to the Output Window.  
    
- Tabs: On the left side of the input area, color-coded tabs allow users to organize their inputs into categories for better management. On the right side of the main interface, tabs can be used to dock frequently accessed feature windows, such as the Audio Mixer or the Instant Replay Controller.1 This customization aids in creating an efficient, personalized workspace.  
    
- Input Bar: This area, typically at the bottom of the interface, displays all loaded sources (cameras, videos, titles, etc.). Each input shows a small, real-time preview thumbnail. Clicking an input queues it in the Preview Window, while double-clicking opens its detailed settings window. Multiple rows of inputs can be displayed to accommodate a large number of sources.1  
    
- Footer Bar: Located at the very bottom of the main window, this bar contains essential global controls, including the "Add Input" button and buttons for configuring and initiating Recordings, Streams, and External Outputs.1

This Preview/Program bus concept is a staple of hardware vision mixers, and its adoption in vMix facilitates a more intuitive experience for users familiar with such equipment.

2.4 Working with Presets: Saving and Loading Your Production Setups.

Presets in vMix are a powerful feature for saving and quickly recalling complete production configurations. They are crucial for efficiency, especially for users who produce recurring shows or manage different types of events.1 A preset is designed to be a comprehensive snapshot of the production environment, storing a wide array of settings, including 1:

- All added inputs and their associated settings (such as position, color adjustments, chroma key configurations, and multiview layouts).  
    
- Recording settings.  
    
- Overlay configurations and settings.  
    
- Locally defined shortcut keys and activators.  
    
- Audio settings for each input and for all audio buses (Master, A, and B).  
    
- All created PlayLists, including the currently active one if applicable.  
    
- Custom category labels.  
    
- Streaming settings, including all saved profiles (which will replace any existing streaming settings when the preset is loaded).  
    
- External Output settings (size, frame rate, device).  
    
- Outputs configuration (e.g., if MultiView is selected for the Fullscreen output).  
    
- Data Sources and their related settings.  
    
- The master frame rate and output size of the production.

When loading a preset, if the saved master frame rate or output size differs from the current vMix configuration, a confirmation message will appear.1 It is important to note a critical practical consideration regarding media assets (videos, images, title templates, etc.): these are referenced by their filename and path only. Presets do not embed the media files themselves. Therefore, if a preset is moved to a different computer or if media files are reorganized, it is essential to copy these assets and ensure they are placed in the same folder locations as when the preset was saved, otherwise, the inputs will fail to load correctly.1 This underscores the importance of maintaining good media management practices when working with vMix presets.

vMix provides the following preset management options, typically found in the top-left corner of the interface 1:

- New Preset: Creates a new, blank production environment and optionally allows changing the current output video format.  
    
- Open Preset: Opens a file dialog to select an existing preset file. Upon selection, users are presented with two choices:  
    
- Open: Closes all currently open inputs and replaces the entire session with the contents and settings from the selected preset.  
    
- Append: Adds the inputs from the selected preset to the existing session while ignoring all other settings (like streaming or recording configurations) from the preset file. This offers flexibility in merging components from different productions.  
    
- Save Preset: Saves the current production configuration to a preset file.  
    
- Last Preset: vMix periodically and automatically saves the current state of the production to a separate recovery file. The "Last" button allows users to load this automatically saved preset, which can be invaluable in case of an unexpected shutdown or error.

The comprehensive nature of what is stored within a preset makes it a powerful tool for minimizing setup time and ensuring consistency across productions.

---

Section 3: Mastering Inputs: The Building Blocks of Your Production

Inputs are the fundamental components of any vMix production, representing all the various sources that can be mixed, recorded, or streamed. Understanding how to add and configure these inputs is key to leveraging vMix's capabilities.

3.1 The "Add Input" Window: Your Gateway to Sources.

The primary method for introducing content into a vMix session is through the "Add Input" window. This window is accessed by clicking the "Add Input" button, typically located in the footer bar of the main vMix interface.1 Upon clicking, a dialog appears, presenting a categorized list of all the different types of sources that vMix can handle.1 The sheer breadth of natively supported input types is a testament to vMix's design philosophy of providing a comprehensive, all-in-one solution. These types include, but are not limited to: Video files, DVDs, Lists (playlists of video/audio), Cameras (via capture cards), NDI / Desktop Capture, Streams (RTSP/SRT), Instant Replay feeds, Image Sequences (often used for stingers), Video Delay, single Images, folders of Photos, PowerPoint presentations, solid Colours, Audio files, dedicated Audio Inputs (for microphones/external mixers), Titles / XAML (including GT Titles), Virtual Sets, Web Browser content, vMix Call remote guests, and even other vMix Mix inputs.1 This extensive list means users can often ingest a wide array of media and sources directly, reducing the need for external conversion tools or numerous third-party applications and thereby simplifying the overall production chain.

3.2 Common Input Types and Configuration.

Each input type has its own specific configuration options, tailored to the nature of the source.

3.2.1 Video Files (AVI, MP4, etc.) and DVDs.

vMix supports a wide range of common video file formats for playback, including AVI, MPG, MXF, MP4, WMV, and QuickTime.1 When adding a video file, users can specify custom start (Mark In) and end (Mark Out) points for playback.1 This basic, NLE-like functionality allows for non-destructive trimming of clips directly within the live environment, which is useful for cueing specific segments without needing to pre-edit every file externally, thereby speeding up the preparation workflow.

For DVD playback, users can select either a physical DVD drive or a folder containing DVD files. vMix supports navigation of DVD menus directly from the Preview or Output windows by clicking on menu items. Additionally, right-clicking the DVD input window provides options to manually select chapters or return to the main menu.1

3.2.2 Cameras and Capture Devices.

Live camera feeds are typically brought into vMix using compatible video capture devices. The "Camera" input type allows users to select their installed capture card and configure its settings.1 These settings include selecting the specific physical input on the card (e.g., SDI 1, HDMI 2), the desired resolution and frame rate, and whether the source is interlaced (including support for Progressive Segmented Frame, or PsF, formats). Users can also specify the video format if the card supports multiple (e.g., YUY2, YV12). An extensive list of officially supported capture cards from various manufacturers like AJA, Blackmagic Design, and AVerMedia can be found on the vMix website.2

Audio from cameras can also be configured, including selecting specific embedded audio inputs. For certain cards (e.g., from AJA, Blackmagic, Magewell), an "EmbeddedAllChannels" option may be available, allowing vMix to ingest up to 8 channels of audio simultaneously from an SDI or HDMI source, which can then be managed in the vMix Audio Mixer.1 This deep level of hardware integration and control, allowing fine-grained adjustments to how the capture hardware delivers the signal, is crucial for achieving professional quality and for effective troubleshooting.

3.2.3 NDI Sources: Local and Remote Desktop Capture.

Network Device Interface (NDI) is a cornerstone of modern IP-based video workflows, and vMix provides comprehensive support for it, both for receiving and sending NDI streams.1 NDI effectively acts as a flexible "virtual" cabling system, allowing for easier setup of distributed workflows and the capture of non-traditional sources.

To add an NDI source, users select the "NDI / Desktop Capture" input type. vMix will automatically discover and list available NDI sources on the local network, complete with preview thumbnails.1 This can include outputs from other NDI-enabled software, hardware devices, or even other vMix instances.

A particularly useful feature is the ability to capture remote computer desktops. By running the free vMix Desktop Capture application (available for PC and Mac) on a remote computer on the same network, its screen or individual application windows become available as NDI sources in the main vMix system.1 This is invaluable for bringing in presentations, software demonstrations, or gaming feeds.

vMix also offers "Local Desktop Capture," which allows for high-performance, full-frame-rate capture of screens or windows from the same computer running vMix.1 This is excellent for capturing applications like Skype or web browsers without needing a second computer or complex routing.

When working with NDI inputs, several options are available to manage performance and quality 1:

- Low Bandwidth Mode: Switches the NDI feed to a lower resolution and bandwidth version, useful for congested networks.  
    
- Audio Only: Disables video and brings in only the audio from the NDI source.  
    
- PsF (Progressive Segmented Frame): Should be ticked if the NDI source is a camera sending progressive video over an interlaced signal, to improve video quality.  
    
- Increase Buffer Size: Can help smooth out video playback on unstable or wireless networks, though it will increase latency by approximately five frames. These options acknowledge that network conditions can impact NDI performance and provide users with tools to mitigate potential issues by trading off quality or latency for stability.

3.2.4 Streaming Inputs (RTSP, SRT).

vMix can ingest live streams from IP cameras and streaming servers using various protocols. The "Stream / SRT" input type supports RTSP (Real Time Streaming Protocol), Transport Streams (delivered via UDP or TCP), and SRT (Secure Reliable Transport).1

For RTSP sources, such as many IP cameras or Teradek Cube encoders, users enter the RTSP URL (e.g., rtsp://\<ip\_address\>/stream1). Options include specifying RTSP over UDP or TCP, setting a network buffer (in milliseconds, to reduce jitter), and enabling a "Low Latency Mode" for compatible devices, which can achieve sub-5-frame delay if the buffer is set to 0.1

SRT is a more recent protocol designed for reliable video transport over unpredictable networks like the public internet. vMix supports SRT in three connection modes:

- Caller: vMix initiates the connection to a remote SRT listener.  
    
- Listener: vMix waits for an incoming connection from an SRT caller on a specified port.  
    
- Rendezvous: Both vMix and the remote end are set to Rendezvous mode with an identical port number, facilitating connection through most firewalls automatically. SRT configuration includes setting the Hostname (for Caller/Rendezvous), Port, Latency (in milliseconds, to adapt to network congestion – typically at least 4x the ping time), and an optional Passphrase for AES encryption (up to 256-bit).1 SRT inputs in vMix can utilize H.264 or HEVC video codecs with AAC audio. The inclusion of SRT, particularly its Rendezvous mode and robust error correction, positions vMix as a strong tool for ingesting remote feeds over the internet, a critical capability for modern distributed productions.

3.2.5 Images, Photos, and PowerPoint Presentations.

vMix handles static visual media through several input types 1:

- Image: For adding individual image files in formats like PNG, JPEG, TIFF, or BMP.  
    
- Photos: This input type loads all photos from a specified directory into a single vMix input. A "SlideShow Settings" window (accessible via right-click menu or cog icon menu) allows users to select which photo to display, set transition effects between photos, and define the duration each photo is shown, enabling basic automated slideshows.1  
    
- PowerPoint: Loads Microsoft PowerPoint presentations directly into vMix. This requires a copy of PowerPoint to be installed on the vMix computer. Similar to the Photos input, a "SlideShow Settings" window is available for controlling slide transitions and timing.1 This integrated slideshow functionality for Photos and PowerPoint provides a convenient way to manage presentations directly within vMix, reducing the need for manual advancement or separate presentation software for many common use cases.

3.2.6 Audio Inputs and Audio Files.

vMix provides dedicated inputs for audio-only sources 1:

- Audio: For playing back audio files, such as MP3 and WAV.  
    
- Audio Input: This versatile input type allows users to add multiple discrete audio sources to their production, such as microphones connected via USB audio interfaces, line-level inputs from external audio mixers, or sources compatible with ASIO (Audio Stream Input/Output) drivers. Each "Audio Input" can be independently controlled from the vMix Audio Mixer, effectively turning vMix into a capable audio console for many users. Configuration options include selecting the Audio Device and the specific Channels from that device (e.g., a stereo pair or a single mono channel).1 This integrated audio capability can simplify setups by reducing the need for an external hardware mixer in many common scenarios, especially when combined with vMix's built-in audio processing features like EQ, compression, and audio buses.

3.2.7 Titles and XAML (including GT Title Designer overview).

Professional-looking titles and graphics are essential for high production value, and vMix offers robust tools for this.1 The "Title / XAML" input type is used to bring in titles, lower thirds, and other graphical elements. Users can select from a variety of built-in title templates or create their own custom templates using the GT Title Designer.1 GT Title Designer is a dedicated application for creating high-quality, GPU-accelerated title templates, which can include animations (animations are supported in the 4K and Pro editions of vMix, though built-in GT templates work in all editions).1 The emphasis on GT Designer for GPU-accelerated graphics signifies a move towards more sophisticated and performant titling capabilities. A legacy "vMix Title Designer" is also mentioned for older format files.1

Once a title input is added, its text content can be easily edited by right-clicking the input and selecting "Title Editor." The Title Editor allows for modification of text fields, and users can save different sets of text as "Title Presets" for quick recall during a production.1 Titles can also feature dynamic elements like countdown timers, which can be configured with specific durations, stop/start times, and display formats.1 The ability to use Title Presets and dynamic elements like countdowns, coupled with the later-discussed Data Sources feature, means that titles in vMix are not merely static text but can be highly dynamic and data-driven, crucial for live event information.

3.2.8 Web Browser Inputs.

The "Web Browser" input allows users to integrate any web page directly into their vMix production.1 Configuration involves specifying the URL of the web page, and optionally setting a custom Width and Height for rendering the page. This is particularly useful for HTML-based widgets or alerts that are designed for specific dimensions and may be used as overlays.1

Once added, the web page can be controlled using the mouse within the vMix input window or the Preview/Output windows. Keyboard input can also be enabled via a right-click menu option, though this will temporarily disable vMix's own keyboard shortcuts.1 A significant capability of the Web Browser input is its support for transparent backgrounds and alpha channels, making it ideal for integrating web-based graphics like those from TwitchAlerts or custom-designed HTML overlays. To achieve transparency, the web page's element should not have a background color specified.1

The Web Browser input leverages the Chromium Embedded Framework (CEF), providing compatibility with most features of the Google Chrome browser, including HTML5 video and audio playback, and WebRTC.1 Audio from web browser inputs is fully supported and can be independently mixed within the vMix Audio Mixer, eliminating the need for desktop audio capture workarounds.1 This ability to pull in live web pages, including those with transparency and rich media, opens up a vast range of possibilities for incorporating dynamic, real-time information and graphics from the internet, such as streaming overlays, social media feeds, or custom web-based scoreboards, without needing to recreate such content natively.

3.2.9 vMix Call.

vMix Call is an integrated solution for adding remote guests to a production using only a web browser and a webcam.1 It supports guests connecting via Google Chrome, Firefox, and Safari (on iOS 11+) across Windows, Mac, Android, and iOS devices. Key features include peer-to-peer encryption for secure, low-latency connections, "Auto Mix Minus" technology to automatically prevent audio echo for guests, full-duplex high-quality audio, and a configurable return video/audio feed for each guest (up to HD 1080p at 4Mbps). The number of guests supported depends on the vMix edition: 1 for HD, 4 for 4K, and 8 for Pro.1

The browser-based approach of vMix Call significantly lowers the technical barrier for remote guests compared to solutions requiring software installations or complex configurations, which is paramount for smooth remote productions. The Auto Mix Minus feature further simplifies the audio setup for the vMix operator.1

3.2.10 Virtual Sets.

vMix's Virtual Set feature allows users to integrate a live, chroma-keyed camera feed (typically of a person in front of a green or blue screen) and other graphic elements into a real-time 3D rendered virtual environment.1 These virtual sets can be smoothly zoomed and panned, mimicking the look of a professional television studio, even without the physical space or budget for one. Setup involves choosing from one of the built-in Virtual Set presets. Control is managed through two tabs within the Virtual Set input: the "Camera" tab for selecting pre-defined camera angles and zoom speeds, and the "Setup" tab for customizing layers within the set, such as the background, on-screen graphics (e.g., a video playing on a virtual monitor), and the position and visibility of the keyed talent.1 This feature offers a cost-effective way to achieve sophisticated visual presentations.

3.2.11 Mix Inputs (4K/Pro Editions).

Available in the 4K and Pro editions of vMix, the "Mix" input type allows users to add up to three additional "mini mixers" within their main vMix production.1 Each Mix input can take two other vMix inputs and perform basic transitions (cuts and fades with customizable effects) between them. The input preview window for a Mix input conveniently shows both its internal Preview and Output windows side-by-side.1

This feature enables more complex layered compositions or the management of separate sub-mixes. For example, a multi-camera view of a panel discussion could be pre-switched within a Mix input, and then that Mix input's output can be treated as a single camera source in the main vMix production. However, Mix inputs have some restrictions: they do not support stinger transitions, overlays (these would need to be manually set up using the standard input MultiView feature if desired on the Mix input's sources), automatic play/pause/restart of their internal inputs, automatic audio mixing, or T-Bar transitions.1 These limitations indicate that Mix inputs are designed for specific sub-mixing or composition use cases rather than replicating the full functionality of a main vMix instance.

3.3 Input Settings In-Depth.

Every input in vMix has a comprehensive set of settings that can be accessed by clicking the cog icon (⚙️) underneath its preview thumbnail in the Input Bar, or by double-clicking the thumbnail itself.1 These settings provide granular control over an input's appearance, behavior, and interaction within the production. Key tabs within the Input Settings window include:

- General: Allows changing the input's display Name, manually setting its Aspect Ratio, enabling Deinterlace (Blend method) or Sharpen effects, and applying a horizontal Mirror. It also contains toggles for automatic audio mixing and automatic play/restart/pause behaviors linked to transitions. The Change button allows swapping the source of the input (e.g., changing which camera feed it uses) while preserving all other settings like color adjustments or multiview configurations. The Create Virtual Input option copies the current input and its settings into a new, dependent input; if the original source is closed, the virtual input becomes blank.1  
    
- Colour Adjust: Provides controls for Black Stretch (increasing black level), White Stretch (increasing white level/brightness), independent adjustment of Red, Green, Blue channels, Alpha (transparency), and Saturation. A Premultiplied Alpha checkbox is available for sources using this alpha channel format (common in MOV files).1  
    
- Colour Correction: Offers professional-grade color correction tools using industry-standard Lift (adjusts darks/shadows), Gamma (adjusts mid-tones), and Gain (adjusts brights/highlights) controls, presented as color wheels or individual RGB bars. It also includes Hue and Saturation adjustments, a Basic Auto Correct button, and the ability to save/load color correction Presets.1 These adjustments are applied in real-time and non-destructively.  
    
- Colour Key / Chroma Key: Enables transparency effects. Auto Colour Key allows selecting a color directly from the input to make transparent. Tolerance adjusts how closely vMix matches the keyed color. For green/blue screen work, Chroma Key (with an associated Chroma Key Filter to reduce green/blue halos) and Auto Chroma Key Presets provide specialized tools. Luma Key keys out the background based on brightness. A Key/Fill Input option allows using another input as the key channel.1  
    
- Layer / Multi View: A powerful compositing tool allowing up to 10 inputs (layers) to be combined into a single input, creating effects like split-screens or complex picture-in-picture arrangements. Each layer can be selected from existing vMix inputs and positioned by dragging within a preview box (Shift+drag to resize) or via the Position tab. The Z-order (which layer is on top) is determined by the layer number (10 is topmost). Layouts of these 10 layers (position, border, crop) can be saved as templates and imported/exported.1 This makes vMix a potent tool for creating sophisticated on-screen presentations.  
    
- Position: Adjusts the Zoom, Pan X/Y, and Rotate of the input (or a selected layer within Multi View). It also provides Crop X1/X2/Y1/Y2 controls to trim the edges of the input.1  
    
- Triggers: Allows for event-driven automation directly tied to an input's lifecycle. Triggers can execute functions (like playing another input, showing an overlay, or running a script) based on events such as OnTransitionIn (input starts transitioning to Output), OnTransitionOut, OnOverlayIn (input is activated as an overlay), OnOverlayOut, OnCompletion (video/list/photos/PowerPoint input finishes, if not looping), or OnCountdownCompleted (a title's countdown timer reaches zero). Multiple triggers can be added, each with a specific function, target input, duration, and delay. Triggers run sequentially as listed for the same event type. There is a maximum duration of 30 seconds for trigger delays/actions to prevent unexpected long-running operations; longer sequences should use PlayList or Scripting.1 This feature can significantly simplify complex cue sequences for operators.  
    
- Tally Light: Configures tally light settings if using Arduino-based hardware.1  
    
- PTZ: Configures Pan-Tilt-Zoom camera control if the input is a PTZ camera.1  
    
- Advanced: Contains settings like DirectShow Filters for the input and a Delay option (in frames) for capture inputs.1  
    
- Copy From: Allows copying selected settings (Triggers, Multi View, Colour Adjust/Key/Correction) from another input to the current one.1

3.4 Organizing Inputs: Categories and Input Rows.

For productions with a large number of inputs, organization is key to maintaining an efficient workflow. vMix provides two main tools for this:

- Categories: Inputs can be assigned to one of six color-coded categories: RED, GREEN, ORANGE, PURPLE, AQUA, and BLUE. These category buttons are displayed on the left side of the Inputs Row. Users can assign custom labels to these categories (e.g., "Cameras" for RED, "Videos" for GREEN) by right-clicking any category button. An input's category can be changed by dragging its preview thumbnail onto the desired category button or by selecting the category in the input's General settings. The input's cog icon will change color to match its assigned category.1  
    
- Input Rows: The main vMix window can display multiple rows of inputs. The dividing line between the input rows and the Preview/Output windows can be dragged up or down to show more or fewer rows, depending on screen resolution (1920x1080 is recommended for up to three rows). If more inputs are added than can be displayed, a scroll bar appears.1

These visual organization tools are crucial for managing potentially dozens of inputs in complex productions, helping the operator quickly locate the correct source and reducing cognitive load in a high-pressure live environment.

---

Section 4: Live Switching and Video Effects

Live switching is the core of any live production, and vMix provides a robust set of tools for transitioning between video sources and applying visual effects. The fundamental workflow involves selecting a source in the Preview Window and then using a transition control to move it to the Output Window.1

4.1 The Art of the Transition: Cut, Fade, Wipe, and More.

vMix offers a balance of simple, one-click transitions for speed and customizable options for more stylized changes, catering to various operational needs and production aesthetics.1

- Cut Button: This provides an instantaneous switch from the Preview Window to the Output Window, with no transition effect or delay.1 It is often the fastest and cleanest way to change sources.  
    
- Quick Play Button: When this button is pressed, the input currently in the Preview Window automatically transitions to the Output Window. If the input is a video clip, it will also start playing from its current position. Each input also has its own Quick Play button for direct activation. By default, Quick Play uses a half-second fade, but this transition effect and its duration can be customized in Settings \-\> Options.1  
    
- Customizable Transition Buttons: vMix features four main transition buttons located in the center of the interface, below the Preview and Output windows. By default, these are set to Fade, Wipe, Fly, and Zoom. Clicking the arrow next to each button allows the user to select a different transition effect (e.g., Slide, CrossZoom, FlyRotate, Cube, CubeZoom, VerticalWipe, VerticalSlide, Merge, or Stinger 1/2) and set its duration in milliseconds.1 This allows for creative and engaging scene changes tailored to the production's style.  
    
- Merge Effect: This is a unique transition effect that seamlessly animates matching Inputs between the Preview and Output windows. For example, if a graphic element is small in a multi-box view in Preview and then becomes full-screen in Output, the Merge transition will animate this change smoothly. Any other layers or inputs that do not appear in both Preview and Output will transition using the standard Fade effect during a Merge.1 This effect suggests a focus on high production value and sophisticated visual storytelling.

4.2 Stinger Transitions: Professional Animated Wipes.

Stinger transitions allow the use of custom animations, often incorporating branding elements, instead of a standard cut or fade when switching between Preview and Output. This feature significantly elevates production value, giving shows a polished, broadcast-style look.1 Stinger transitions are supported on vMix editions with more than one Overlay channel, such as vMix HD and above.1

Configuration steps for Stinger Transitions are as follows 1:

1. Add Animation as Input: The animation to be used as a stinger should first be added as a standard input in vMix. The "Image Sequence" input type is recommended for stingers, especially if they require high quality and full alpha transparency (for see-through areas).  
     
2. Configure in Overlay Settings: Open the Overlay settings window (by clicking the "Overlay" button in the bottom right of the main vMix window). From the "Number" dropdown, select "Stinger 1" or "Stinger 2" to configure one of the two available stinger channels.  
     
3. Set Stinger Parameters:  
     
- Effect: This specifies an additional transition effect (usually "Cut") that occurs when transitioning to and from the stinger animation itself.  
    
- Duration: Define the total duration of the stinger animation in milliseconds or frames. This should typically match the length of the animation file.  
    
- Stinger Input: Select the input that was added in step 1 (the animation file).  
    
- Stinger Cut Point: This is a crucial setting. It specifies the precise point in time (in milliseconds or frames from the start of the animation) when vMix will cut from the outgoing source (Preview) to the incoming source (Output). If the stinger animation has an alpha channel and is designed to fully cover the screen at some point, the Stinger Cut Point is usually set to that frame.  
    
- Display underneath overlays: Tick this checkbox if the stinger transition should appear underneath any currently active overlays (channels 1-4).  
    
4. Using the Stinger: Once configured, select "Stinger 1" or "Stinger 2" as one of the four customizable transition buttons in the main vMix interface. Clicking this button will then execute the stinger transition.

4.3 Utilizing the Fade Bar (T-Bar) for Manual Control.

The Fade Bar, also known as a T-Bar, is a virtual slider located just below the FTB (Fade To Black) button in the vMix interface.1 It allows for manual control over the transition from the Preview Window to the Output Window. By clicking and dragging the T-Bar, the operator can vary the speed of the transition in real-time. The specific transition effect that the T-Bar executes (e.g., Fade, Wipe, Zoom) is determined by the effect selected for the first of the four customizable transition buttons.1 The inclusion of a T-Bar, even a virtual one, mimics a key control from hardware switchers, offering a familiar experience and allowing for nuanced, real-time control over transition speed, which some operators prefer for specific pacing or effects.

4.4 Overlays and Picture-in-Picture (PIP) Effects: Setup and Management.

The Overlay feature in vMix allows an input to be displayed on top of the currently live input in the Output Window. This is essential for displaying lower thirds, logos, on-screen alerts, or creating Picture-in-Picture (PIP) effects.1

- Activation: Overlays are typically activated by clicking one of the numbered buttons (1, 2, 3, 4\) located on each input in the Input Bar. Clicking the button again will remove the overlay, usually with the transition effect running in reverse.1 vMix HD and 4K editions support four simultaneous overlay inputs.1  
    
- Alpha Channel and Colour Keys: Overlays respect alpha channels present in the source input (e.g., a PNG image with a transparent background). Additionally, a Colour Key can be set for an input via its Input Settings, making a specific color in that input transparent when used as an overlay.1  
    
- Overlay Settings: The "Overlay Settings" window (accessed by clicking the main "Overlay" button in the bottom right corner of the vMix interface) provides detailed configuration for each of the four overlay channels 1:  
    
- Number: Selects which overlay channel (1-4) is being configured.  
    
- Type:  
    
- Fullscreen: The overlay input is displayed on top of the currently selected Output input, typically filling the screen (unless the overlay input itself has transparency or is smaller).  
    
- Picture In Picture (PIP): The overlay input is displayed on top of the Output input using specified Pan and Zoom settings, creating a smaller inset window. A blue box in the settings window provides a preview of the PIP positioning and size.  
    
- Effect: Specifies the transition effect (e.g., Fade, Slide, Zoom) to be used when the overlay is activated or deactivated. Animated transition effects will run forward when the overlay is brought on screen and in reverse when it is taken off.  
    
- Effect Duration: Sets how long the chosen transition effect should last, in milliseconds.  
    
- Duration: Specifies how long the overlay should remain on screen before automatically closing. Setting this to 0 disables automatic closing, meaning the overlay must be manually removed.  
    
- Stinger Cut Point / Stinger Input: These settings are relevant if the overlay channel is being used for Stinger Transitions (as discussed in section 4.2).  
    
- Border: For PIP overlays, a custom border can be added. Options include setting the border Colour, Thickness, and Radius (for rounded corners; 0 for square borders).  
    
- Overlay Preview: An overlay can be previewed in the Preview Window before taking it live. This is done by right-clicking the desired overlay number button (1, 2, 3, or 4\) on an input. Right-clicking again removes the overlay from preview. This "safe preview" mechanism is crucial in live production to check an overlay's appearance and positioning, reducing the chance of on-air mistakes. A useful tip is that an overlay being previewed will automatically be sent to the Output along with the main source during the next transition or cut operation.1  
    
- Picture In Picture Zoom: When an overlay is active in "Picture In Picture" mode, right-clicking its numbered button (on the input that is currently overlaid) will cause the PIP window to expand and fill the screen. Right-clicking again will reduce it back to its configured PIP size and position.1 This is a handy feature for temporarily highlighting the content of a PIP source.

The availability of four independent overlay channels, each with customizable transitions, types, and borders, provides significant flexibility for creating complex and professional-looking on-screen graphics arrangements.

4.5 Fade To Black (FTB): Uses and Configuration.

The Fade To Black (FTB) button is a standard switcher function used to cleanly fade the main production outputs to or from a black screen. This is often used at the beginning or end of a program, or for transitioning to commercial breaks.1

When FTB is activated in vMix, it affects the following outputs: Recordings, External Output, and the Fullscreen display. A key design choice is that the main Output Window within the vMix user interface is not affected by FTB.1 This is a deliberate decision to aid the operator, allowing them to fade the actual broadcast outputs to black while still being able to see and cue up the next source in the vMix interface, preventing them from working "blind."

Audio can also be included in the fade to black. If the "Fade To Black includes Audio" option is ticked in Settings \-\> Audio, the audio will fade in or out in sync with the video when FTB is activated or deactivated.1

---

Section 5: Professional Audio Mixing in vMix

A high-quality audio mix is just as crucial as good video for a professional production. vMix includes a comprehensive built-in Audio Mixer with features that can rival dedicated hardware consoles for many applications.

5.1 The vMix Audio Mixer: Interface and Core Controls.

The vMix Audio Mixer is the central hub for all audio control within the software. It can be accessed by clicking the "Audio Mixer" button, typically located on the right-hand side of the main vMix interface.1 The Audio Mixer panel displays vertical faders for each input that contains an audio source, as well as for the main audio outputs (Master, and Buses A and B if configured). Each fader is accompanied by stereo audio level meters (Left and Right channels) providing real-time visual feedback of audio levels.1 A dedicated rotary knob is provided for independent control of the Headphones volume.1 For flexibility in screen layout, especially in multi-monitor setups, the Audio Mixer panel can be detached from the main vMix window by clicking its "Pin" button.1 The design, with faders and meters, mirrors physical audio consoles, offering a familiar interface for audio engineers and a clear visual representation of levels for all users.

5.2 Managing Input Audio: Levels, Muting, Soloing, Auto-Mixing.

vMix provides essential controls for managing individual audio sources effectively 1:

- Levels: The primary way to control the volume of an audio input is by adjusting its corresponding fader in the Audio Mixer.  
    
- Audio Settings: Clicking the cog icon (⚙️) next to an input's fader in the Audio Mixer opens the "Audio Settings" window for that specific input, providing access to more advanced controls and effects (detailed further below).  
    
- Mute: A speaker icon (🔊) on each input's mixer channel acts as a Mute button. Clicking it toggles the audio for that input on or off for all audio buses it's routed to.1  
    
- Solo (S): The "S" button on each input channel enables Solo functionality. When an input is soloed, its audio is sent exclusively to the Headphones output, allowing the operator to listen to that source in isolation without affecting the main program mix (Master, Recording, Stream). This is effectively a Pre-Fader Listen (PFL) or After-Fader Listen (AFL) depending on the signal flow, crucial for checking audio quality, diagnosing issues, or cueing sources. Right-clicking the Solo button allows multiple inputs to be soloed simultaneously.1  
    
- Automatically Mix Audio ("Follow"): A button with interlocked Green and Orange Arrows on each input's mixer channel toggles the "Automatically Mix Audio" feature for that input. When enabled (often referred to as "audio follows video" or "Follow"), the audio for that input will automatically unmute when the input becomes live in the Output window and mute when another input is transitioned to. This is a significant workflow enhancement, especially for single operators, as it automates a common task and helps prevent errors like having no audio or multiple microphones live unintentionally. This behavior can also be set globally in Settings \-\> Audio and on a per-input basis in the input's General settings tab.1

5.3 Audio Buses (Master, A-G): Advanced Routing and Mix-Minus Setups.

vMix supports up to eight independent audio buses, labeled Master (M), A, B, C, D, E, and G.1 These buses allow for sophisticated audio routing scenarios, essential for tasks like creating separate mixes for different outputs, providing in-ear monitor feeds, or setting up mix-minus feeds for remote guests.

- Master Bus (M): This is the default main audio mix. Audio routed to the Master bus is typically sent to the main Recording, Stream, and External Output.1  
    
- Auxiliary Buses (A-G): These seven additional buses (A through G) can be used to create independent audio mixes. Each auxiliary bus can be routed to a specific audio output device (physical sound card output or NDI audio output) configured in Settings \-\> Audio Outputs.1  
    
- Routing Inputs to Buses: Underneath each input's fader in the Audio Mixer, there are buttons labeled "M", "A", and "B". Clicking these buttons toggles the assignment of that input's audio to the Master, Bus A, or Bus B respectively. By default, new inputs are usually routed only to the Master bus. To access routing for buses C through G, users can right-click the A or B buttons to reveal a selection menu.1  
    
- Sending Auxiliary Buses to Master: It's also possible to route the entire output of an auxiliary bus (A-G) to the Master bus. This is done by clicking the "M" button located under the fader of the auxiliary bus itself in the "OUTPUTS" section of the Audio Mixer. This allows for submixing workflows, where groups of inputs can be mixed on an auxiliary bus, and then that submix is fed into the main Master mix.1 (Note: For vMix Call, Master/Headphones audio excludes buses sent to master this way to ensure mix-minus functionality for calls works correctly 1).

The multiple audio buses are particularly crucial for creating mix-minus feeds. In a mix-minus setup (often required for remote guests via vMix Call or other systems), each remote participant receives the main program audio minus their own voice to prevent them from hearing an echo or feedback. While vMix Call has an "Auto Mix Minus" feature 1, the bus system provides the capability for manual and more complex mix-minus configurations for other scenarios, or for sending different language feeds or custom monitor mixes to various destinations. The ability to send distinct audio programs to different physical or NDI outputs also enables multi-language productions or zoned audio applications.

5.4 Audio Effects: EQ, Compression, Noise Gate.

vMix includes several fundamental audio processing tools that can be applied on a per-input basis via the "Audio Settings" window.1 These tools help improve audio clarity, control dynamics, and reduce unwanted noise, contributing to a more polished and professional final mix.

- EQ (Equalizer): A 10-band graphical equalizer is available for each audio input. This allows users to boost or cut specific frequencies to shape the tonal balance of the audio source. For example, EQ can be used to reduce low-frequency rumble from a microphone, add clarity to vocals, or remove harshness.1  
    
- Compressor: vMix provides a standard dynamic range compressor. The user can set the Ratio (e.g., 2:1, 4:1), which determines how much the audio signal is reduced once it exceeds a certain level, and the Threshold (in dB), which is the level at which the compressor begins to act. Compression is used to even out volume levels, making quiet parts louder and loud parts softer, resulting in a more consistent and controlled audio signal. This is particularly useful for dialogue.1  
    
- Noise Gate: A noise gate is a tool for reducing unwanted background noise on an audio input, such as a microphone. It works by quickly fading out (or "gating") the audio signal when its level drops below a user-defined Threshold (in dB). This can help eliminate low-level hum, computer fan noise, or room ambiance when the primary sound source (e.g., a person speaking) is silent.1

The inclusion of these per-input audio processing tools directly within vMix can significantly enhance audio quality and potentially reduce the need for external hardware processors for many common audio sweetening tasks.

5.5 Channel Mixer and Matrix: Fine-Grained Audio Control.

For inputs that contain multiple audio channels (e.g., embedded audio in an SDI or NDI feed, or multi-channel audio interfaces), vMix offers more granular control through the Channel Mixer and Channel Matrix, found in the input's "Audio Settings" window.1

- Channel Mixer: This section allows users to set the volume level of individual channels within a multi-channel input. Each channel typically has its own audio meter as well, providing visual feedback for each sub-channel's level.1  
    
- Channel Matrix: This is a powerful 16x16 audio router built into every input. It provides a grid where each column represents a source audio channel from the input (up to 16 channels), and each row represents a destination bus channel (e.g., Master Left, Master Right, Headphones Left, Headphones Right, Bus A Left, Bus A Right, etc.). By clicking the corresponding boxes in the grid, users can route any source channel to any destination bus channel.1 This is extremely useful for complex scenarios. For example:  
    
- Converting a mono microphone (e.g., connected to Channel 1 of an interface) to a stereo signal by routing Channel 1 to both Master Left and Master Right.1  
    
- Handling SDI or NDI sources that carry multiple language pairs on different embedded audio channels, allowing the operator to route the desired language pair to the Master bus, and perhaps another language pair to Bus A for a separate recording or stream.1  
    
- Isolating specific audio channels from a multi-channel source for individual processing or monitoring.

The Channel Matrix is particularly potent for inputs with multiple embedded audio channels, allowing users to extract, reroute, or mix specific channels as needed to suit the production's requirements.

5.6 Using VST3 Audio Plugins.

To further extend its native audio processing capabilities, vMix supports the use of third-party 64-bit VST3 audio plugins.1 VST3 is a popular audio plugin standard developed by Steinberg, widely used in Digital Audio Workstation (DAW) software. This allows users to integrate a vast library of specialized audio effects into their vMix workflow.

- Installation: To use a VST3 plugin, it must first be installed on the vMix computer using the installer provided by the plugin vendor. Once installed, it should appear automatically within vMix without requiring additional configuration.1  
    
- Adding and Configuring Plugins:  
    
1. Open the "Audio Settings" window for the desired input or audio bus (Master, A-G).  
     
2. Navigate to the Plugins tab.  
     
3. Click the \+ button to add a new plugin. A dialog will appear where the user can select the plugin from "Driver" and "Plugin" dropdown lists (some plugin sets may offer multiple variations).  
     
4. Once added, the plugin will appear in a list. To configure the plugin's specific settings, select it from the list and click the Show Editor button. This will open the plugin's own graphical user interface.1  
     
- Managing Plugins:  
    
- Order of Processing: Plugins are applied to the audio signal in the order they appear in the list, from top to bottom. The order can be changed using arrow buttons next to the list.  
    
- Toggling Plugins: A checkbox next to each plugin in the list allows it to be temporarily enabled or disabled without removing it.1

VST3 plugin support opens the door to a huge range of advanced audio effects beyond vMix's built-in tools, such as sophisticated reverbs, delays, de-essers, vocal processors, mastering suites, and more. This allows users with specific audio needs or preferences to integrate their favorite professional audio tools directly into the vMix environment, offering near-limitless sonic possibilities.

5.7 Configuring Audio for Recording and Streaming.

It is essential to ensure that the correct audio mix is being sent to the various outputs of vMix, such as recordings, live streams, and external hardware outputs. vMix provides flexibility in selecting which audio bus feeds these destinations.1

- Recording Audio: In the Recording Setup window (accessed via the cog icon next to the "Record" button), there is an "Audio" dropdown menu. From here, users can select which audio bus will be included in the recording (e.g., Master, BusA, BusB, etc.). It's important to note that while the AVI video format and the separate WAV File Record option support more than 2 channels of audio, if a multi-channel bus option (like MAB for 6 channels) is selected for other recording formats, typically only the first 2 channels will be included.1  
    
- Streaming Audio: Similarly, in the Streaming Quality settings window (accessed via the cog icon in the Streaming settings), the "Channels" dropdown under the "Audio" section allows users to select the audio bus (Master, BusA, etc.) that will be sent to the live stream.1  
    
- External Output Audio: For outputs to hardware devices (like AJA or Blackmagic cards), the "Audio Channels" dropdown in Settings \-\> External Output allows selection of the audio bus to be sent to that device. Many professional devices support multiple channels of embedded audio (e.g., 2, 4, 6, or 8 channels over SDI).1  
    
- WAV File Record: As mentioned in Section 6.5, vMix offers the option to record a separate, uncompressed PCM WAV file alongside the main video recording. This WAV file will contain the audio from the bus selected for the main recording (or a specifically designated bus if options evolve) and serves as a high-quality audio master.1

This ability to select different audio buses for different outputs provides powerful flexibility. For instance, a production might require a "clean feed" (program video with only natural sound, no commentary) to be recorded on Bus A, while the main Master mix (with commentary and music) is streamed live. This caters to diverse production requirements where different audiences or destinations need distinct audio programs.

---

Section 6: Recording Your Production

vMix offers robust recording capabilities, allowing users to capture their live productions in various formats suitable for different post-production workflows, archival, or direct distribution.

6.1 Recording Setup: Choosing Formats (vMix AVI, MP4, MKV, FFMPEG).

Before initiating a recording, it's crucial to configure the settings appropriately. This is done by clicking the cog icon (⚙️) next to the "Record" button in the main vMix window, which opens the "Recording Setup" window.1 vMix supports several recording formats, each with its own characteristics regarding quality, file size, editability, and fault tolerance:

- vMix AVI: This is a proprietary format developed by StudioCoast.  
    
- Pros: It offers near-lossless video quality, is optimized for fast post-production editing within environments that can read it (requiring vMix to be installed on the editing computer, though not necessarily licensed), and is inherently fault-tolerant, meaning recordings are often recoverable in the event of a power outage or system crash.1 It supports SD, HD, and 4K resolutions, as well as interlaced content.1  
    
- Cons: File sizes are very large. For editing on systems without vMix, files may need conversion (e.g., using the included vMix Media Converter to ProRes MOV).1  
    
- File Size Estimates: HD1080p30 is around 100-150 Mbps (\~55 GB per hour), while 4K60 can be 700-900 Mbps (\~350 GB per hour).1  
    
- AVI (Standard): This option allows recording to standard AVI files using various codecs.  
    
- Codecs: For SD recordings, the DV Video Encoder is often recommended. For HD, the built-in MJPEG Encoder or MagicYUV codecs are good choices. Users can also utilize compatible third-party codecs installed on their system, such as CineForm or Avid DNxHD (HQX).1  
    
- File Format (within AVI): vMix also provides an option to save these AVI recordings within an MKV container instead of a standard AVI file. The MKV format offers the advantage of supporting partial recordings, which can be recovered if a power outage or system failure interrupts the recording process.1  
    
- MP4: This format creates video files using H.264 video compression and AAC audio compression.  
    
- Pros: MP4 files offer good video quality for their file size and are widely compatible, making them suitable for direct upload to websites like YouTube or for playback on most devices.1  
    
- Cons: The H.264 compression process is computationally intensive and "requires a faster processor for optimal performance".1 While good for delivery, the higher compression may not be ideal for extensive high-quality post-production editing compared to less compressed formats. Under Windows 7, MP4 recordings have a maximum file size limit of 4GB; for larger recordings, a different format or upgrading to a newer Windows version is necessary.1  
    
- Fault Tolerance: Standard MP4 recordings are generally not fault-tolerant. However, vMix offers an option (a checkbox) to create fault-tolerant MP4 recordings, but the documentation advises that these should be thoroughly tested for compatibility with target devices and software before use in critical productions.1  
    
- FFMPEG: vMix leverages the open-source FFMPEG encoding tool to provide recording capabilities in a variety of additional formats, including MPG (MPEG-2 Program Stream), TS (MPEG-2 Transport Stream), MOV, and MXF.1  
    
- Codecs via FFMPEG: Options include MPEG-2, MP4 (using x264 for H.264 video and AAC audio), and VC-3 (similar to Avid DNxHD).  
    
- Fault Tolerance: When using FFMPEG, choosing container formats like MXF or non-indexed MOV/MP4 is recommended as they generally support file recovery in the event of power or system failure.1  
    
- MPEG-2 (often via FFMPEG or dedicated option):  
    
- File Formats: Can be saved as Program Stream (MPG) or Transport Stream (TS). TS is often recommended if the video will be edited in programs like Sony Vegas.1  
    
- Fault Tolerance: Both MPG and TS formats created by vMix are generally fault-tolerant.1

The choice of recording format involves a trade-off between video quality, suitability for editing, file size, system compatibility, and CPU load. For archival purposes or high-end post-production, a high-quality, less compressed, and fault-tolerant format like vMix AVI or FFMPEG to MOV/MXF might be preferred. For direct web upload or wider compatibility, MP4 is often the go-to choice. Users with less powerful CPUs might need to opt for less computationally demanding codecs.1

Table 6.1: vMix Recording Format Comparison.

|  |  |  |  |  |  |
| :---- | :---- | :---- | :---- | :---- | :---- |
| Feature | vMix AVI | AVI/MKV (MJPEG) | MP4 (H.264) | FFMPEG (MPEG-2 PS/TS) | FFMPEG (MOV/MXF \- VC-3/X264) |
| Key Codecs | vMix Codec | MJPEG, DV, MagicYUV, 3rd party | H.264 (AAC audio) | MPEG-2 | VC-3, H.264 (AAC audio) |
| Typical Use Case | High-quality archive, editing (PC) | HD/SD editing, general purpose | Web upload, general playback | Broadcast, editing (TS) | Professional editing, archive |
| Pros | Near lossless, fast edit, fault-tol | Good quality, codec choice | Good quality/size, compatibility | Fault-tolerant, TS good for edit | High quality, fault-tolerant (MXF/MOV non-indexed) |
| Cons | Very large files, vMix for edit | AVI not fault-tol (MKV is) | Higher CPU, Win7 4GB limit, not ideal for heavy edit | Larger than MP4 | Can be large files |
| Relative File Size | Very High | High | Medium | Medium-High | High |
| CPU Load | Low | Low-Medium | Medium-High | Medium | Medium-High |
| Fault Tolerant | Yes | AVI: No, MKV: Yes | No (Yes with checkbox, test) | Yes | MXF/MOV (non-indexed): Yes |

This table provides a quick reference to help users choose the recording format that best aligns with their specific production needs, considering various factors.

6.2 Optimizing Recording Quality and Settings.

Within the "Recording Setup" window, several settings can be fine-tuned for each chosen format to ensure the recording meets the desired quality and technical specifications 1:

- Filename: Specify the name and location for the recorded file.  
    
- Frame Rate: This should generally be set to match the Master Frame Rate configured under Settings \-\> Display to ensure smooth recordings without frame duplication or dropping.  
    
- Codec: (For AVI/FFMPEG) Select the appropriate video codec.  
    
- File Format: (For AVI/FFMPEG) Choose the container (e.g., AVI, MKV, MP4, MOV, TS, MXF).  
    
- Audio: Enable audio recording and select the audio channels/bus to be included (e.g., Master mix, Bus A). An Audio Delay can also be set in milliseconds if there's a sync issue between the incoming audio and video.  
    
- New File Every: This highly practical feature allows users to automatically start a new recording file every 'x' minutes (e.g., every 30 minutes). The split is seamless, meaning no frames are lost between segments, which is excellent for very long recordings. It makes file management easier and also contributes to fault tolerance, as if one segment is corrupted, others are likely to be intact.1  
    
- Bit Rate (for MP4, MPEG-2, etc.): For formats like MP4 and MPEG-2, the video bit rate (in Mbps) and audio bit rate (in Kbps) can be specified to control the quality and file size. For MP4, 25 Mbps is recommended for high-quality HD, and 128-192 Kbps for AAC audio.1  
    
- Global Recording Settings: In Settings \-\> Recording, users can set a default folder for all recordings, customize the default filename format, and adjust the recording memory buffer (recommended value is 10), which can help reduce dropped frames on systems with slower hard drives.1

6.3 The Importance of Fault-Tolerant Recordings.

Live production environments can be unpredictable, with potential for software crashes, hardware failures, or power outages. For many recording formats, crucial file information (like the file header or index tables) is held in memory and only written to disk when the recording is properly stopped. If an interruption occurs before this, the entire recording can become corrupt and unrecoverable.1

vMix addresses this critical issue by offering several fault-tolerant recording formats. These formats are designed to write data to disk in a way that allows for recovery even if the recording process is abruptly terminated. The documentation explicitly highlights this, with a table indicating the fault tolerance of each format 1:

- Fault-Tolerant: vMix AVI, AVI in MKV container, MPEG-2 (MPG and TS), WMV, FFMPEG to MXF, FFMPEG to MOV (non-indexed), FFMPEG to MP4 (non-indexed).  
    
- Not Fault-Tolerant (or conditional): Standard AVI, standard MP4 (unless the "Fault Tolerant" checkbox is ticked, in which case thorough compatibility testing is advised), FFMPEG to indexed MOV/MP4.

The vMix AVI format is specifically noted as the "best fault tolerant format" among the options.1 Utilizing a fault-tolerant format, especially in conjunction with the "New File Every" feature, provides a significant safety net, minimizing the risk of catastrophic data loss during live events. This emphasis on reliability underscores an understanding of the critical nature of capturing live event footage.

6.4 Second Recorder and MultiCorder Capabilities.

For more advanced recording workflows, vMix offers additional capabilities in its higher-tier editions 1:

- Second Recorder (vMix 4K and higher): This feature allows a second, independent recording to be made simultaneously with the primary recording. It is configured by selecting the "2" button at the top of the "Recording Setup" window and enabling it. The second recorder has its own independent settings for format, codec, and even the video and audio sources it uses. This is very flexible; for example, a high-quality master could be recorded using vMix AVI, while a lower-quality, smaller MP4 proxy file is created concurrently by the second recorder for quick sharing or internet publishing. The second recording starts and stops in sync with the primary recording.1  
    
- MultiCorder (vMix 4K and Pro editions): MultiCorder is a powerful feature for productions that require isolated recordings (ISOs) of multiple camera feeds. It allows users to record the raw video and audio from selected capture inputs (Cameras, NDI sources, and even the main vMix Output channels) to separate files, in addition to the main vMix program recording.1 This provides maximum flexibility in post-production for re-editing the event from different angles, fixing switching errors, or creating alternative content.  
    
- System Requirements: MultiCorder is demanding, requiring at least a Solid State Disk (SSD) for storing recordings, an Intel Core i7 Quad Core processor or higher, and a high-end graphics card.1  
    
- Configuration: Users select the sources to record from a list in the MultiCorder window. Supported recording formats include vMix AVI, AVI, MKV, MP4, and FFMPEG. Audio can be sourced from the input's embedded audio or the Master mix. SRT inputs are always recorded in their native.ts format. A particularly useful optimization is the option to record NDI sources in their original MOV format, which bypasses re-compression and thus uses minimal additional system load.1  
    
- Limitation: A critical operational constraint is that Instant Replay and MultiCorder cannot be used at the same time.1 Both features are highly disk and CPU intensive due to continuous recording of multiple streams, implying a shared underlying recording engine or resource limitation. Users must choose which of these advanced features is more critical for a given production.

6.5 WAV File Recording for Separate Audio Masters.

In addition to the audio embedded within the video recording, vMix provides an option to record a separate, uncompressed PCM WAV audio file simultaneously. This is toggled via the "WAV File Record" button in the "Recording Setup" window.1 This feature does not affect the audio that is part of the video recording itself; it creates an additional, high-quality audio master. The audio format of this WAV file is fixed within vMix but can be converted to other formats like MP3 using third-party applications if needed.1 This option caters to professional audio post-production workflows where a pristine, uncompressed audio source is preferred for mixing, mastering, or archival, separate from the video file.

---

Section 7: Live Streaming with vMix

vMix integrates comprehensive live streaming capabilities, allowing users to broadcast their productions directly to various online platforms and services.

7.1 Getting Started with Streaming: Provider Setup (RTMP).

The initial step to begin streaming is to configure the connection to the chosen streaming provider. This is done through the streaming settings window, accessed by clicking the cog icon (⚙️) next to the "Stream" button in the main vMix interface.1

vMix offers a streamlined setup for many major streaming platforms. Users can often select their provider (e.g., YouTube Live, Facebook Live, Twitch) from a dropdown list and then log in with their account credentials directly within vMix to retrieve a list of available channels or events to stream to.1

For providers not listed, or for streaming to private servers, the "Custom RTMP Server" option provides the necessary flexibility. In this case, the user needs to obtain the RTMP URL (e.g., rtmp://example.com/live) and the Stream Name or Key from their provider and enter these details into the respective fields in vMix.1 This dual approach caters both to ease-of-use for popular services and adaptability for a wide range of other RTMP-based streaming destinations.

7.2 Configuring Streaming Quality: Bitrates, Resolution, Encoders (FFMPEG, FMLE, Hardware Encoding).

The quality of the live stream is determined by several settings that balance visual fidelity against available upload bandwidth and the processing power of the vMix computer. These settings are found in the "Streaming Quality" window, accessed via a cog icon within the main streaming settings panel.1

Key quality parameters include 1:

- Video Bit Rate: Measured in kilobits per second (kbps) or megabits per second (Mbps), this determines the amount of data used for the video stream. Higher bitrates generally result in better quality but require more upload bandwidth.  
    
- Encode Size (Resolution): The resolution of the streamed video (e.g., 1920x1080 for 1080p, 1280x720 for 720p, 640x360 for 360p). This should match the aspect ratio being used in the vMix production.  
    
- Audio Bit Rate: The data rate for the audio stream, typically in kbps. 128 kbps AAC is a common setting for good quality stereo audio.  
    
- Encoder Application: vMix offers choices for the underlying encoding engine:  
    
- FFMPEG: This free, open-source encoder is installed with vMix and is generally the recommended option. It supports H.264 video and AAC audio and is noted for providing "better quality and AAC audio support" compared to FMLE.1 It is also required for streaming to multiple destinations simultaneously.  
    
- Adobe Flash Media Live Encoder (FMLE): This is an older, optional encoder from Adobe that can be downloaded and installed separately. It supports H.264 video and MP3 audio natively (AAC audio requires an additional paid plugin from MainConcept). FMLE might be used if a streaming provider specifically requires it or if MP3 audio encoding is essential.1  
    
- Use Hardware Encoder: Many modern NVIDIA graphics cards feature dedicated hardware encoders. vMix can leverage these to offload the CPU-intensive task of video encoding, significantly reducing system load. This option is available as a checkbox. However, it's important to be aware that NVIDIA GeForce series cards typically have a limit of two simultaneous hardware encoding sessions per system. This means if a user is already recording to MP4 using hardware encoding, only one stream can concurrently use hardware encoding. NVIDIA Quadro series cards generally do not have this restriction.1  
    
- Advanced Encoding Parameters (primarily for FFMPEG):  
    
- Video Source: In vMix 4K and Pro, users can select which output (Output 1 or Output 2\) feeds the stream.  
    
- H.264 Profile: Options like "Baseline" (lower quality, less CPU) or "Main" (higher quality, more CPU) affect the complexity and efficiency of the H.264 encoding.  
    
- Preset (FFMPEG x264): Controls the trade-off between encoding speed and compression efficiency. veryfast is the recommended default, offering a good balance of CPU usage and quality.1  
    
- Keyframe Frequency: The interval (in seconds) between full picture frames (keyframes) in the video stream. Two seconds is a common recommendation from streaming providers.1  
    
- Network Buffer: The maximum amount of data (in seconds) vMix can buffer before sending to the streaming server. Increasing this can help smooth out streams over unreliable internet connections but also increases latency.  
    
- Strict CBR (Constant Bit Rate): Attempts to keep the streaming bitrate as close as possible to the target, which may sometimes reduce quality if the content is highly complex.

These numerous settings give users fine-grained control to optimize their stream for their specific conditions. Hardware encoding is a particularly valuable feature for maintaining system stability during demanding productions.

7.3 Streaming to Multiple Destinations Simultaneously.

vMix allows users to stream to up to three different destinations concurrently from a single instance, a powerful feature for maximizing audience reach (e.g., streaming to YouTube, Facebook, and Twitch at the same time).1 This capability is available when FFMPEG is selected as the streaming application.1 The 1, 2, and 3 buttons at the top of the Streaming Settings window are used to configure each destination.

By default, all three destinations will use the same quality settings as defined for Stream 1\. However, users can configure independent quality settings (bitrate, resolution, etc.) for each destination by unticking the "Use Stream 1 Quality" checkbox for Streams 2 and 3.1 It's important to note that when using multiple destinations, the Multi Bitrate Streaming feature (discussed next) is disabled.1 This multi-platform distribution from a single source simplifies the workflow for simulcasting significantly.

7.4 Multi-Bitrate Streaming for Adaptive Delivery.

Multi-Bitrate Streaming involves sending several versions of the stream at different bitrates (and potentially resolutions) to the streaming provider. The provider's Content Delivery Network (CDN) and the viewer's video player can then work together to deliver the optimal quality stream based on the viewer's available internet bandwidth. This is the foundation of Adaptive Bitrate Streaming (ABR), which significantly enhances the viewer experience by reducing buffering and dynamically adjusting quality.

vMix supports setting up multi-bitrate streams for both FMLE and FFMPEG applications.1 There are two main methods, depending on the streaming provider's requirements:

1. Single Stream Key Method: Some providers use a single stream key but can ingest multiple bitrate renditions sent to the same ingest point.  
     
- Configure the primary stream (highest quality) under Stream 1\.  
    
- For the additional lower-bitrate streams (up to two more), select "Stream 1 Multi-Bitrate" as the "Destination" for Stream 2 and Stream 3\.  
    
- Untick the "Use Stream 1 Quality" checkbox for these additional streams and configure their independent (lower) bitrates and resolutions in their respective Quality settings.1  
    
2. Multiple Stream Keys Method: Some providers issue separate stream keys (and potentially different ingest URLs) for each bitrate rendition.  
- In this case, select "Custom Multi-Bitrate" as the "Destination" for each stream (Stream 1, Stream 2, Stream 3\) and enter the unique URL and Stream Key provided for each specific bitrate.1

When sending multiple bitrates, the "Keyframe Aligned" option in the Streaming Quality settings can be enabled. This ensures that keyframes across all bitrate streams are synchronized, which can improve the seamlessness of switching between quality levels at the player end, albeit potentially at a slight cost to overall compression efficiency.1 While vMix itself doesn't perform the ABR switching (that's handled by the CDN and player), its ability to output the necessary multiple bitrate streams is crucial for enabling this professional delivery method.

7.5 Advanced Streaming Options and Troubleshooting.

The "Advanced" button within each stream's configuration provides additional options that may be required by specific streaming providers, such as fields for a separate Username and Password (distinct from the main login for providers that support direct channel selection). For FMLE, options for a Backup Stream URL (if the primary fails) and Save to file (to save a local copy of the stream) are also available here.1

vMix offers independent control over the configured streams. Users can start or stop all streams simultaneously using the main "Stream" button or the "Start All / Stop All" buttons in the streaming settings window. Alternatively, individual streams can be started or stopped by clicking the arrow next to the main "Stream" button and selecting the specific stream, or by selecting the stream's tab (1, 2, or 3\) in the settings window and using the "Start x / Stop x" button at the bottom.1

This independent control provides resilience in multi-stream environments. If one stream encounters an error (e.g., due to an issue with one platform), it will stop, but the other configured streams will continue to run as normal. The problematic stream can then be manually restarted once the issue is resolved.1 To aid in diagnosing connection issues, the "View Status" button (available when a stream is running or attempting to connect) provides technical information about the stream's connection and performance.1

---

Section 8: Advanced vMix Features and Workflows

Beyond core switching, recording, and streaming, vMix offers a suite of advanced features that cater to more complex and professional production scenarios.

8.1 Virtual Sets: Creating Immersive Environments with Chroma Keying.

Virtual Sets in vMix allow producers to place live talent (shot against a green or blue screen) into sophisticated 3D rendered environments, complete with realistic camera movements, all without the need for large physical sets.1 This feature can dramatically enhance production value, especially for creators with limited space or budget.

- Setup: To use a virtual set, one of the built-in presets is added as an input. These presets often show placeholder images indicating where talent and other graphic elements will be positioned.1 The effectiveness of a virtual set relies heavily on good Chroma Keying. The Colour Key settings within the talent's camera input are used to make the green or blue background transparent, allowing the virtual environment to show through.1  
    
- Control: Each Virtual Set input has two main control tabs:  
    
- Camera Tab: This tab displays thumbnail previews of various pre-defined camera angles within the 3D virtual set. Clicking a thumbnail smoothly transitions the virtual camera to that angle. The speed of these camera movements (zooms and pans) can be controlled using F (Fast), M (Medium), S (Slow), and C (Cut) buttons associated with the angles.1 This dynamic camera movement adds a layer of realism and engagement that static virtual backgrounds lack.  
    
- Setup Tab: This tab allows for customization of the various layers that make up the virtual set. Users can select different layers (e.g., "Talent," "Screen," "Background") and assign different vMix inputs to them. For instance, the "Talent" layer would be assigned the chroma-keyed camera input, while a "Screen" layer (representing a monitor within the virtual set) could be assigned a video playback input or a PowerPoint presentation. The position and scale of these layers within the 3D scene can often be adjusted by clicking and dragging in the preview window (holding Shift to resize), and layers can be toggled visible or invisible (e.g., to hide a virtual desk).1 This layer-based customization provides creative flexibility to integrate various media elements directly into the virtual environment.

8.2 Instant Replay System: Setup and Operation for Multiple Cameras.

vMix includes a powerful Instant Replay system, primarily in its 4K and Pro editions, designed for sports and live event production. It allows for continuous recording of up to eight camera inputs and provides two independent playback channels with features like slow motion, reverse playback, and frame-by-frame control.1

- Core Features:  
    
- Records up to eight camera inputs (including 4 channels of audio per camera) as high-quality vMix AVI 4:2:2 files, supporting resolutions up to 4K and both progressive and interlaced formats.  
    
- Two output playback channels (Replay A and Replay B) that can be controlled independently or in sync, with any recorded camera angle assignable to each.  
    
- Precise slow-motion playback control from 0% to 100%.  
    
- Twenty event lists are available, each capable of holding an unlimited number of Mark In and Mark Out points that can be created on the fly and edited. Each event can have a default camera angle and text comments for easy recall.  
    
- Ability to playback entire event lists or selected entries as a highlight reel, complete with transition effects and background music.  
    
- Quick event creation using auto mark-in/out buttons (e.g., for the last 5, 10, or 20 seconds).  
    
- Extensive keyboard shortcut support and compatibility with hardware controllers (X-Keys, JLCooper, Contour ShuttlePro).  
    
- Events can be exported as separate video files, or the raw recordings can be used directly in video editing software (vMix AVI can be imported into Premiere Pro and Vegas Pro, or converted to MP4/ProRes).1  
    
- System Requirements: Instant Replay is a very demanding feature, requiring a powerful CPU, a high-end NVIDIA GeForce GTX graphics card (specific models recommended based on channel count), and, crucially, dedicated SSD storage (NVMe SSDs for higher channel counts) due to the high data rates involved in continuously recording multiple video streams.1  
    
- Workflow Changes (since vMix 23): The user guide notes significant workflow changes in vMix 24, including the shift to the vMix AVI recording format (from MPEG-2), fully independent A and B output channels, changes to how event transitions overlap, updates to ShuttlePro v2 controller mapping, and the introduction of per-event playback speeds.1 Users familiar with older versions need to be aware of these adjustments. The move to vMix AVI for replay enhances recording quality (4:2:2 color sampling) and editability but may require exporting to MP4 for direct web uploads.1  
    
- Setup:  
    
1. Add all cameras to be used for replay as standard inputs in vMix.  
     
2. Click "Add Input" and select the "Instant Replay" tab.  
     
3. Configure the Session Folder (must be on a dedicated SSD), the Recording Format (must match camera sources), and select which camera inputs to include (the main vMix "Output" can also be selected as a source).  
     
4. Choose the Playback Audio Source (e.g., "Master" for program audio, or "Follow" to use the active camera angle's embedded audio).  
     
5. Set In, Out, and Event Transitions to be used during replay playback.1  
     
- Operation:  
    
- Once set up, "Replay A" and "Replay B" inputs appear in vMix for playback.  
    
- The Instant Replay Controller (dockable tab or separate window) is used to manage events.  
    
- Events can be created in Live Mode (based on current time) or Recorded Mode (by scrubbing through previously recorded footage to mark events that were missed live).1  
    
- Events are defined by Mark In and Mark Out points, and can have multiple camera angles tagged and commented on. Playback speed can be set per event or controlled live.1

The comprehensive feature set and demanding hardware requirements indicate that Instant Replay is a professional-grade tool, a key differentiator for the higher editions of vMix.

8.3 PTZ Camera Control: Direct Integration and Control Methods.

vMix (4K and Pro editions) offers direct control over Pan-Tilt-Zoom (PTZ) cameras, streamlining operations by integrating camera movement controls into the production software.1 This support can be enabled on any input type (SDI, HDMI, NDI, or RTSP stream) that is receiving video from a PTZ camera.

- Enabling PTZ Control:  
    
1. In the Input Settings of the camera input, go to the PTZ tab.  
     
2. Select the Device Type that matches the PTZ camera. vMix supports a range of network-controlled PTZ cameras (an up-to-date list is on their website). It's important to note that vMix primarily supports cameras using network control (Ethernet); cameras that only offer serial control (e.g., VISCA or Pelco via RS-422/RS-232) are not currently supported, simplifying integration by avoiding complex serial interfacing.1  
     
3. Enter the IP Address or Web Address of the PTZ camera (as configured in the camera's own network settings).  
     
4. Click Connect. If successful, the PTZ controls will become active.1  
     
- Control Methods:  
    
1. PTZ Control using Virtual Inputs: This is a particularly powerful method. The operator can move the physical PTZ camera to a desired position (pan, tilt, zoom) and then click "Create Input at this Position" in the PTZ settings. This creates a new "virtual" input in vMix that, when selected into Preview, will automatically command the physical PTZ camera to move to that saved preset position. Multiple virtual inputs can be created from a single PTZ camera, effectively allowing one camera to act as several distinct camera angles. This can allow a single operator to manage a multi-angle production from one or two PTZ cameras with simple input switching in vMix.1  
     
2. PTZ Control using the Mouse: The PTZ tab in Input Settings provides on-screen buttons for manual control: up, down, left, right, zoom in, zoom out, focus controls, and speed adjustments.1  
     
3. PTZ Control using Shortcuts and Joysticks: Most PTZ functions (e.g., PTZMoveUp, PTZZoomIn, PTZFocusFar, preset recall) can be assigned to keyboard keys, MIDI controller buttons/faders, or even the joysticks on an XBOX-compatible controller. vMix includes a shortcut template for XBOX controllers. Custom speeds can be specified for shortcut-driven movements, and pressure sensitivity can be enabled for variable speed control with joysticks.1

The direct integration of PTZ control, especially the virtual input concept, significantly enhances workflow efficiency for smaller productions or single-operator scenarios.

8.4 vMix Call: Integrating Remote Guests Seamlessly.

vMix Call is an integrated solution for bringing remote guests into a live production with high-quality audio and up to HD video, requiring only a web browser and webcam on the guest's end.1

- Guest Experience: Guests connect by visiting [www.vmixcall.com](http://www.vmixcall.com) in a supported browser (Google Chrome, Firefox on Windows/Mac/Android; Safari on iOS 11+) and entering a name and a password provided by the vMix operator. No software installation is needed for the guest, which significantly lowers the barrier to participation and reduces technical support overhead.1  
    
- Host (vMix Operator) Setup:  
    
1. In vMix, click "Add Input" and select the "Video Call" tab.  
     
2. Choose "Host a Call." An automatic password will be generated to share with the guest.  
     
3. Configure the Return Feed sent to the guest:  
     
- Video Source: Select which vMix output (Output 1, 2, 3, or 4 in 4K/Pro editions) or "None" to send as video to the guest.  
    
- Video Bandwidth: Choose the quality/bandwidth of this return video. This setting is global for all guests.  
    
- Audio Source: Select the audio mix (Master, Headphones, or an Aux Bus A-G) to send to the guest. vMix Call features Auto Mix Minus, ensuring guests do not hear an echo of their own audio regardless of the source selected.1  
    
4. Click OK to add the vMix Call input.  
     
- Features:  
    
- Peer-to-peer encryption for secure connections.  
    
- Full-duplex high-quality audio.  
    
- Dynamic bandwidth estimation automatically adapts the quality of each guest's video to changing network conditions.  
    
- Video and audio from each guest are also available as individual NDI sources within vMix.1  
    
- Call Manager: A dedicated Call Manager window (right-click any vMix Call input to open) allows the operator to monitor the status of all calls (connection quality indicated by color codes: Green, Amber, Red), view statistics (resolution, bandwidth, frame rate, jitter), and engage in text chat with all connected guests.1  
    
- Troubleshooting: Common issues include guests not having selected their webcam/microphone in the browser, internet connection interruptions (guest refreshes browser to reconnect), network congestion affecting quality (operator can try lowering return video bandwidth), and audio echo (guest should use headphones).1 The quality of vMix Call is fundamentally dependent on the internet connections of both the host and the guest, despite adaptive technologies.1

8.5 NDI Deep Dive: Sending and Receiving Video/Audio Over Network.

Network Device Interface (NDI) allows for high-quality, low-latency transport of video and audio over a standard Gigabit Ethernet network. vMix has comprehensive NDI support, acting as both an NDI receiver and sender, effectively turning it into a powerful NDI matrix or router for complex IP-based workflows.1

- Receiving NDI Sources:  
    
- To add an NDI source, select "Add Input" \-\> "NDI / Desktop Capture." vMix automatically discovers NDI sources available on the local network.  
    
- The vMix Desktop Capture application (free for PC/Mac) allows any computer's desktop or application window to become an NDI source.  
    
- Options for received NDI streams include Low Bandwidth Mode, Audio Only, PsF handling, and an increased buffer for unstable networks.1  
    
- Sending NDI from vMix:  
    
- NDI outputs are enabled in Settings \-\> Outputs / NDI.  
    
- vMix can send various feeds as NDI:  
    
- Output 1, 2, 3, 4: The main program output or other configured independent outputs (Preview, MultiView, specific input).  
    
- Cameras / Calls / Audio Inputs: Individual camera inputs, vMix Call guest feeds, and dedicated audio inputs can each be made available as separate NDI streams on the network.  
    
- Audio Outputs: The Master audio mix, Headphones mix, and auxiliary audio buses (A-G) can be sent as audio-only NDI streams.1  
    
- Alpha Channel over NDI: For NDI outputs (Output 1-4), vMix can send video with an alpha channel. This is configured by clicking the cog icon next to the desired output in the Outputs / NDI settings and selecting "Straight" or "Premultiplied" for the Alpha Channel setting. This is crucial for professional graphics workflows, allowing vMix to send keyed graphics (like lower thirds with transparency) to other NDI-compatible systems.1 vMix also automatically supports alpha channel when detected on an incoming NDI source (with a "premultiplied alpha" checkbox in Colour Adjust settings if needed).1

8.6 Data Sources: Linking Titles to Dynamic Content (Google Sheets, Excel, XML, Text, RSS, JSON).

Data Sources in vMix allow title inputs to be linked to external data, enabling dynamic text and even image updates automatically as the source data changes.1 This is invaluable for live events with frequently changing information like scores, speaker names, or social media comments, significantly improving workflow efficiency.

- Supported Data Source Types: Excel/CSV files, Google Sheets (requires a Google API Key and the sheet to be publicly viewable), XML files or URLs, JSON data (object arrays), RSS feeds, and plain Text files.1 This broad support allows integration with many existing data workflows and online services.  
    
- Setup:  
    
1. Open the Data Sources Manager (from the hamburger menu in the bottom right of vMix).  
     
2. Click the \+ button to add a new data source.  
     
3. Name the source, provide the file path or URL, and configure options like "Use first row as column names" or "Convert rows to columns" (which flattens multiple rows into a single row with numbered columns).1  
     
- Mapping Data to Titles:  
    
1. Open the Title Editor for a title input (right-click the input).  
     
2. Select a text field (e.g., "Headline") or image placeholder in the title.  
     
3. Click the Data Source button in the Title Editor's toolbar.  
     
4. Choose the Data Source, Table (if applicable, like a sheet in Excel), and Column. "Auto" mapping attempts to match column names to field names or uses index order.  
     
5. A Format string can be used to add static text around the dynamic data (e.g., Score: {0}).1  
     
- Controlling Data Sources:  
    
- Data Sources Manager: Manually select the current row to display from a table. "Auto Next" can cycle through rows at a timed interval, with a "Loop" option.  
    
- Shortcuts: Functions like DataSourceNextRow, DataSourcePreviousRow, DataSourceSelectRow allow for programmatic control.  
    
- Editing Source File: Since data sources update automatically, modifying the source file (e.g., an Excel spreadsheet or Google Sheet) and saving it will reflect the changes in vMix titles.1  
    
- Images in Data Sources: If a title template has an image field, the data source can provide a full URL or local file path to dynamically update that image.1

8.7 PlayList for Automated Switching.

The PlayList feature in vMix provides a way to automate a sequence of switching tasks or to play multiple video or audio files sequentially.1 This is useful for pre-programmed segments of a show, unattended operation (like a lobby display), or playing a series of video clips during a break.

- Configuration:  
    
- Access the PlayList window via the cog icon next to the "PlayList" button in the main vMix interface.  
    
- Add inputs from the "Available Inputs" column to the "Playlist" column.  
    
- For each item in the playlist, double-click to set:  
    
- Starting Position: (For video clips) Where the clip should start playing from.  
    
- Duration: How long this item will play before moving to the next. If 0, it defaults to the input's own duration.  
    
- Transition: The transition effect to use when this item becomes active.  
    
- Transition Duration: The length of that transition.  
    
- Display Type: Can be set to "Overlay," causing this playlist item to appear as an overlay over the previous item for its duration.1  
    
- Global playlist settings include Loop (restart from beginning when finished), Begin from selected item, Clear Overlays (before starting), and Manual Mode (playlist waits for "Next" button click to advance).1  
    
- Operation: Once configured, the main "PlayList" button starts or stops the playlist. "Previous" and "Next" buttons in the PlayList window allow manual navigation.  
    
- Playlists are saved as part of the vMix Preset they were created in and are loaded with that preset.1 This simple automation is ideal for repetitive sequences, reducing operator workload.

8.8 Tally Lights Integration.

Tally lights provide visual confirmation to camera operators and on-screen talent which source is currently live (Program) or cued (Preview). vMix supports several tally light solutions, catering to different budgets and technical capabilities 1:

- Smart Phone Tally Lights: An innovative and highly accessible option. The vMix Web Controller has a "Tally Lights" page that can turn any Wi-Fi connected smartphone's screen into a tally light, displaying different colors based on the input's status.1  
    
- Commercial USB Tally Lights: vMix supports dedicated USB tally light systems from vendors like Tally-Lights.com and metaSETZ. These often work automatically, with tally numbers corresponding to input numbers in vMix (e.g., Tally 1 for Input 1).1 Radio-Far tally lights are also mentioned.1  
    
- Arduino Tally Lights: For DIY enthusiasts, vMix supports custom-built tally lights using the open-source Arduino hardware platform. This requires loading the "StandardFirmata" firmware onto the Arduino device. In vMix, the Arduino is connected via a COM port, and individual digital pins on the Arduino are assigned to tally numbers (and thus to vMix inputs) via the Settings \-\> Tally Lights tab.1 This offers a very cost-effective and customizable solution.

---

Section 9: Customization, Automation, and Control

vMix offers extensive customization and automation capabilities, allowing users to tailor the software to their specific workflows and control preferences. This is primarily achieved through Shortcuts, Activators, Triggers, and Scripting.

9.1 Shortcuts: Keyboard, MIDI, and Controller Mapping.

Shortcuts in vMix are akin to macros, enabling complex actions or sequences of functions to be triggered by a single keyboard key press, MIDI controller event (button, fader, knob), or input from supported devices like X-Keys controllers, Contour Design ShuttlePROv2, or Elgato Stream Deck devices.1 An unlimited number of shortcuts can be configured.

- Adding a Shortcut:  
    
1. Navigate to Settings \-\> Shortcuts tab and click Add.  
     
2. The Find... button allows quick assignment by pressing the desired key or moving the physical control. For MIDI controllers, ensure the device is connected and enabled in MIDI Settings within the Shortcuts tab before vMix starts.1  
     
3. Select a Function from an extensive categorized list (the full Shortcut Function Reference is provided in the user guide, pages 210-230).  
     
4. If the function is a transition, set its Duration in milliseconds.  
     
5. Assign an Input if the function targets a specific source. The shortcut can be tied to the input's current number or its unique identity (so it follows the input if moved).  
     
6. Optional Title and Description fields are for display in the Web Controller.  
     
7. Display options configure the button's appearance in the Web Controller (Default text, Colour, custom Image, or Input Thumbnail).  
     
8. Local Shortcut (This Preset Only) checkbox saves the shortcut with the current preset; otherwise, it's global. Local shortcuts override global ones for the same key.  
     
9. Show in Web Controller checkbox controls visibility on the remote interface.1  
     
- Multiple Functions per Button: Multiple shortcut entries can be assigned to the same key/control. They will execute in the order listed in the Shortcuts window.1  
    
- Advanced MIDI Shortcuts: For MIDI controls, the Channel and Note/CC number are usually auto-detected. The Value (0-127) can be specified to trigger different functions based on a control's position (e.g., a rotary knob). The Type can be set to "Default" for linear controls or various "JogWheel" settings for continuous rotary encoders, enabling functions like frame-by-frame jogging or speed control for replays.1  
    
- Dynamic Inputs and Values: This advanced feature allows a small number of physical buttons to control many different targets.  
    
- Dynamic Inputs: A shortcut function (e.g., Fade) can be set to target Dynamic1, Dynamic2, Dynamic3, or Dynamic4. Another shortcut using functions like SetDynamicInput1 can then assign a specific vMix input (by name or number) to that dynamic target. Pressing the "SetDynamicInput" button first chooses the target, then pressing the "Fade" button acts on that chosen target.1  
    
- Dynamic Values: Similarly, a shortcut function requiring a text value (e.g., SetText for a title) can have its value set to Dynamic1, etc. Another shortcut using SetDynamicValue1 can then assign the actual text string to that dynamic value.1 This enables context-sensitive controls, reducing the need for large control surfaces by creating logical "banks" or modes of operation.  
    
- Shortcut Templates: vMix allows importing and exporting sets of shortcuts. Built-in templates are provided for devices like the Novation LaunchControlXL and Contour ShuttlePROv2 (for Replay).1

The depth of the shortcut system, with its vast function library and support for diverse controllers, allows users to create highly personalized and efficient control surfaces, significantly speeding up operations during live productions.

9.2 Activators: Device Feedback (LEDs, Faders) for Enhanced Control.

Activators create a two-way communication link with MIDI and X-Keys controllers. While Shortcuts send commands from the controller to vMix, Activators allow vMix to send status updates back to the controller, triggering responses like lighting up button LEDs or moving motorized faders.1 This provides crucial visual and tactile feedback, enabling confident operation without constantly needing to look at the vMix interface.

- Setup:  
    
1. Go to Settings \-\> Activators tab.  
     
2. Click Enable Devices to select and enable the MIDI/X-Keys controller(s) to be used for feedback.  
     
3. Click Add to create a new Activator.1  
     
- Configuration:  
    
- Control: Specify the MIDI Note or ControlChange (or X-Keys equivalent) of the button light or fader to be controlled. The Find... button helps auto-detect these settings.  
    
- Event: Select the vMix event that will trigger the feedback. Examples include Input (input is live in Output), InputPreview (input is in Preview), InputPlaying (input is a playing video), InputVolume (volume of an input changes, for motorized faders), FadeToBlack (FTB is active), Recording (recording is active), etc..1  
    
- Input: If the event relates to a specific input, select it here. The activator can be assigned to a specific input number.  
    
- Type: Defines the behavior of the feedback on the controller. For buttons with multiple LED colors (like on an AKAI APC40), this is where the color is selected (e.g., red for live, green for preview). For motorized faders, this would correspond to the fader movement.  
    
- Local (this preset only): Saves the Activator with the current preset.1 The user guide provides examples for configuring activators for various common controllers.1

9.3 Triggers: Automating Actions Based on Input Events.

Triggers offer a more granular level of automation compared to global shortcuts or playlists, as they are tied to specific lifecycle events of individual inputs.1 This allows for context-specific actions without manual intervention.

- Configuration: Triggers are set up within an input's Input Settings window, under the Triggers tab.  
    
- Components of a Trigger:  
    
- Trigger Event: The condition that activates the trigger. Options include:  
    
- OnTransitionIn: When the input begins transitioning into the Output window.  
    
- OnTransitionOut: When the input begins transitioning out of the Output window.  
    
- OnOverlayIn: When the input is activated as an overlay.  
    
- OnOverlayOut: When the input is deactivated as an overlay.  
    
- OnCompletion: When a video, list, photo, or PowerPoint input finishes playing (assuming Loop is not enabled).  
    
- OnCountdownCompleted: When a countdown timer within a Title input reaches zero.1  
    
- Function: The action to be performed (selected from the same list as Shortcuts). Note: to prevent loops, transition effects (like Fade, Cut) used as functions have no effect for OnTransitionIn or OnTransitionOut triggers.  
    
- Input: The target input for the function (if applicable).  
    
- Duration: The duration of the function (e.g., for a transition), in milliseconds.  
    
- Delay: The time (in milliseconds) to wait after the trigger event occurs before executing the function.  
    
- Execution: Multiple triggers for the same event on an input will run sequentially in the order they are listed. The maximum duration for a trigger's delay or action is 30 seconds (30,000 ms) to prevent unexpected long-running operations; longer automated sequences should be handled by PlayLists or Scripting.1 For example, a video input could have an OnCompletion trigger that automatically transitions to a specific camera input. A title input could have an OnOverlayIn trigger that starts its associated countdown timer.

9.4 Scripting with VB.NET and Web Scripts: Unleashing Advanced Automation.

For automation needs that go beyond predefined functions, vMix 4K and Pro editions include a powerful Scripting feature.1 This transforms vMix from a configurable application into a programmable platform for advanced users, allowing for bespoke automation, integration with external systems, or complex conditional logic.

- Workflow:  
    
1. Create a script in Settings \-\> Scripting tab and give it a unique Name.  
     
2. Create a Shortcut, set its Function to ScriptStart, and enter the script's Name in the appropriate field.1  
     
- Scripting Languages:  
    
- VB.NET Scripting: vMix supports a significant subset of VB.NET 2.0 code, executed within a single subroutine or function (custom classes/structures are not supported, but many.NET base classes like System.Net.WebClient for HTTP requests are). Scripts can interact with vMix through built-in objects:  
    
- Input Object: Find inputs by name/number/key (Input.Find(...)), access Preview/Output as inputs (Input.Preview, Input.Output), read/write title text fields (anInput.Text("FieldName")), execute shortcut functions on inputs (anInput.Function("Play")), and wait for video completion (anInput.WaitForCompletion(timeout)).1  
    
- Overlay Object: Find overlay channels (Overlay.Find(channelNumber)) and control them (anOverlay.In("InputName"), anOverlay.Out(), anOverlay.Off()).1  
    
- Console Object: Write debug messages to the vMix Script console (Console.WriteLine("message")).1  
    
- API Object: Access the vMix API from within a script, either to retrieve the full XML state (API.XML()) or to execute API functions (API.Function("FunctionName", input:="InputName", value:="Value")).1 This allows scripts to query vMix's state, make decisions, and then control vMix or even other network-connected devices.  
    
- Web Scripting: A simpler syntax for executing a sequence of vMix API functions. Each line uses the same query string format as the HTTP Web API (e.g., Function=OverlayInput1In\&Input=NewsHD.xaml). A unique Sleep command can be used to pause between functions.1  
    
- Local Scripts: Scripts can be saved globally (available in any preset) or locally (saved within a specific preset and only loaded with it). Local scripts are shown in bold in the script list and take precedence if a global script has the same name.1

Scripting enables the development of highly customized solutions, such as integrating with broadcast automation systems, creating custom dashboards, or implementing complex conditional workflows tailored to unique production needs.

9.5 Web Controller: Remote Control via Web-Enabled Devices.

The vMix Web Controller allows for remote operation of many vMix functions using any web-capable device (like a tablet, smartphone, or another computer) on the same network.1 This is enabled by default, and the web address for access can be found in Settings \-\> Web Controller tab.

- Features: The Web Controller interface provides access to:  
    
- Shortcuts: Any configured shortcuts (with their assigned titles/descriptions) can be triggered remotely.  
    
- Switcher: A simplified switching interface resembling a traditional hardware switcher, with Preview, Program, and transition controls.  
    
- Tally Lights: Turns the screen of the connected mobile device into a tally light, changing color based on the status of a selected vMix input (Red for Program, Green for Preview). This is an extremely accessible and low-cost tally solution.1  
    
- Title Editor: Allows remote editing of text fields within Title and XAML inputs in vMix. Users can update live titles or manage title presets from the web interface.1  
    
- Password Protection: Access to the Web Controller can be password-protected for security. Individual pages (Shortcuts, Switcher, etc.) can also be granted access without requiring a password, even if a master password is set.1

The Web Controller facilitates distributed control and collaboration. For example, a director might use a tablet for switching, while another crew member updates titles from a laptop, and camera operators use their phones as tally lights, all untethered from the main vMix PC.

---

Section 10: Optimizing vMix: Key Settings and Monitoring

Ensuring smooth and stable performance is paramount in live production. vMix provides several key settings areas and monitoring tools to help users optimize their system and diagnose potential issues.

10.1 Performance Settings: Graphics Adapter, Latency, High Input Mode.

The Settings \-\> Performance tab contains crucial options for tuning vMix to the specific hardware configuration and production load.1

- Graphics Adapter: This displays the graphics card vMix is currently using. In systems with multiple GPUs (e.g., a laptop with integrated Intel graphics and a dedicated NVIDIA card), it's important that vMix utilizes the more powerful dedicated GPU for optimal performance. This setting should generally match the graphics card to which the main vMix interface monitor is connected. For laptops with NVIDIA Optimus technology, the GPU selection is typically managed through the NVIDIA Control Panel, not directly within vMix.1  
    
- Low Latency Capture: Enabling this option can reduce the latency of camera inputs by approximately one frame. However, this comes at the cost of substantially increased load on the graphics card and may lead to dropped frames under heavy load. It should be used with caution and tested thoroughly in the production environment.1  
    
- High Input Performance Mode: This mode is designed for productions using a large number of camera inputs (typically more than eight) and a high total number of inputs. When enabled, it can improve performance, but it requires a graphics card with a significant amount of built-in memory (3GB or more). Enabling it on systems with less graphics memory or on Intel integrated graphics may result in poor performance.1  
    
- Disable Windows Update while vMix is running: To prevent unexpected performance drops or system restarts during a live production, this option temporarily disables Windows Update while vMix is active. This is a recommended best practice for maintaining stability in live environments.1  
    
- Display Method: This setting controls how vMix renders video to the on-screen Preview and Output windows, as well as to Fullscreen outputs connected to the graphics card. It does not affect the quality or performance of recordings, streams, or external hardware outputs. Options include:  
    
- Auto: vMix selects the best method based on current settings (usually Low Latency for frame rates \< 30fps, Smooth otherwise).  
    
- Low Latency: Prioritizes displaying video as quickly as possible, minimizing on-screen latency, though video playback might appear less smooth.  
    
- Smooth: vMix makes efforts to ensure smooth video playback on the display, which may introduce a couple of frames of additional delay.  
    
- Legacy: Uses the display method employed by older versions of vMix (vMix 20 and earlier).1

These performance settings often involve a balancing act. For instance, "Low Latency Capture" offers quicker response but higher GPU strain. Users need to understand these trade-offs and test configurations to find what works best for their specific hardware and production complexity.

10.2 Decoder Settings: Deinterlacing, Codec Preferences.

The Settings \-\> Decoders tab allows users to configure how vMix handles the decoding of various video file formats and how it processes interlaced video signals.1

- Preferred Deinterlacing: When using interlaced camera sources (e.g., 1080i59.94) in a vMix session that is set to a progressive Master Frame Rate (e.g., 1080p29.97), vMix needs to deinterlace the incoming video. This setting determines the method used:  
    
- Blend: Combines the two fields of an interlaced frame into a single progressive frame. This can result in some motion blur on fast-moving content.  
    
- Discard: Uses the first field of each interlaced frame and discards the second. This avoids motion blur but results in half the vertical resolution compared to Blend for that frame.1  
    
- FFMPEG Decoder Usage: Users can select which video file formats (e.g., QuickTime.MOV files, MXF files are enabled by default in the 64-bit version of vMix) should be decoded using the built-in FFMPEG decoder. This can sometimes provide better compatibility or performance for certain file types.1  
    
- DirectShow Decoders: For other video formats, vMix uses DirectShow decoders installed on the Windows system. This section allows selection of custom DirectShow decoders for various video types (e.g., MPEG-2, H.264), though it's generally recommended to leave these set to "Auto" unless specific issues arise.1  
    
- MPEG 2 Video / Audio Codecs: Specific custom codecs can be selected for playing DVD video (MPEG-2) and its associated audio.1  
    
- Use vMix Deinterlacing (for DVD/MPG): If the selected MPEG-2 video codec does not properly deinterlace DVD/MPG sources, ticking this box allows vMix to handle the deinterlacing.1  
    
- Filters \- Blocked Filter List: This feature can be used to prevent problematic DirectShow filters from being used by vMix. By default, the ffdshow filter pack is often blocked as it can sometimes conflict with vMix's internal decoders.1

10.3 Interpreting the Statistics Window for Performance Monitoring.

The Statistics window (accessed via an icon in the bottom right of the vMix interface, often resembling a graph or heartbeat) provides real-time performance metrics for each live input and for the overall system. Understanding this data is crucial for diagnosing dropped frames, audio sync issues, and other performance bottlenecks.1

Key columns in the Statistics window include:

- Source Dropped: Shows the number of frames dropped by the capture card or camera input itself before even reaching vMix for processing. This could be due to issues with the camera, cable, capture card, or a bandwidth bottleneck on the capture device's connection (e.g., USB, PCIe).1  
    
- Renderer Dropped: Indicates the number of frames dropped by the vMix rendering engine, usually because the graphics card is overloaded and cannot process and display frames quickly enough.1  
    
- Resync: Counts frames dropped because the source (camera/capture card) is running slightly faster than the vMix session's clock, causing vMix to discard extra frames to maintain synchronization.1  
    
- Video (Timing): Displays timing information for incoming video frames. For example, 33 33 33 33 (49) might indicate that the last four frames arrived approximately 33ms apart (consistent with \~30fps), and the number in parentheses (49) shows how long it took for the most recent frame to be processed and displayed by vMix (in this case, about 1.5 frame times at 30fps). Consistent deviations from the expected frame interval (e.g., a 30p camera showing consistent 38ms intervals) can indicate the source is running slow (correlating with "Source Dropped") or fast (correlating with "Resync").1  
    
- Audio (Timing & Buffer): Shows timing statistics for audio samples. This includes values indicating the fullness of the audio buffer (e.g., 60/67 ms), the number of dropped audio samples (read/write), and the amount of audio (in milliseconds) that has been resampled (stretched or compressed slightly in time) to maintain synchronization with the video or the vMix clock.1  
    
- GPU Memory Usage, CPU Usage, Render Time: Other critical statistics often displayed (though not explicitly detailed for every column in the snippet for the Statistics window itself, these are common vMix performance indicators seen elsewhere like the status bar) include the GPU's memory consumption, overall CPU utilization by vMix, and the render time (in milliseconds) – how long it takes the GPU to render a single frame. If render time consistently exceeds the frame interval (e.g., \>33ms for a 30fps session), frames will be dropped.

Monitoring these statistics, especially during demanding parts of a production, helps identify whether performance issues are source-related, GPU-bound, or CPU-bound, guiding troubleshooting efforts.

10.4 Key Display Settings: Frame Rate, Output Size, Fullscreen Configuration.

The Settings \-\> Display tab controls fundamental aspects of the vMix production's video format and how it's displayed on connected monitors.1

- Master Frame Rate: This is a critical setting that defines the base frame rate for the entire vMix session (e.g., 29.97p, 50p, 59.94i). All inputs will be converted to this frame rate. It should ideally be set to match the frame rate of the primary video camera sources where possible to minimize conversions.1  
    
- Output Size (Resolution): This sets the master resolution (e.g., 1920x1080, 1280x720, 3840x2160) to which all inputs are scaled before being sent to Fullscreen display, Recording, External Output, or Streaming.1  
    
- Output Aspect Ratio: Defines the aspect ratio of the output display (e.g., Widescreen 16:9, Normal 4:3).1  
    
- Fullscreen Display Configuration: vMix can send a dedicated fullscreen output of its Program feed (or other sources like Preview or MultiView) to a secondary monitor, projector, or TV connected to the computer's graphics card.  
    
- Display: Selects which connected screen (Display 1, Display 2, etc.) will be used for the fullscreen output. Display 1 is always the primary Windows desktop.  
    
- Position: By default, the fullscreen output fills the entire selected display. Custom position and size can be set if needed.  
    
- Hide Cursor, On Top, Minimise: Options to control cursor visibility, ensure the fullscreen window stays on top of other windows (if on a different display), and minimize the fullscreen window when vMix is minimized.1  
    
- Multiple Fullscreen Outputs: vMix 4K and Pro editions support up to two independent fullscreen outputs, configurable if the graphics card supports three or more simultaneous displays.1  
    
- Input Size: Controls the size of the input preview thumbnails in the main vMix window. This can be increased on larger screens for clearer visibility of each input.1

10.5 Understanding Outputs / NDI Settings.

The Settings \-\> Outputs / NDI tab is central to configuring what content is sent to vMix's various output channels and how NDI is utilized.1

- Output Channels (Output 1, 2, 3, 4): vMix editions offer a varying number of independent output channels (vMix 4K/Pro have more).  
    
- Output 1 (Program): This is the primary mixed output of vMix, used by default for Recording, Streaming, and External Output 1\.  
    
- Output 2, 3, 4: These are additional independent outputs. For each, users can select what source it shows: the main Output (Program), the Preview window, a MultiView configuration, or a specific Input. Changes to these output assignments can affect what is seen on corresponding External Outputs (e.g., External 2 shares with Output 2\) or NDI feeds.1  
    
- NDI Output Configuration:  
    
- Cameras / Calls / Audio Inputs: Ticking this option automatically converts all active camera inputs, vMix Call guest feeds, and dedicated Audio Inputs in the current vMix session into live, individual NDI outputs available on the network.1  
    
- Audio Outputs (NDI): Enabling this converts all enabled audio buses (Master, Headphones, A-G from Audio Outputs settings) into live, audio-only NDI outputs.1  
    
- Per-Output NDI Settings (Cog Icon): Next to each main output (Output 1-4), a cog icon allows access to specific NDI settings for that output, such as selecting a different Audio Bus to send with that NDI feed, or enabling Alpha Channel support (Straight or Premultiplied) for sending keyed graphics over NDI.1  
    
- Overlay Customization per Output: If an output channel (e.g., Fullscreen, Output 2\) is set to show "Output" (the main program mix), checkboxes allow customization of which overlay channels (1-4) are visible on that particular output. This enables scenarios like sending a "clean feed" (main program video without overlays) to a recording, while the Fullscreen display for a live audience includes all overlays.1  
    
- MultiView Output Configuration: If an output is set to show "MultiView," this section allows customization of the MultiView layout (e.g., which inputs appear in which slots of the multiviewer grid) and the position/content of titles within the MultiView display.1

These output settings provide immense flexibility in tailoring different feeds for various destinations, whether they are local displays, recordings, streams, or other devices on an NDI network.

10.6 Common Troubleshooting Solutions from FAQs.

The vMix User Guide includes FAQ and troubleshooting sections for features like vMix Call and general streaming, offering solutions to common problems.1

- vMix Call Issues:  
    
- No video/audio from guest: Ensure guest has selected their webcam/microphone in the browser settings. In Chrome, this is often via a camera icon in the address bar; Firefox prompts on connection.1  
    
- Guest drops out: Usually due to internet interruption. Guest should refresh their browser page to reconnect.1  
    
- Guest flashing orange/amber in Call Manager (network congestion): vMix Call adapts, but if the return video bandwidth from vMix to the guest is too high for the guest's connection, the operator may need to lower it (right-click Call input in vMix).1  
    
- Low quality video/audio from guest: Can be due to guest's upload speed being below 2Mbps, or temporary network congestion. A different webcam might also help if network is stable.1  
    
- Video/audio not smooth: Frame rate can drop during network congestion or due to guest's device performance or poor camera lighting.1  
    
- High Latency: The Jitter Buffer in vMix Call adds latency (200ms to 1.5s+) for smoothness. If latency becomes excessive after congestion, guest refreshing browser can reset it.1  
    
- Audio echo from guest: Guest must use headphones/earphones, not speakers, to prevent return audio feeding back into their microphone. If speakers are unavoidable, a directional mic is needed.1  
    
- General Streaming Issues:  
    
- Error on starting stream: Double-check RTMP URL, Stream Key, and any login credentials match those provided by the streaming platform.1  
    
- Hardware Encoder limitations: Remember the 2-simultaneous-encode limit on NVIDIA GeForce cards if also recording with hardware encoding.1  
    
- Stream errors on one destination (multi-destination streaming): If one stream fails, others continue. The failed stream can be restarted manually once the issue (e.g., platform outage, incorrect key) is resolved.1

---

Section 11: Conclusion: Harnessing the Power of vMix

vMix presents itself as an exceptionally comprehensive and scalable software solution for live video production, recording, and streaming. Its architecture, which consolidates a vast array of traditionally hardware-based functionalities into a single PC application, offers significant advantages in terms of cost-effectiveness, flexibility, and operational efficiency.1 The software's support for various resolutions from SD to 4K, coupled with a tiered edition structure, allows it to cater to a wide spectrum of users, from individual content creators to professional broadcast operations.1

A recurring theme throughout the exploration of vMix's features is its deep customizability and emphasis on user-defined workflows. From the organization of inputs into categories and rows 1 to the extensive Shortcut and Activator systems 1, users are empowered to tailor the interface and control mechanisms to their specific needs and preferences. This is crucial in the fast-paced environment of live production, where quick and intuitive access to functions can make a significant difference.

The software's robust input management, supporting a multitude of sources including physical cameras, video files, NDI feeds, web content, and remote guests via vMix Call 1, underscores its role as a central hub in modern production ecosystems. The integration of advanced features like multi-channel Instant Replay, network-based PTZ camera control, dynamic Virtual Sets, and data-driven titles further elevates its capabilities beyond simple switching.1 These features, while often demanding on system resources, provide tools that rival dedicated, and often much more expensive, hardware solutions.

The extensive audio mixing capabilities, including multiple buses, per-input EQ, compression, noise gating, and VST3 plugin support, demonstrate that vMix treats audio as a first-class citizen, not merely an adjunct to video.1 This integrated approach can simplify setups and reduce the need for external audio hardware in many scenarios.

For output and distribution, vMix offers a wealth of options. The ability to record in multiple formats, including fault-tolerant ones like vMix AVI and MKV, provides reliability and flexibility for post-production.1 The sophisticated streaming module, supporting multiple destinations, multi-bitrate encoding, and hardware acceleration, ensures that productions can reach a wide audience with optimal quality.1 Furthermore, comprehensive NDI support for both input and output, including alpha channel, positions vMix as a key player in IP-based video workflows.1

However, the power and flexibility of vMix come with the need for users to understand its intricacies and the capabilities of their underlying hardware. Features like high-channel Instant Replay, 4K production, or extensive use of hardware encoding have specific and often demanding system requirements, particularly concerning CPU, GPU, and storage speed.1 Users must carefully consider these requirements to ensure a stable and performant system.

In conclusion, vMix is a remarkably powerful and adaptable live production software. Its strength lies not only in its extensive feature set but also in its ability to be customized and automated to fit a wide range of production scales and complexities. By investing time in understanding its core concepts, input/output configurations, and advanced features, users can unlock a professional-grade production environment capable of delivering high-quality results for a multitude of applications. The ongoing development and inclusion of modern protocols like NDI and SRT, alongside user-focused features like vMix Call and comprehensive control options, suggest a commitment to evolving with the needs of the live production industry.

#### **منابع مورداستناد**

1. 8 vMix User Guide \[English\]\[Live Stream\]..pdf  
     
2. Supported Hardware | vMix, زمان دسترسی: ژوئن 11, 2025، [https://www.vmix.com/software/supported-hardware.aspx](https://www.vmix.com/software/supported-hardware.aspx)  
     
3. System Requirements \- vMix User Guide, زمان دسترسی: ژوئن 11, 2025، [https://www.vmix.com/help24/SystemRequirements.html](https://www.vmix.com/help24/SystemRequirements.html)

\*\*  
