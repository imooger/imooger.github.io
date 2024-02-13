---
layout: page
menubar: docs_menu
title: Installation
subtitle: Getting Started
show_sidebar: false
toc: false
---

# Installation
The recommended method to install **adix** is via [pip](https://pypi.org/project/adix/), the Python package manager.


{% include notification.html
message="**adix is still under development** If you encounter any data, compatibility, or installation issues, please don't hesitate to reach out!"
status="is-warning"
icon="fas fa-rocket"
%}


1. **Standard Install**:
   ```bash
   pip install adix
   ```

2. **Specific Version**:
   ```bash
   pip install adix==0.2.0
   ```

3. **Upgrade to Latest Version**:
   ```bash
   pip install adix --upgrade
   ```
   or

   ```bash
   pip install adix -U
   ```

4. **Install just requirements.txt**:
   ```bash
   pip install -r requirements.txt
   ```
5. **Install without Dependencies**:
   ```bash
   pip install --no-deps adix
   ```

<!-- 5. **Install from Source**:
   ```bash
   pip install /path/to/adix
   ```

6. **Install in Editable Mode**:
   ```bash
   pip install -e /path/to/adix
   ``` -->
