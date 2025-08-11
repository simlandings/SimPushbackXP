# SimPushbackXP by SimLandings

**Version:** 0.0.12-dev  
Pushback utility for X-Plane 12 with multiple tug types, smart directional control, and realistic tug visuals.

---

## ✈️ Features
- **Multiple tug types** — choose from various pushback vehicles with distinct performance.  
- **Smart directional pushback** — set direction via compass or nearest taxiway alignment.  
- **Realistic tug visuals** — bundled OBJ model ensures visibility without external libraries.  
- **Logging system** — detailed logs in `SimPushbackXP.log` for troubleshooting.  
- **Error database** — common error codes documented for quick fixes.  

---

## 📦 Installation
1. Ensure you have **[XPPython3](https://xppython3.readthedocs.io/en/latest/)** installed in:
   ```
   X-Plane 12/Resources/plugins/XPPython3
   ```
2. Download the latest release of SimPushbackXP from the [Releases page](../../releases).  
3. Extract the archive and place the **PythonPlugins** folder into:
   ```
   X-Plane 12/Resources/plugins/
   ```
4. Start X-Plane 12 and check under **Plugins → SimPushbackXP by SimLandings**.

---

## 🕹 Usage
1. From the **Plugins** menu, select **SimPushbackXP by SimLandings**.  
2. **Choose Tug Type** → Pick from available models.  
3. **Choose Direction** → Use compass headings or taxiway-based alignment.  
4. **Set Distance** → Optional; skip to use default push length.  
5. **Start Pushback** → Tug attaches and moves aircraft accordingly.  

---

## 🛠 Troubleshooting
- **Plugin not visible:** Ensure `PI_SimPushbackXP.py` is in `PythonPlugins` and file is unblocked in Windows.  
- **No tug visible:** Confirm OBJ model exists in plugin folder; see `E-0007` in [CHANGELOG.md](CHANGELOG.md).  
- **No movement:** See `E-0005` in changelog for loop registration fix.  
- **Crashes:** Check `SimPushbackXP.log` and [XPPython3Log.txt](XPPython3Log.txt).  

---

## 📜 Version History
See the [CHANGELOG.md](CHANGELOG.md) for a complete list of versions and known issues.

---

## 🌐 Connect with SimLandings
- **Website:** [simlandings.com](https://simlandings.com)  
- **YouTube:** [@Sim.Landings](https://www.youtube.com/@Sim.Landings)  
- **Instagram:** [@sim.landings](https://www.instagram.com/sim.landings/)  

---

⭐ If you enjoy SimPushbackXP, please **star** this repo and follow SimLandings for updates!
