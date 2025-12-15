+++
title = 'The First Step into the Temple: How I Started My Linux Journey'
date = '2025-12-15T12:04:44+07:00'
draft = false
description = 'The Story about me and Linux distros'
categories = ['linux-scripting']
tags = ['linux']
showHero = true
+++

I remember exactly when I first entered the world of **Linux**. It was during my third year of university.

I didn't switch because I wanted to be "that Linux guy" in class, or because of the fancy features everyone talks about. My Windows laptop simply couldn't handle the workload anymore. Between running heavy **Java** applications and trying to spin up multiple **Docker** containers, my machine just can not handle it.

I knew it was time to try something different—something I had always wanted to do but never did. I decided to install **Linux**.

Like any other guys that made the first step into **Linux**, it was like a maze of distro, kernel or desktop environment. It was exciting. Choosing a distro felt like picking a **character class** in an RPG video game—each one looked unique, specialized, and just plain cool.

This is how my journey started. Now, I want to share that journey with you.

## The Obvious Choice: Ubuntu

I think this is how **90%** of us start our **Linux** journey. I went searching on the Internet and ended up with the default choice: **Ubuntu**.

The first time booting **Ubuntu** on my **Asus TUF Gaming Laptop** was unforgettable. I was so satisfied with how it looked, how it felt, and how every **GNOME** component worked together. The UI was strange yet magical to me. I spent two days exploring this new OS, installing everything I wanted, and playing with the terminal (since I already had some experience fighting with **WSL2**). Everything felt perfect.

Unfortunately, the honeymoon didn't last long. Once I had my full stack installed — **VS Code**, **Docker**, **IntelliJ**, **Postman** — the reality hit.

Don't get me wrong, the native **Docker** performance was out of this world compared to **Windows**. But when I stopped playing around and tried to do actual work, I faced the exact same problem that made me leave **Windows**.

Everything was just... heavy. I don't know how else to explain it, but the system felt sluggish. My laptop only had **8GB** of **RAM** at the time, so running two **Postgres** databases alongside my **Spring Boo**t project made everything crawl.

Only later did I discover that **Snap** packages were the likely culprit behind the sluggishness. But by the time I realized that, it was too late. I had already set my sights on my next destination: **Linux Mint**.

## The Antidote : Linux Mint

If **Ubuntu** is the most famous distro, then **Linux Mint** is arguably the most loved.

All I knew about **Mint** at the time was that it was based on **Ubuntu** and offered the most **Windows-like** experience.

The setup process was pain-free. It came with almost everything I needed out of the box. But the real game-changer—and the reason I stayed—was the performance. It was incredibly smooth and lightweight, completely solving the lag issues I had with **Ubuntu**.

I used the **Cinnamon** edition. Since the interface was so similar to **Windows**, I felt at home immediately. It might sound weird for a "distro hopper," but I barely customized anything on Mint.

That turned out to be a blessing in disguise. By spending less time tweaking the UI, I had more time to mess around with the terminal—which became my favorite playground.

This is where I spent the most significant part of my early **DevOps** journey. It was on **Mint** that I truly got my hands dirty with the OS, the command line, coding, and cloud computing.

One final thing I have to mention: **NVIDIA Drivers**. On other distros, this can be a nightmare, but **Mint’s Driver Manager** made it a breeze. Huge thanks to the **Mint** team for that.

I honestly thought **Mint** would be my endgame. But as my love for Linux grew, so did my curiosity. I knew I had to dig deeper into the **Linux** ecosystem.

## The Professional Turn: Fedora

**Linux Mint** is fantastic, and I would still recommend it to anyone starting their **Linux** journey today.

However, as I got more comfortable, I hit a bottleneck: The Kernel. Since Mint is based on **Ubuntu LTS**, the kernel is often outdated. It has to wait for **Ubuntu** to update, and then **Mint** updates itself. I wanted something fresher.

That’s when I heard about **Fedora**—the distro recommended by **Linus Torvalds**, the creator of Linux himself.

It wasn't just the celebrity endorsement that drew me in. I learned that **Fedora** ships a "Vanilla" kernel, meaning they barely modify the original code. While other distros patch and tweak the kernel, **Fedora** delivers it almost exactly as the developers intended.

It was also time for me to leave the **Debian**-based ecosystem (**Ubuntu**, Mint, Pop!_OS) and try something new. And surprisingly, I fell back in love with **GNOME**. While I hated it on **Ubuntu**, the "pure" GNOME experience on **Fedora** feels modern, fluid, and has excellent UX. Some say it’s a macOS clone, but honestly? I love it.

The performance difference was immediate. Access to a newer kernel meant better hardware support and features that didn't exist in older versions. But the biggest win was the lack of bloat. I was traumatized by **Snap** packages on **Ubuntu**; they were just too heavy for daily usage.

**Fedora** was a breath of fresh air. **DNF** (the package manager) is a game-changer—it’s structured, reliable, and combined with **Flatpak**, it fulfills all my software needs without slowing down the system.

This was also where I started experimenting with advanced workflows. I moved to i3 (a tiling window manager), and **Fedora** handled it perfectly.

Overall, **Fedora** remains my top choice for professional work. It strikes the perfect balance between stability, bleeding-edge features, and a clean user experience.

## The Monk’s Path: Void Linux

If **Linux Mint** is a comfortable home and **Fedora** is a high-tech office, then **Void Linux** is an empty dojo high up in the mountains.

I didn't switch to **Void** because I needed another daily driver. I switched because I wanted to understand **Linux** at its core. I was tired of "magic" happening in the background. I wanted full control.

**Void** is not for the faint of heart. It doesn't hold your hand. There is no graphical installer welcoming you with a slideshow. From the moment you boot the live **ISO**, the system expects you to know what you are doing—or at least, be willing to read the documentation and learn the hard way.

The biggest culture shock—and the main reason I came here—was the init system. Every other distro I had used (**Ubuntu**, **Mint**, **Fedora**) relied on **systemd**. While powerful, **systemd** is complex and does a lot of things behind the scenes.

**Void** uses **runit**.

The difference was night and day. **runit** is incredibly simple. It doesn't try to do everything; it just starts your services and gets out of the way. For the first time, I could actually read and understand the scripts that started my computer. It wasn't a black box anymore; it was transparent.

And the payoff? Speed. Absolute, raw speed.

My laptop boots faster than I can open the lid. The system feels instantaneous. When I log in, the system idles at around **200MB** of **RAM**. Coming from the heavy memory usage of **GNOME** on **Ubuntu**, this felt like magic. There is zero bloat because you are the one adding every single package. Nothing exists on your drive without your permission.

**Void** isn't just an Operating System to me; it's a philosophy. It forced me to stop relying on automated tools and start understanding how filesystems, permissions, and services actually interact under the hood.

It didn't just make me a better **Linux** user; it made me a better engineer. This pursuit of simplicity, control, and deep understanding is exactly why I started this blog.

It is the path of the **Linux Monk**.
