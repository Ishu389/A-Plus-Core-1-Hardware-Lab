# Lab Log #01: Second-Hand Desktop Teardown and Rebuild

**Date:** A couple of months ago (Post-Core 1 Exam Prep)  
**Objective:** Take a cheap, used second-hand desktop completely apart, clean it, inspect the components, and rebuild it to a fully functional POST state.

## 🖥️ The Donor PC Spec Sheet
I bought a cheap used tower locally to mess around with without breaking my main rig.
* **CPU:** Intel Core i5 (4th Gen) LGA 1150 socket
* **Motherboard:** OEM Micro-ATX board
* **RAM:** 8GB DDR3 (Single stick, unbuffered)
* **Storage:** 240GB SATA SSD (Mounted loosely in the bay)
* **PSU:** Generic 450W non-modular power supply

---

## 🛠️ The Disassembly Process
1. **Safety First:** Unplugged the system and held the power button for 10 seconds to drain any leftover power in the capacitors. Set up on a clean wooden table.
2. **The Rip-Out:** 
   * Disconnected all SATA data cables and the chunky 24-pin ATX power connector.
   * Unscrewed the stock Intel CPU cooler. The thermal paste was absolutely bone-dry—practically turned to cement. 
   * Popped the load lever on the LGA socket and carefully pulled the i5 chip out, making sure not to touch or bend the motherboard pins.
3. **Deep Cleaning:** Used 91% Isopropyl alcohol and a microfiber cloth to dissolve the crusty thermal paste off the CPU lid and the copper base of the heat sink. Used a compressed air can to blow out years of dust from the cooling fins and the RAM slots.

---

## 🔧 Reassembly & The Twist
Putting it back together was mostly smooth, but it gave me a real-world troubleshooting moment.

* **Thermal Paste:** Applied a pea-sized drop of fresh thermal compound right in the middle of the CPU integrated heat spreader. Mounted the cooler back down in a cross-pattern to keep the pressure even.
* **The Mistake (Human Error!):** First time I put the RAM back in, I didn't push hard enough on one side. The clip didn't click. 
* **The Result:** When I plugged the monitor in and hit power, the fans spun up, but the screen stayed black. No display, and the motherboard started giving me short repeating beeps.
* **The Fix:** Recognised the beep code as a memory issue. Powered down, pulled the RAM out, reseated it firmly until both sides clicked, and tried again.

## 📺 Boot Results
Success! The machine cleared the Power-On Self-Test (POST), loaded into the BIOS successfully, and correctly identified the i5 CPU and the full 8GB of DDR3 RAM. 

### Key Takeaways from this lab:
* Never trust the previous owner's thermal paste.
* Double-check RAM seating before screwing the case side-panel back on.
* Beep codes from Core 1 studies are incredibly real and helpful.
