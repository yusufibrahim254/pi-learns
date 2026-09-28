# pi-learns

A Raspberry Pi 5 that learns to recognize things I teach it, built from scratch to learn **how AI actually works** and **how to use Linux comfortably**.

The end goal is a headless Pi that watches through a camera or reads Arduino sensors, recognizes things I trained it on, logs what it sees, and serves a small status page on my home network. It should start itself at boot and recover on its own.

---

## Roadmap

### Stage 1 — Living in the terminal
- [ ] Flash the OS and boot the Pi headless (no monitor or keyboard)
- [ ] Connect over SSH from my laptop
- [ ] Create my own user, set up SSH keys, disable password login
- [ ] Learn the filesystem layout (`/etc`, `/var/log`, `/home`, …)
- [ ] Understand file permissions and ownership
- [ ] Install and remove packages with `apt`
- [ ] Monitor CPU, RAM, disk, and temperature
- [ ] Set up git on the Pi and push to this repo over SSH
- **Checkpoint:** reboot, reconnect, and explain every command in my shell history

### Stage 2 — A neural network with no AI libraries
- [ ] Set up a Python virtual environment
- [ ] Get the MNIST dataset onto the Pi
- [ ] Write a neural network using only NumPy (forward pass, loss, backprop, training loop)
- [ ] Train it and track accuracy over epochs
- **Checkpoint:** above 90% accuracy, and I can explain what backpropagation is doing

### Stage 3 — Real tools, real data
- [ ] Rebuild the Stage 2 model in PyTorch and compare it with my hand-built one
- [ ] Collect my own dataset (camera photos or Arduino sensor readings)
- [ ] Train a model on my own data
- [ ] Run inference on the Pi and measure speed
- [ ] Investigate why it's slow, and try a way to make the model smaller or faster
- **Checkpoint:** the Pi recognizes my own things in real time, or close to it

### Stage 4 — Make it a real system
- [ ] Run the recognizer as a service that starts at boot and restarts on crash
- [ ] Log results to files, with log rotation
- [ ] Serve a small status web page on the home network
- **Checkpoint:** unplug the Pi, plug it back in, and everything comes back on its own

### Bonus — Language models
- [ ] Run a small local LLM on the Pi
- [ ] Have it describe what the recognizer saw in plain English
- [ ] Write up how it differs from the model I trained myself

---

## Learning log

Short notes after each session: what I tried, what broke, and what I learned. See [`notes/`](notes/).

| Date | Stage | What I learned |
|------|-------|----------------|
|      |       |                |

---

## Hardware
- Raspberry Pi 5
- Camera module *(if available)*
- Elegoo Arduino starter kit *(sensors for Stage 3)*
