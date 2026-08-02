# EMR Picking Sequence Optimizer - Warehouse Scheduling Optimization 2026

> **EMR Picking Sequence Optimizer is a browser-based planning tool for improving pallet-picking schedules in dense mobile-rack warehouses through bi-objective optimization, hybrid genetic search, and interactive 3D replay.**

[![Platform](https://img.shields.io/badge/Platform-Web%20browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/andrewfisheruos5642/emr-picking-optimizer-2026?style=flat-square)](https://github.com/andrewfisheruos5642/emr-picking-optimizer-2026)

---

<p align="center">
  <a href="https://andrewfisheruos5642.github.io/emr-picking-optimizer-2026/">
    <img src="https://img.shields.io/badge/Download-EMR%20Picking%20Sequence%20Optimizer%20Latest-brightgreen?style=for-the-badge" alt="Download EMR Picking Sequence Optimizer">
  </a>
</p>

> **[Download the latest build](https://andrewfisheruos5642.github.io/emr-picking-optimizer-2026/)**

---

[Download Latest Build](https://andrewfisheruos5642.github.io/emr-picking-optimizer-2026/)

---

## Overview

EMR Picking Sequence Optimizer is intended for warehouse planning teams managing dense mobile-rack configurations. Instead of reducing scheduling to one metric, it compares candidate picking sequences using two objectives: aisle-switching effort and weighted tardiness.

Its optimization workflow uses a dual-stage hybrid genetic algorithm, injects greedy solutions, and applies a physical movement-cost model covering forklifts and racks. Once a result has been calculated, users can study it in a time-scaled 3D replay with several camera angles and export the visuals for analysis, presentations, or operational discussions.

---

## Capabilities

- Evaluate picking schedules against aisle-switching effort and weighted tardiness
- Apply a dual-stage hybrid genetic algorithm with greedy solution injection
- Model movement costs involving forklifts, racks, and aisle access
- Represent dense mobile-rack warehouses containing up to 960 slots
- Replay computed picking sequences in an interactive 3D warehouse
- Match playback timing to the schedule through time-proportional animation
- Import solution sequences from CSV files
- View the warehouse from isometric, plan, or elevation perspectives
- Save PNG snapshots and record replays as WebM
- Use Three.js for warehouse visualization and simulation

---

## Getting Started

### Open the hosted application

The browser version is available here:

[Launch EMR Picking Sequence Optimizer](https://andrewfisheruos5642.github.io/emr-picking-optimizer-2026/)

No native installer is needed for ordinary use because the project is provided as a web application.

### Serve the project locally

Clone the repository, move into its directory, and serve the files through a local HTTP server:

    git clone https://github.com/andrewfisheruos5642/emr-picking-optimizer-2026.git
    cd REPO

After starting any static web server available in your environment, open the local address it reports in a supported browser. HTTP serving is recommended for reliable browser behavior.

---

## Typical Workflow

The usual planning and review process looks like this:

1. Start the application in a current web browser.
2. Import a solution sequence from a CSV file.
3. Check the warehouse layout and scheduling inputs.
4. Run the optimization or inspect an existing result.
5. Compare aisle-switching activity with weighted tardiness.
6. Use replay controls to follow forklift and rack movement.
7. Change among isometric, plan, and elevation camera views.
8. Export a PNG image or record the replay in WebM format.

Time-proportional playback is useful when examining both the movement order and the timing of activity throughout the warehouse.

---

## Input and Configuration

CSV files provide the main input path. Prepare a solution sequence using the format expected by the application, then load it through the web interface.

    sequence.csv

The application manages configuration through its controls and imported data; there is no separately documented configuration file. Keep imported files on hand so schedules and replay settings can be reloaded during comparisons.

---

## System Requirements

- A modern desktop browser with JavaScript enabled
- WebGL capability for the Three.js warehouse visualization
- A local HTTP server for running the cloned project
- CSV files when importing solution sequences
- Adequate browser memory for dense warehouse layouts and 3D replay
- Storage space for exported PNG files and WebM recordings

The optimizer supports dense mobile-rack environments with up to 960 slots.

---

## Frequently Asked Questions

### Do I need to install a desktop application?

No. The intended environment is a web browser. You can also serve a cloned copy through a basic local HTTP server.

### Does the application accept an existing picking sequence?

Yes. Existing solution sequences can be imported as CSV files. The file must follow the column structure expected by the application.

### Which scheduling measures are optimized?

The optimizer considers aisle-switching effort and weighted tardiness. Together, these objectives represent warehouse movement activity and schedule lateness.

### How do I review an optimization result?

Open the interactive replay to watch the simulated warehouse operations. Playback follows the schedule timing, and the interface includes isometric, plan, and elevation views.

### Are visual results exportable?

Yes. You can save the current view as a PNG snapshot or record the replay as WebM.

### What can I do if the 3D warehouse view is blank?

First verify that JavaScript and WebGL are enabled, then reload the application in a current browser. For local testing, confirm that the project is being served over HTTP instead of opened directly from the filesystem.

### Where do I get updates?

The hosted build contains the latest published browser version. For a local installation, pull newer repository changes as they become available.

---

## Future Directions

Possible areas for later development include:

- More extensive schedule comparison workflows
- Additional warehouse layouts and movement scenarios
- Deeper controls for replay analysis
- Expanded export and reporting capabilities

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
